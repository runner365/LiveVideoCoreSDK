# LiveVideoCoreSDK 
基于IOS的手机视频直播SDK.
============================
LiveVideoCoreSDK是基于IOS的视频直播SDK(支持IOS8.1以上,基于开源videocore进行了改进)
-----------------------------------------------------------------------------
分辨率,速率配对关系:<br/>
1, 720x1280:至少1.5mbps;<br/>
2, 540x960: 至少800kbps;<br/>
3, 360x640: 至少:600kbps;<br/>
 
如果想获取丰富的滤镜直播效果，并且免除编译整合的困难, 可以到我新的基于gpuimage的代码库:<br/>
1, 多滤镜IOS推流SDK:<br/>
基于GPUImage的多滤镜拍摄, 滤镜资源丰富. [GPUImageRtmpPush](https://github.com/runner365/GPUImageRtmpPush)<br/>
2, Android rtmp拍摄直播SDK:<br/>
Android手机软编码，手机适配能力强，支持所有市面的RTMP服务器。
[android_rtmppush_sdk](https://github.com/runner365/android_rtmppush_sdk) <br/>
<br/>
RTMP推荐开源服务器:
----------------------
推荐多媒体流媒体服务: [cpp_media_server](https://github.com/runner365/cpp_media_server)

支持跨平台(linux/mac)

### 直播相关特性
* rtmp推拉流服务(支持h264/vp8+aac/opus in rtmp/flv)
* httpflv拉流服务(支持h264/vp8+aac/opus in rtmp/flv)
* hls录像服务(支持h264/vp8+aac/opus in mpegts)
* webobs: websocket推送flv直播服务(webcodec编码，websocket flv推流封装)

### webrtc视频会议特性
* 房间管理服务
* websocket长连接接入
* 加入/离开房间
* 推流/停止推流
* 拉流/停止拉流
* 高性能webrtc转rtmp: 无转码
* 高性能支持webrtc的旁路rtmp直播
* 高性能rtmp转webrtc: 无转码
* 高性能支持低延时直播，支持rtmp转为webrtc
