# Windows 下 Shadowsocks 設置方法

## 1、下載客戶端

推薦您使用最新版本的客戶端，點擊[這裏](https://github.com/shadowsocks/shadowsocks-windows/releases)下載最新的客戶端

![Markdown](http://i1.bvimg.com/629647/cc8dcd2d79849d64.png)

## 2、安裝 .NET Framework

一般 Windows 10 已經自帶，不需要額外安裝，如果您的系統版本略舊，請在[這裏](https://www.microsoft.com/zh-tw/download/details.aspx?id=53345)下載適用於 Windows 7 SP1、Windows 8.1、Windows Server 2008 R2 SP1、Windows Server 2012 及 Windows Server 2012 R2 的 Microsoft .NET Framework 4.6.2 (Web 安裝程式)

## 3、解壓 Shadowsocks 客戶端

閣下完成下載後，可以在熟悉的位置創建一個便於找到的文件夾，在本文中我們嘗試在桌面新建名為 `Shadowsocks` 的文件夾，之後請打開下載的 Shadowsocks 客戶端文件 請選中其中`Shadowsocks.exe`文件拖動至剛剛新建的 Shadowsocks 文件夾，並雙擊運行 `Shadowsocks.exe`

![](https://ooo.0o0.ooo/2017/05/22/5922f811318ad.png)

## 4、配置 Shadowsocks

在您右下方狀態欄 Shadowsocks 圖標右鍵-服務器

![Markdown](http://i2.bvimg.com/629647/beb7b35c4ab7c6eb.png)

填写配置信息即可，信息会在群里公布

![Markdown](http://i2.bvimg.com/629647/ccd00fcae7f2e00f.png)

## 5、配置系統代理

右擊您右下方狀態欄的 Shadowsocks 圖標，勾選 啟用系統代理 並選擇 Pac 模式,上google一下，能上，就说明你已经完成配置，恭喜你，同学，可以享受自由了。

![](https://ooo.0o0.ooo/2017/05/22/5922fe379b134.png)



注意事項:

1. 負載均衡模式高可用模式與在於分散流量和提高可用性上，對於速度的提升沒有幫助，如果對某一節點的連接質量較佳，推薦直接選中該服務器
2. 推薦使用 `PAC模式`，該模式可以實現自動代理，及沒被屏蔽的網站的流量不會經過代理。但是在 `Shadowsocks Win 2.x` 版本中因內置的 GFWList 鏈接已失效，導致 PAC 規則無法更新，您可以從選擇從本站下載 PAC 文件，或者遇到無法代理的網站時，通過編輯本地 PAC 文件，自己添加規則不包含但自己所需要代理的網站
3. `全局模式`表示基本上電腦內所有的流量都會經過代理，不推薦日常使用，因為很容易導致您的國內網站的流量以及迅雷等下載網站流量經過代理造成我們收到 ISP 投訴的嚴重后果

