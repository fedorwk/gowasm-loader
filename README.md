# gowasm-loader
Script for setting up runtime for golang generated WASM and loading WASM programm itself
## Usage
HTML:  
```html
<script type="module">
	import {default as setupWasm} from './gowasm.js'
	setupWasm('main.wasm')
</script>
```
Separate call for setting up the runtime and loading the WASM file:  
```javascript
import { setupRuntime, loadWASM } from './gowasm.js'  
	
setupRuntime();  
// do stuff  
loadWASM('main.wasm');  
```
