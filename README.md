# vue-lupus-paragraph-link
Vue paragraph link component.



## Install

via npm:
`npm install https://github.com/drunomics/vue-lupus-paragraph-link.git`


import it:

```
import PgLink from 'vue-lupus-paragraph-link';

Vue.component('pg-link', PgLink);
```

## Slots
You can use the following slots

- `title` ( optional )
  A title.
- `link` ( default )
  The link

## Example
```
<pg-link>
  <h3 slot="title">The title value</h3>
  <a href="#the-url" slot="link">The link label</a>
</pg-link>
```
