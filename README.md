# scrollingApi

'scroll-behavior'を使用せずに任意のデバイスでスクロールするためのAPI。
現在、「scroll-behavior」はiOSデバイスで使用できないので、その代わりに使います。

#### 使い方
---
●　main.js を読み込んでから、
　 [エレメント].scrollto();
　 を実行する。
#### 例
```
<!DOCTYPE html>
<html lang="en">
<head>
<script src="main.js"></script>
</head>
~~省略~~
<p id="m">ターゲット</p>
~~省略~~
<button onclick="scrollEvent()">ターゲットまでスクロール</button>
<script>
function scrollEvent() {
		document.getElementById('m').scrollto();
}
</script>
</html>
```

---
●　このスクリプトによるスクロールを中止させないようにするには、
　 第一引数をtrueにする。
  (デフォルトでは、許可されている)
[例]
```
~~省略~~
document.getElementById('m').scrollto(true);
~~省略~~
```
---
