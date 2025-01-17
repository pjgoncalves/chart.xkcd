---
title: Getting started
---

It's easy to get started with chart.xkcd. All that's required is the script included in your page along with a single `<svg>` node to render the chart.

In the following example we create a line chart and render that in our page.

```html
<svg class="bar-chart" width="600" height="400" ></svg>
<script src="../dist/chart.xkcd.js"></script>
<script>
  const svg = document.querySelector('.bar-chart')

  new chartXkcd.Bar(svg, {
    data: {
      labels:['github stars', 'patrons'],
      datasets: [{
        data: [100, 2],
      }]
    },
  });
</script>
```

**Result**

<p class="codepen" data-height="424" data-theme-id="light" data-default-tab="result" data-user="timqian" data-slug-hash="GRKqLaL" style="height: 424px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="chart.xkcd example">
  <span>See the Pen <a href="https://codepen.io/timqian/pen/GRKqLaL/">
  chart.xkcd example</a> by timqian (<a href="https://codepen.io/timqian">@timqian</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>