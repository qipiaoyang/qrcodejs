# QRCode.js
QRCode.js is javascript library for making QRCode. QRCode.js supports Cross-browser with HTML5 Canvas and table tag in DOM.
QRCode.js has no dependencies.

Project forked by Zhiyuan Ling from KeeeX/qrcodejs, I merged the border option from https://github.com/davidshimjs/qrcodejs/pull/54/commits/ceab422d98d36fb6b8f138954745d1b4461b28cb.

## Basic Usages
```html
<div id="qrcode"></div>
<script type="text/javascript">
new QRCode(document.getElementById("qrcode"), "https://github.com/KeeeX/qrcodejs");
</script>
```

or with some options

```html
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCode(document.getElementById("qrcode"), {
	text: "https://github.com/KeeeX/qrcodejs",
	width: 128,
	height: 128,
	border: 4,
	colorDark : "#000000",
	colorLight : "#ffffff",
	correctLevel : QRCode.CorrectLevel.H
});
</script>
```

and you can use some methods

```javascript
qrcode.clear(); // clear the code.
qrcode.makeCode("https://github.com/KeeeX"); // make another code.
```

### Using with webpack

```javascript
const QRCode = require("@keeex/qrcodejs-kx");
// Use QRCode as usual
```

## Browser Compatibility
IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, ETC.

## License
MIT License
