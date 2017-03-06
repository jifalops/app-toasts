[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/app-toasts)

# app-toasts
A swipeable, actionable, and themable paper-toast. Four pre-themed toasts are available:
success, info, warning, and error.

## Installation
```
bower install --save app-toasts
```

## Usage
* Drop `app-toasts` in and call one of the `show()` methods.
* Or use `app-toast` directly.

## Demo
<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="app-toasts.html">
    <next-code-block></next-code-block>   
  </template>
</custom-element-demo>
```
-->

```html
<app-toasts id="toasts"></app-toasts>
<app-toasts id="toasts2" intense></app-toasts>
<label><input id="intense" type="checkbox"/>Intense coloring</label><br/><br/>
<button onclick="showSuccessToast()">Success</button>
<button onclick="showInfoToast()">Info</button>
<button onclick="showWarningToast()">Warning</button>
<button onclick="showErrorToast()">Error</button>
<button onclick="showDefaultToast()">Default</button>
<script>
  var toasts = document.getElementById('toasts');
  var toasts2 = document.getElementById('toasts2');
  var intense = document.getElementById('intense');
  function showSuccessToast() {    
    if (intense.checked) toasts2.showSuccessToast();
    else toasts.showSuccessToast();
  };
  function showInfoToast() {    
    if (intense.checked) toasts2.showInfoToast();
    else toasts.showInfoToast();
  };
  function showWarningToast() {    
    if (intense.checked) toasts2.showWarningToast();
    else toasts.showWarningToast();
  };
  function showErrorToast() {  
    if (intense.checked) toasts2.showErrorToast();
    else toasts.showErrorToast();
  };
  function showDefaultToast() {    
    if (intense.checked) toasts2.showDefaultToast();
    else toasts.showDefaultToast();
  };
</script>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/app-toasts/demo/demo/index.html)
| [github](https://jifalops.github.io/app-toasts/components/app-toasts/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/app-toasts/app-toasts)
| [github](https://jifalops.github.io/app-toasts).

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
