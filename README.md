# T5Player-web
百度云js播放器
使用方法：
首先推荐看演示演示：HTTP：//cyberplayer.bcelive.com/demo/new/index.html
3.3.0版本简介：
FLV和HLS视频格式的点播及直播，在支持MediaSourceExtension的浏览器中高优使用H5进行播放，以应对闪存即将下线的现状。
在其他低版本浏览器环境中，依旧自动调用闪存播放器进行播放，目前用户依旧可以通过主参数进行调度控制。

3.3.0更新日志如下：
1360浏览器展示问题优化。
2，时长展示不准确的错误修正。
3，倍速播放的一个修正错误。
如图4所示，令牌加密播放的使用升级。

几个注意点：
1，flv或hls必须支持跨域访问，即ResponseHeader中要设置Access-Control-Allow-Origin：*，不然会出错，除非设置了primary：'flash'通过flash播放器播放（并不推荐这么做） 。
2，用H5播放HLS格式视频此版本无需加载videojs文件，会自动根据系统环境来加载。
3，播放直播视频流的时候，一定要设置isLive：true。
如图4所示，在部分的Android手机环境的浏览器上，原生不支持播放HLS。

更多帮助和API请见：HTTPS：//cloud.baidu.com/doc/MCT/Web-SDK.html
