# weibo-img-crypto
自动加密解密微博上传的图片

## 如何使用
在浏览器地址栏输入以下代码，上传图片时就会自动加密，在图片上点击鼠标右键就会自动解密。注意前面的 "`javascript:`" 必须手动输入，不能复制粘贴，否则会被浏览器自动去掉

```javascript
javascript:fetch('https://raw.githubusercontent.com/xfgryujk/weibo-img-crypto/master/weibo-img-crypto.js').then(res => res.text(), e => alert('载入失败：' + e)).then(res => {let script = document.createElement('script'); script.innerHTML = res; document.body.appendChild(script)})
```

也可以按 `Ctrl + Shift + J` 打开控制台，在控制台输入。也可以将这些代码作为网址添加到书签/收藏夹，能更快使用

目前不支持 GIF 图，以后可能支持

只在 Chrome、Edge 浏览器测试过，不保证支持其他浏览器<del>（IE 是什么？我可不知道）</del>

## 效果
加密后：

![加密后](https://github.com/xfgryujk/weibo-img-crypto/blob/master/encrypted.jpg)

解密后：

![解密后](https://github.com/xfgryujk/weibo-img-crypto/blob/master/decrypted.png)

原图：

![原图](https://github.com/xfgryujk/weibo-img-crypto/blob/master/origin.jpg)
