## 基本用法

```
<div id="qrcode"></div>
<script type="text/javascript">
new QRCode(document.getElementById("qrcode"), "http://jindo.dev.naver.com/collie");
</script>
```

或者使用一些可选参数设置：

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

同样我们可以使用以下方法：

```
qrcode.clear(); // 清除代码
qrcode.makeCode("http://naver.com"); // 生成另外一个二维码
```

## 标记

完全克隆[qrcode2](https://github.com/davidshimjs/qrcodejs)

原因：处理严格模式下._admin报错问题
