# Vue2 Medium Editor

Vue2 component for Medium Editor wrapper with https://github.com/yabwe/medium-editor
But all plugins are re-writing in Vue.js

## Features
- Medium like editor
- Image uploader and description
- Embed

## Usage

### Installation

```
yarn add https://github.com/tui2tone/vue2-medium-editor
```

### Usage

add to global component

```
import Vue from 'vue'
import MediumEditor from 'vue2-medium-editor'

Vue.component('medium-editor', MediumEditor)
```

usage

```
<medium-editor :content='content' :options='options' />

<script>
export default {
    data() {
        return {
            content: "",
            options: {
            }
        }
    }
}
</script>
```

### Nuxt.js Usage

create a plugins

```
import Vue from 'vue'
import MediumEditor from 'vue2-medium-editor'

Vue.component('medium-editor', MediumEditor)
```

import a plugin in nuxt.config.js with disable ssr mode

```
plugins: [
    { src: '~/plugins/medium-editor', ssr: false },
]
```

include a css file
```
css: [
    'medium-editor/dist/css/medium-editor.css',
    'medium-editor/dist/css/themes/bootstrap.css'
]
```

## Configuration



## License

MIT: https://github.com/tui2tone/vue2-medium-editor/blob/master/LICENSE