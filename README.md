[![Published on Vaadin  Directory](https://img.shields.io/badge/Vaadin%20Directory-published-00b4f0.svg)](https://vaadin.com/directory/component/jifalopsapp-toasts)
[![Stars on vaadin.com/directory](https://img.shields.io/vaadin-directory/star/jifalopsapp-toasts.svg)](https://vaadin.com/directory/component/jifalopsapp-toasts)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/app-toasts)

# app-toasts
Success, error, info, and warning theme presets for app-toast.

## Installation
```
bower i -S app-toasts      # Polymer 2.0 hybrid (1.x compatible)
bower i -S app-toasts#0.3  # Polymer 1.x based
```

## Usage
* Drop `app-toasts` in and call one of the `show()` methods.
* Or use [app-toast](https://www.webcomponents.org/element/jifalops/app-toast)
  directly.

## Demo
<!--
```
<custom-element-demo height="300">
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="app-toasts.html">
    <next-code-block></next-code-block>
    <script>
      var toasts = document.getElementById('toasts');
      var toasts2 = document.getElementById('toasts2');
      var intense = document.getElementById('intense');
      var text = document.getElementById('text');
      var duration = document.getElementById('duration');
      var actionText = document.getElementById('actionText');
      var showCancel = document.getElementById('showCancel');
      var disableSwipe = document.getElementById('disableSwipe');
      var fitBottom = document.getElementById('fitBottom');
      var feedback = document.getElementById('feedback');
      function showSuccessToast() {
        if (intense.checked) toasts2.showSuccessToast(text.value, _makeProperties());
        else toasts.showSuccessToast(text.value, _makeProperties());
      }
      function showInfoToast() {
        if (intense.checked) toasts2.showInfoToast(text.value, _makeProperties());
        else toasts.showInfoToast(text.value, _makeProperties());
      }
      function showWarningToast() {
        if (intense.checked) toasts2.showWarningToast(text.value, _makeProperties());
        else toasts.showWarningToast(text.value, _makeProperties());
      }
      function showErrorToast() {
        if (intense.checked) toasts2.showErrorToast(text.value, _makeProperties());
        else toasts.showErrorToast(text.value, _makeProperties());
      }
      function showDefaultToast() {
        if (intense.checked) toasts2.showDefaultToast(text.value, _makeProperties());
        else toasts.showDefaultToast(text.value, _makeProperties());
      }
      function _makeProperties() {
        return {
          duration: Number(duration.value),
          actionText: actionText.value,
          showCancel: showCancel.checked,
          disableSwipe: disableSwipe.checked,
          fitBottom: fitBottom.checked,
          onAction: function() { feedback.innerText = "onAction()"; },
          onCancel: function() { feedback.innerText = "onCancel()"; }
        };
      }
      function closeToast() {
        toasts.close();
        toasts2.close();
      }
    </script>
  </template>
</custom-element-demo>
```
-->

```html
<app-toasts id="toasts"></app-toasts>
<app-toasts id="toasts2" intense></app-toasts>
<input id="text" placeholder="text" value="text"/><br/>
<input id="duration" placeholder="duration (ms)" value="3000"/><br/>
<input id="actionText" placeholder="action button text" value="action"/><br/>
<label><input id="showCancel" type="checkbox"/>Show cancel</label><br/>
<label><input id="disableSwipe" type="checkbox"/>Disable swipe</label><br/>
<label><input id="fitBottom" type="checkbox"/>Fit to bottom</label><br/>
<label><input id="intense" type="checkbox"/>Intense coloring</label><br/><br/>
<button onclick="showSuccessToast()">Success</button>
<button onclick="showInfoToast()">Info</button>
<button onclick="showWarningToast()">Warning</button>
<button onclick="showErrorToast()">Error</button>
<button onclick="showDefaultToast()">Default</button>
<button onclick="closeToast()">Close</button><br/>
Last Event: <span id="feedback"></span>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/app-toasts/demo/demo/index.html)
| [github](https://jifalops.github.io/app-toasts/components/app-toasts/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/app-toasts/app-toasts)

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
