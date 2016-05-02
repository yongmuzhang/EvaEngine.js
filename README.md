# EvaEngine For Node

A development engine for NodeJS.



## Quick Start

``` js
import EvaEngine from 'evaengine/src/engine';
const engine = new EvaEngine({
  projectRoot: `${__dirname}/..`,
  port: process.env.PORT || 3000
});

engine.bootstrap();
EvaEngine.getApp().use('/', 
  (req, res) => { res.json({ hello => 'world'}); });
engine.run();
```