腾讯云视立方·短视频 SDK ，是音视频终端 SDK（腾讯云视立方）的子产品 SDK 之一，基于腾讯云强大的上传、存储、转码、分发的云点播能力，提供集成了采集、剪辑、拼接、特效、分享、播放等功能的客户端 SDK，并整合腾讯的 IM、视频内容识别等技术，帮助用户聚焦业务本身，快速轻松实现基于移动端的短视频应用。更多关于短视频 SDK 的文档详情请参见 [短视频 SDK ](https://cloud.tencent.com/document/product/584)。

音视频终端 SDK（腾讯云视立方）结构示意如下图：

![](https://qcloudimg.tencent-cloud.cn/raw/fb9148de43ab9f833a69d88d9e958d35.jpg)

## 短视频 SDK 功能列表

<table>
<thead>
<tr>
<th>功能模块</th>
<th>功能项</th>
<th>功能简介</th>
</tr>
</thead>
<tbody><tr>
<td>界面</td>
<td>自定义 UI</td>
<td>开发者自定义 UI。小视频 App 提供了一套完整的 UI 交互源码，可复用或自定义。</td>
</tr>
<tr>
<td rowspan=14>采集拍摄</td>
<td>屏比</td>
<td>支持16:9，4:3，1:1多种屏比拍摄。</td>
</tr>
<tr>
<td>清晰度</td>
<td>支持标清、高清、超清拍摄，支持自定义码率、帧率、gop。</td>
</tr>
<tr>
<td>拍摄控制</td>
<td>拍摄前后摄像头切换、灯光的控制。</td>
</tr>
<tr>
<td>时长设置</td>
<td>自定义拍摄的最短和最长时长。</td>
</tr>
<tr>
<td>水印</td>
<td>拍摄支持添加水印。</td>
</tr>
<tr>
<td>焦距</td>
<td>拍摄支持调节焦距。</td>
</tr>
<tr>
<td>对焦模式</td>
<td>支持手动对焦和自动对焦。</td>
</tr>
<tr>
<td>分段录制</td>
<td>拍摄过程中可以暂停分段并且可以回删。</td>
</tr>
<tr>
<td>拍照</td>
<td>支持拍摄照片。</td>
</tr>
<tr>
<td>变速录制</td>
<td>拍摄时支持慢速和快速录制。</td>
</tr>
<tr>
<td>背景音乐</td>
<td>拍摄前可以选择本地的 MP3 作为背景音。</td>
</tr>
<tr>
<td>变声和混响</td>
<td>拍摄前对录制的声音变声（如萝莉、大叔）和混响效果（如 KTV、会堂）。</td>
</tr>
<tr>
<td>滤镜</td>
<td>支持实时预览滑动切换滤镜的效果，支持自定义滤镜及设置滤镜程度。</td>
</tr>
<tr>
<td>基础美颜</td>
<td>拍摄设置人脸的磨皮、美白、红润，并调节强度。</td>
</tr>
<tr>
<td rowspan=12>特效编辑</td>
<td>快速导入</td>
<td>Android 支持快速导入视频。</td>
</tr>
<tr>
<td>视频裁剪</td>
<td>按照给定的时间范围精确裁剪视频。</td>
</tr>
<tr>
<td>码率设置</td>
<td>可以指定码率生成视频。</td>
</tr>
<tr>
<td>获取封面</td>
<td>根据时间获取帧图像。</td>
</tr>
<tr>
<td>按帧预览</td>
<td>移动时间线时，在预览窗口显示基准游标停留的帧图像。</td>
</tr>
<tr>
<td>滤镜</td>
<td>给视频添加滤镜，并支持设置滤镜的强度。</td>
</tr>
<tr>
<td>时间特效</td>
<td>给视频添加倒放、反复、慢动作的时间特效。</td>
</tr>
<tr>
<td>滤镜特效</td>
<td>给视频添加灵魂出窍、动感光波、分裂、幻影等特效。</td>
</tr>
<tr>
<td>背景音乐</td>
<td>选择自带声音文件或用户手机本地的 MP3 作为背景音，支持背景音乐的裁剪和设置音量大小。</td>
</tr>
<tr>
<td>动态或者静态贴纸</td>
<td>添加动态或者静态贴纸，支持设置在视频画面中显示位置和起始时间。</td>
</tr>
<tr>
<td>字幕</td>
<td>添加字幕，可以选择字幕边框背景的样式，例如气泡等，支持设置在视频画面中显示位置和起始时间。</td>
</tr>
<tr>
<td>图片转场</td>
<td>导入多张图片，并选择旋转、淡入淡出等转场效果，并生成视频。</td>
</tr>
<tr>
<td rowspan=2>视频拼接</td>
<td>多视频拼接</td>
<td>支持多视频前后拼接。</td>
</tr>
<tr>
<td>跟拍</td>
<td>支持根据播放的视频进行跟拍，生成双画面视频。</td>
</tr>
<tr>
<td>视频上传</td>
<td>上传到云点播</td>
<td>云点播支持媒资管理、内容审核等功能。</td>
</tr>
<tr>
<td>点播播放</td>
<td>超级播放器</td>
<td>基于点播播放器实现的集视频信息拉取、横竖屏切换、清晰度选择、弹幕、直播时移等功能于一体的解决方案，且完全开源。</td>
</tr>
</tbody></table>

## 短视频 License 介绍

### 短视频 SDK 精简版 License

您可以登录 [云点播控制台](https://console.cloud.tencent.com/vod/license) 在线申请为期一个月的短视频 SDK 基础版试用 License，该 License 可以在短视频 SDK 上使用。

购买云点播流量资源包-10TB，可以获取为期一年的短视频 SDK 精简版 License 使用权限。云点播资源包请参见 [资源包（预付费）](https://cloud.tencent.com/document/product/266/14667)，购买成功后，登录 [云点播控制台](https://console.cloud.tencent.com/vod/license) 获取短视频 SDK 精简版 License。

### 短视频 SDK 基础版 License

购买云点播流量资源包-50TB、流量资源包-200TB、流量资源包-1PB，可以获取为期一年的短视频 SDK 基础版 License 使用权限。云点播资源包请参见 [资源包（预付费）](https://cloud.tencent.com/document/product/266/14667)，购买成功后，登录 [云点播控制台](https://console.cloud.tencent.com/vod/license) 获取短视频 SDK 基础版 License。
