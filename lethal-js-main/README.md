# lethal-js

A clean framework for creating web-proxies with just 4 lines of code
## reworked by GD-Cybernetix
### reworks
  - fixed up file paths
  - fixed css (borders, margins, etc)
### working on
  - q param system for embedding


# Usage

> [!IMPORTANT]  
> You need to move the contents of `/lethal-js` to your root folder (due to scope issues)

```js
import { setTransport, setWisp, makeURL, getProxied } from "/lethal.js";

const frame = document.getElementById("frame");

setTransport("epoxy");
setWisp("wss://wisp.mercurywork.shop/wisp/");

frame.src = await getProxied(makeURL("Hello World!"));
```

See `example.html` for more.
