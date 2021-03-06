This repository is now a part of [qubyte/toisu-monorepo](https://github.com/qubyte/toisu-monorepo).

# toisu-static

[![Greenkeeper badge](https://badges.greenkeeper.io/qubyte/toisu-static.svg)](https://greenkeeper.io/)

A tiny wrapper around serve-static for Toisu!

This module accepts the same arguments as
[serve-static](https://github.com/expressjs/serve-static).

## Example

```javascript
const http = require('http');
const Toisu = require('toisu');
const serveStatic = require('toisu-static');

const app = new Toisu();

// Serve the "public" directory (relative to the app root).
app.use(serveStatic('public'));

http.createServer(app.requestHandler).listen(3000);
```
