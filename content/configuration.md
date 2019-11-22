# Configuration

In the following example, the `value` property is used in the configuration object to specify the default image value.

```ts
import { Uppload } from "uppload";

const uploader = new Uppload({
  value: "https://example.com/image.jpg"
});
```

The keys you can use in the configuration object are:

| Key | Type | Description |
| --- | ---- | ----------- |
| `value` | String | Default/current image URL |
| `bind` | *Elements* | Set value of these elements |
| `call` | *Elements* | Clicking on these elements should open modal |
| `defaultService` | String | Default service to open widget on |
| `lang` | Object | [Language pack](/i18n) |
| `uploader` | Function | Function to [upload files](/uploaders) |
| `inline` | Boolean | Show widget inline instead of modal |
| `customClass` | String | Adds an additional class to the container |

\*The *Elements* type can be any of the following:

- String (e.g., a query selector like `".image"`)
- String[] (e.g., a query selector array like `[".image", ".img"]`)
- Element (e.g., a DOM element like `document.getElementById("img")`)
- Element[] (e.g., a DOM element array like `[document.createElement("div")]`)
- An array consisting Strings and Elements