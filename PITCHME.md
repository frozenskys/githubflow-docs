#HSLIDE

An Introduction to <span style="color:#e49436">GitHub Flow</span>

![Logo](assets/github.png)

#HSLIDE

Before we start...

There is an introduction to <span style="color:#e49436">git</span> here if you need it...

https://www.gitpitch.com/frozenskys/githubflow-docs/introduction-to-git

#HSLIDE

Github Flow

"GitHub Flow is all about short feedback loops (everything in DevOps mostly is, actually). This means work branches (‘work’ could mean a new feature or a bug fix – there is no distinction) starts from the production code (master) and are short lived – the shorter the better. Merging back becomes a breeze and we are truly continuously integrating."

#VSLIDE
Our Current Status

![Logo](assets/hell-on-earth.png)

#VSLIDE

GitHub Flow

![Logo](assets/githubflow.png)

#HSLIDE

Branching

- Branches should be short lived
- Never develop on master! 

#VSLIDE

![Logo](assets/branching.png)

#VSLIDE

Create a new branch from the current and check it out 

```bash
git checkout -b well-named-feature
```

#VSLIDE

Write some Code...

```javascript
var express = require('express');
var app = express();

app.get('/', function (req, res) {
  res.send('Hello World!');
});

app.listen(3000, function () {
  console.log('Example app listening on port 3000!');
});
```

#HSLIDE

The End :)