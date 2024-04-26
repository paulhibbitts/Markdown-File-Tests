<div data-runkit>

```javascript
var R = require("ramda");
var randrange = require("random-number-in-range");
var d3Graph = require("@runkit/runkit/d3-graph/1.0.0");

var count = 100;
var nodes = R.range(0, 100).map((_, x) => ({ "name": x, "group": Math.floor(x * 7 / count) }));

var links = R.range(0, Math.floor(count * 1.15)).map(function(_, x) {
    var source = x % count;
    var target = Math.floor(Math.log(1 + randrange(0, count)) / Math.log(1.3));
    var value = 10.0 / (1 + Math.abs(source - target));

    return { "source": source, "target": target, "value": value };
});

d3Graph(nodes, links);
```

</div>

**Tip:** Press <kbd>⇧ Shift</kbd> <kbd>⌤ Enter</kbd> to "run" the notebook.
