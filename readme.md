# Syntax Highlighting for Odin

```ts
import "./ayu-mirage.css"; // or any other style you like
import hljs from "highlight.js";
import odin from "./odin-hl";
hljs.registerLanguage("odin", odin);
// after dom-loads:
hljs.highlightAll();
```

Note that procedure highlighting is turned off as it doesnt appear that highlight.js applies its rules recursively, once a function body is consumed the correct colors cannot be applied to variables or types (at least on a cursory attempt).
