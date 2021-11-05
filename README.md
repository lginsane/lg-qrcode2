# QRCode.js
QRCode.js is javascript library for making QRCode. QRCode.js supports Cross-browser with HTML5 Canvas and table tag in DOM.
QRCode.js has no dependencies.

## Basic Usages
```
<div id="qrcode"></div>
<script type="text/javascript">
new QRCode(document.getElementById("qrcode"), "http://jindo.dev.naver.com/collie");
</script>
```

or with some options

```
var qrcode = new QRCode("test", {
	text: "http://jindo.dev.naver.com/collie",
	width: 128,
	height: 128,
	colorDark : "#000000",
	colorLight : "#ffffff",
	correctLevel : QRCode.CorrectLevel.H
});
```

and you can use some methods

```
qrcode.clear(); // clear the code.
qrcode.makeCode("http://naver.com"); // make another code.
```

## 标记

完全克隆[qrcode2](https://github.com/davidshimjs/qrcodejs)

原因：处理严格模式下._admin报错问题
