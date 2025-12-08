# Plot: Dual axis chart

To implement a dual-axis chart, we remap _efficiency_ to its equivalent value in _sales_ using a linear scale. Ref. [#147](https://github.com/observablehq/plot/issues/147).

```js




  ```



  ```js echo
  const v1 = cars.map(d => d["sales"]);
  const v2 = cars.map(d => d["efficiency"])
  //const y2 = d3.scaleLinear(d3.extent(cars, v2), [0, d3.max(cars, v1)]);



  Plot.plot({
    x: {tickFormat: ""}, // no comma for years
    y: {axis: "left", label: "sales (M)", transform: (d) => d / 1e6}, // show sales in millions
    marks: [
      Plot.axisY( {color: "steelblue", anchor: "right", label: "efficiency (mpg)"}),
      Plot.ruleY([0]),
      Plot.lineY(cars, {x: "year", y: v1}),
      //Plot.lineY(cars, Plot.mapY((D) => D.map(y2), {x: "year", y: v2, stroke: "steelblue"}))
    ]
  });

```

```js echo
const cars = FileAttachment("./data/new-passenger-cars.csv").csv({typed: true})
```
