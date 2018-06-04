---
filename: /packages/material-ui/src/TextField/TextField.js
---

<!--- This documentation is automatically generated, do not try to edit it. -->

# TextField

The `TextField` is a convenience wrapper for the most common cases (80%).
It cannot be all things to all people, otherwise the API would grow out of control.

## Advanced Configuration

It's important to understand that the text field is a simple abstraction
on top of the following components:
- [FormControl](/api/form-control)
- [InputLabel](/api/input-label)
- [Input](/api/input)
- [FormHelperText](/api/form-helper-text)

If you wish to alter the properties applied to the native input, you can do so as follows:

```jsx
const inputProps = {
  step: 300,
};

return <TextField id="time" type="time" inputProps={inputProps} />;
```

For advanced cases, please look at the source of TextField by clicking on the
"Edit this page" button above. Consider either:
- using the upper case props for passing values directly to the components
- using the underlying components directly as shown in the demos

## Props

| Name | Type | Default | Description |
|:-----|:-----|:--------|:------------|
| <span class="prop-name">autoComplete</span> | <span class="prop-type">string |   | This property helps users to fill forms faster, especially on mobile devices. The name can be confusing, as it's more like an autofill. You can learn more about it here: https://html.spec.whatwg.org/multipage/form-control-infrastructure.html#autofill |
| <span class="prop-name">autoFocus</span> | <span class="prop-type">bool |   | If `true`, the input will be focused during the first mount. |
| <span class="prop-name">defaultValue</span> | <span class="prop-type">union:&nbsp;string&nbsp;&#124;<br>&nbsp;number<br> |   | The default value of the `Input` element. |
| <span class="prop-name">disabled</span> | <span class="prop-type">bool |   | If `true`, the input will be disabled. |
| <span class="prop-name">error</span> | <span class="prop-type">bool |   | If `true`, the label will be displayed in an error state. |
| <span class="prop-name">FormHelperTextProps</span> | <span class="prop-type">object |   | Properties applied to the `FormHelperText` element. |
| <span class="prop-name">fullWidth</span> | <span class="prop-type">bool |   | If `true`, the input will take up the full width of its container. |
| <span class="prop-name">helperText</span> | <span class="prop-type">node |   | The helper text content. |
| <span class="prop-name">id</span> | <span class="prop-type">string |   | The id of the `input` element. Use that property to make `label` and `helperText` accessible for screen readers. |
| <span class="prop-name">InputLabelProps</span> | <span class="prop-type">object |   | Properties applied to the `InputLabel` element. |
| <span class="prop-name">InputProps</span> | <span class="prop-type">object |   | Properties applied to the `Input` element. |
| <span class="prop-name">inputProps</span> | <span class="prop-type">object |   | Attributes applied to the native `input` element. |
| <span class="prop-name">inputRef</span> | <span class="prop-type">func |   | Use that property to pass a ref callback to the native input component. |
| <span class="prop-name">label</span> | <span class="prop-type">node |   | The label content. |
| <span class="prop-name">margin</span> | <span class="prop-type">enum:&nbsp;'none'&nbsp;&#124;<br>&nbsp;'dense'&nbsp;&#124;<br>&nbsp;'normal'<br> |   | If `dense` or `normal`, will adjust vertical spacing of this and contained components. |
| <span class="prop-name">multiline</span> | <span class="prop-type">bool |   | If `true`, a textarea element will be rendered instead of an input. |
| <span class="prop-name">name</span> | <span class="prop-type">string |   | Name attribute of the `input` element. |
| <span class="prop-name">onChange</span> | <span class="prop-type">func |   | Callback fired when the value is changed.<br><br>**Signature:**<br>`function(event: object) => void`<br>*event:* The event source of the callback. You can pull out the new value by accessing `event.target.value`. |
| <span class="prop-name">placeholder</span> | <span class="prop-type">string |   | The short hint displayed in the input before the user enters a value. |
| <span class="prop-name">required</span> | <span class="prop-type">bool | <span class="prop-default">false</span> | If `true`, the label is displayed as required. |
| <span class="prop-name">rows</span> | <span class="prop-type">union:&nbsp;string&nbsp;&#124;<br>&nbsp;number<br> |   | Number of rows to display when multiline option is set to true. |
| <span class="prop-name">rowsMax</span> | <span class="prop-type">union:&nbsp;string&nbsp;&#124;<br>&nbsp;number<br> |   | Maximum number of rows to display when multiline option is set to true. |
| <span class="prop-name">select</span> | <span class="prop-type">bool | <span class="prop-default">false</span> | Render a `Select` element while passing the `Input` element to `Select` as `input` parameter. If this option is set you must pass the options of the select as children. |
| <span class="prop-name">SelectProps</span> | <span class="prop-type">object |   | Properties applied to the `Select` element. |
| <span class="prop-name">type</span> | <span class="prop-type">string |   | Type attribute of the `Input` element. It should be a valid HTML5 input type. |
| <span class="prop-name">value</span> | <span class="prop-type">union:&nbsp;string&nbsp;&#124;<br>&nbsp;number&nbsp;&#124;<br>&nbsp;arrayOf<br> |   | The value of the `Input` element, required for a controlled component. |

Any other properties supplied will be spread to the root element ([FormControl](/api/form-control)).

## Inheritance

The properties of the [FormControl](/api/form-control) component are also available.
You can take advantage of this behavior to [target nested components](/guides/api#spread).

## Demos

- [Autocomplete](/demos/autocomplete)
- [Pickers](/demos/pickers)
- [Text Fields](/demos/text-fields)
