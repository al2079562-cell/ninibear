# 🐻 Ninibear 动动钟（网页版 · 个人用）

给自己和朋友的可爱健康小助手：
- ⏰ 每 25–45 分钟（可拖杆调节）提醒你起来活动，带提示音、震动、弹窗
- 💊 早 / 晚两次吃药打卡，自动记录"连续全勤天数"
- 📊 今日活动次数 / 专注次数 / 全勤天数统计
- 📴 添加到主屏幕后支持离线使用

---

## 第一步：把 app 放到网上（GitHub Pages，免费，不用写代码）

1. 打开 github.com，注册一个免费账号（只用浏览器即可）。
2. 点右上角 **+ → New repository**，仓库名随便起（比如 `ninibear`），选 **Public**，勾选 **Add a README file**，点 **Create repository**。
3. 进入仓库后，点 **Add file → Upload files**，把解压出来的 **全部 8 个文件** 一起拖进去（或全选上传），点 **Commit changes**。
4. 点仓库的 **Settings → Pages**，Source 选 **Deploy from a branch**，Branch 选 **main / (root)**，点 **Save**。
5. 等 1-2 分钟，刷新该页面，会出现你的网址，形如：
   `https://你的用户名.github.io/ninibear/`

## 第二步：在 iPhone 上"安装"这个 app

1. 用 iPhone 的 **Safari** 打开上面的网址。
2. 点底部分享按钮（方框向上箭头）→ 往下划 → **添加到主屏幕**。
3. 主屏幕上就会出现 🐻 Ninibear 图标，点开就是全屏 app 体验！

> 提醒：锁屏通知需要 **iOS 16.4 及以上**，且必须从主屏幕图标打开过一次、并允许通知。

## 第三步：换成其他 Ninibear 图（可选，已内置 3 张）

当前已内置：趴趴熊（主界面）、茶杯熊（到点提醒）、挥手熊（备用）。
想换图的话：

1. 找到你喜欢的 Ninibear 图片（PNG、透明背景最好），改名为 `ninibear.png`。
2. 在 GitHub 仓库里 **Add file → Upload files** 上传它。
3. 打开仓库里的 `index.html`，点右上角 **铅笔图标 ✏️** 编辑：
   搜索 `内置占位小熊`，把注释下面那一整段 `<svg ... </svg>` 删掉，
   换成：
   ```html
   <img src="ninibear.png" style="width:100%;height:100%;object-fit:contain;">
   ```
4. 点 **Commit changes**，手机上重新打开（或删掉主屏幕图标再添加一次）即可看到新小熊！

## 说明与限制

- 所有数据只存在你自己的手机浏览器里（localStorage），不上传任何服务器。
- iOS 系统限制：网页 app 锁屏后的通知能力不如原生 app，建议保持屏幕常亮使用体验最佳；
  通知权限在第一次点"开始"时会弹出，请选"允许"。
