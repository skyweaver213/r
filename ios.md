用户问 iOS App Store 上有没有类似的"隐蔽摄像头/隐匿录像"应用在线。这需要联网搜索。用 WebSearch 工具（deferred，需要 ToolSearch 加载）。

这个问题涉及：
1. App Store 上类似隐蔽摄像/后台录像/伪装类应用的存在情况
2. 以及 Apple 审核政策对这类应用的态度（对用户后续 iOS 上架决策有参考价值）

先加载 WebSearch 工具。

There are quite a few similar apps, let me search for details on a few of the key ones ( rankings, whether they're still online, pricing ), especially the well-known ones like SP Camera and Discreet, as well as the market landscape. Also, the search results should be organized from the perspective of "requirements for porting our app to iOS".

Another search to understand the Apple review policy stance on such apps (5.2.4 or other policies), as well as the popularity of similar apps ( rankings, reviews ), to provide the user with a complete analysis.

两次搜索结果足够回答用户问题了。总结 iOS 生态状况：

**iOS App Store 上确实有大量同类应用在线**（说明这类应用能过审且能存活）：

1. **SCamera Pro**（id1613327007）——功能几乎和我们的 Veil Camera 一样：下滑隐藏相机、黑色背景模拟关机、虚假背景伪装、点屏拍摄
2. **Secret video recorder - NoCam**（id6743176516）——"completely black recording screen"，完全黑屏录像，4.4 分
3. **Discreet - Black Screen Camera**（id1600729989）——老牌，黑屏+自定义屏幕模式，支持 Apple Watch 控制、4K、连拍
4. **Screet - Black Screen Camera**（id6758235938）——黑屏相机+隐蔽录像，强调会议/讲座/安全记录等正当用途
5. **SP Camera**（id603037910）——最著名的一个，存在多年：假背景（浏览网页/时钟）掩护下录像，甚至有运动检测自动录，支持 Apple Watch

关键洞察：
- 这类 app 在 iOS 上不仅有，而且活得很好（SP Camera 多年在线、Discreet 自称"original top-rated"）
- 共同过审策略：
  a. 强调正当用途（个人记录、安全取证、会议记录——Screet 的描述写得很清楚"with permission"）
  b. "隐蔽"包装成"不打扰"（black screen = 不发光不干扰，discreet = 不引起注意），而非"偷拍"
  c. Apple 政策的关键点：2.3.1（隐藏功能）——不能有对审核员隐藏的功能；5.1.1 隐私。审核时 app 功能要如实展示（我们的新手引导反而有利——明示所有功能）
- 差异点：iOS 系统限制（无后台持续录像、相机指示灯绿点会亮），所以 iOS 版都是"前台黑屏"方案，与我们 Android 前台蒙层方案一致

对用户的意义：iOS 上架可行，市场已验证；需注意 Apple 用词审核（避免 "spy/secret/stealth" 过度），强调 privacy-first 定位。

回复要点：确认有、列代表应用、说明它们怎么过审、对我们 iOS 版的启示。附 Sources（两次搜索的相关链接）。
有的，而且不少。iOS App Store 上这类“隐蔽拍摄”应用长期在线，市场已被充分验证：

## 代表应用

| 应用 | 特点 |
|---|---|
| **SP Camera**（存在多年，最有名） | 假背景掩护录像（伪装成网页浏览/**时钟**/静态图）、运动检测自动录、Apple Watch 遥控 |
| **Discreet - Black Screen Camera** | 自称“原创最高评分”，黑屏/自定义屏幕模式、4K、连拍、Apple Watch 控制 |
| **SCamera Pro** | 与 Veil Camera 功能几乎重合：黑屏模拟关机、滑动隐藏相机、假背景、点屏拍摄 |
| **NoCam - Secret video recorder** | 纯黑屏录像，4.4 分 |
| **Screet - Black Screen Camera** | 黑屏相机，描述强调会议/讲座（*经许可*）、个人安全取证等正当场景 |

## 它们为什么能过审（对我们 iOS 版的启示）

1. **措辞包装**：不叫“偷拍”，叫 "discreet"（低调）、"black screen"（不发光不打扰）。Screet 甚至在描述里主动写 "with permission"（经许可使用）
2. **正当用途定位**：个人记录、演讲彩排、运动拍摄、安全取证——和我们完整说明里的 PERFECT FOR 章节一致
3. **无隐藏功能**：Apple 2.3.1 要求所有功能对审核员透明——我们的新手引导 + 隐私政策反而是加分项
4. **iOS 系统限制**：无真后台录像、录像时状态栏绿点亮起，所以 iOS 同类全是“前台黑屏”方案，恰好与我们现有架构一致

结论：iOS 上架可行且有对标；Veil Camera 的“时钟伪装 + 数据全本地”在同类中定位更干净（多数竞品有订阅/IAP，我们隐私口径更严）。上架时措辞注意用 *discreet/privacy* 而非 *spy/secret* 即可。

Sources:
- [SCamera Pro - App Store](https://apps.apple.com/cn/app/scamera-pro/id1613327007)
- [Secret video recorder - NoCam - App Store](https://apps.apple.com/us/app/secret-video-recorder-nocam/id6743176516)
- [Discreet - Black Screen Camera - App Store](https://apps.apple.com/lr/app/discreet-black-screen-camera/id1600729989)
- [Screet - Black Screen Camera - App Store](https://apps.apple.com/iq/app/screet-black-screen-camera/id6758235938)
- [SP Camera - App Store](https://apps.apple.com/us/app/sp-camera/id603037910)
- [App Review Guidelines - Apple Developer](https://developer.apple.com/app-store/review/guidelines/#5)