I'm working with external JSON files imported with iron-ajax with the following format:

```json
  "url" : {
    "code" : "https://github.com/caraya/polymer-playground",
    "other" : "",
    "writeup" : ""
  }
```

Now I want to use Polymer conditional binding to only display the content of the url.* element if it has a content.  Is this legal?

```html
<template is="dom-if" if="{{url.code}}">
  <p>The content of url.code goes here</p>
</template>
```
