#HSLIDE

An Introduction to <span style="color:#e49436">GitHub Flow</span>!

![Logo](assets/git-pull-request.png)


#HSLIDE
Contents

- Branch 
- Code
- Pull Request

#HSLIDE

There is an introduction to <span style="color:#e49436">git</span> here...

https://www.gitpitch.com/frozenskys/githubflow-docs/introduction-to-git


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

#VLSIDE

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