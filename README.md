# steal-module-element
A Steal Module Element is like the Steal Module Script tag but enables Steal only once
- all steal.js attrs are working on steal-module if none is defined main defaults to @empty and is highly recommended
- default detects environment based on 
- is based on steal-element and directly extends it
- it don't autoregisters  tag via customElement.define('steal-element')

```html
<steal-module>
import ViewModel from './myView.js'
import view from './index.stache'
import stache can-stache
document.currentScript.ownerDocument.replaceChild(document.currentScript, stache('<h1>{{message}}</h1>')({message: 'Frank'}))
</steal-module>
```
