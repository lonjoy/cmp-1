cmp
===
晨风音乐_视频_播放器_CMP_CCHAT
<HTML>
<HEAD>
<title>CMP播放器说明</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<META name=GENERATOR content="MSHTML 8.00.6001.19190">
</HEAD>
<BODY>
<P>一，介绍</P>
<P>CMP<全称为CenFun Music Player>是一款免费的在线Flash音乐播放器，致力于提供最佳在线音乐播放解决方案。支持的音频视频格式主要有MP3,FLV,MP4,并可以通过网页JS接口实现WMP(Windows Media Player)所支持的格式播放，如wma等。主要功能特色有列表式播放(自定义音乐专辑和列表)，MP3可视化效果(声音频谱)，同步歌词（默认支持lrc歌词以及kmc卡拉ok歌词），高清视频和在线直播(h264/rtmp)，自定义皮肤，加载各种插件等等，CMP4支持api的调用，可让用户实现更多自定义功能。</P>
<P>交流论坛：http://bbs.cenfun.com &nbsp;&nbsp; http://www.meenet.cn &nbsp;&nbsp;<a href="http://cmp.meenet.cn">CMP手册</a></P>
<P>====================================================</P>
<P>二，本目录说明<BR>&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/cfplay">cfplay</a>/&nbsp;&nbsp;  CMP1版本程序目录<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/cfplay2">cfplay2</a>/&nbsp; CMP2版本程序目录<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/cmp2.1">cmp2.1</a>/&nbsp;&nbsp;&nbsp;&nbsp; CMP2.1版本程序目录【自本版本开始使用CMP简称】<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/cmp3">cmp3</a>/&nbsp;&nbsp;&nbsp;&nbsp; CMP3版本程序目录<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/cmp4">cmp4</a>/&nbsp;&nbsp;&nbsp;&nbsp; CMP4版本程序目录<BR>
&nbsp;&nbsp;&nbsp; +----/<a href="http://meenet.svn.sourceforge.net/svnroot/meenet/cmp/cmp4/plugins">plugins</a>/&nbsp;&nbsp; CMP4部分插件目录<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/cmp5">cmp5</a>/&nbsp;&nbsp;&nbsp;&nbsp; CMP5版本程序目录<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/music">music</a>/&nbsp;&nbsp;&nbsp;&nbsp; CMP测试音乐<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/meenet/cmp/tree/master/js">js</a>/&nbsp;&nbsp;&nbsp;&nbsp; CMP专用插入脚本<BR>
&nbsp;&nbsp;&nbsp; <a href="https://github.com/meenet/cmp/raw/master/Tracer.swf">Tracer.swf</a>&nbsp; CMP调试器<BR>
&nbsp;&nbsp;&nbsp; <a href="https://github.com/meenet/cmp/blob/master/TrustFiles.txt">TrustFiles.txt</a>&nbsp; 传输协议<BR>
&nbsp;&nbsp;&nbsp; <a href="https://github.com/meenet/cmp/blob/master/updatelog.txt">updatelog.txt</a> 更新日志&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;<a href="http://cmp.meenet.cn/version.htm">版本检测</a>&nbsp;&nbsp;&nbsp; <a href="http://cmp.meenet.cn/down.htm" target="_blank">最新版本压缩包</a></P>
<P>三，安装包说明【最新版本的目录，部分版本未公布或者未收集全】<BR>
&nbsp;&nbsp;&nbsp; +--/lrc/&nbsp; 歌词目录<BR>
&nbsp;&nbsp;&nbsp; +--/music/&nbsp; 测试音乐目录，仅用于环境测试，可删除<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/cenfun/cmp/tree/master/cmp4/plugins">plugins</a>/　插件存放目录<BR>
&nbsp;&nbsp;&nbsp; +--/<a href="https://github.com/cenfun/cmp/tree/master/cmp4/skins">skins</a>/&nbsp; 皮肤存放目录<BR>
&nbsp;&nbsp;&nbsp; ---/<a href="https://raw.github.com/cenfun/cmp/master/js/cmp.js">cmp.js</a>&nbsp; CMP专用插入脚本<BR>
&nbsp;&nbsp;&nbsp; ---/cmp.swf&nbsp; CMP主程序，集成默认皮肤(default.zip)<BR>
&nbsp;&nbsp;&nbsp; ---/cmpn.swf&nbsp; CMP裸版主程序，不集成默认皮肤<BR>
&nbsp;&nbsp;&nbsp; ---/<a href="http://cmp.meenet.cn/config.htm">config.xml</a>&nbsp; 全局配置文件，如不配置url参数，将默认加载此文件为配置<BR>
&nbsp;&nbsp;&nbsp; ---/<a href="http://cmp.meenet.cn/crossdomain.htm">crossdomain.xml</a>&nbsp; flash的跨域策略文件(允许本站资源被跨域调用时使用)<BR>
&nbsp;&nbsp;&nbsp; ---/<a href="http://cmp.meenet.cn/demo.htm">index.htm</a>&nbsp; CMP调用demo例子页面<BR>
&nbsp;&nbsp;&nbsp; ---/<a href="http://cmp.meenet.cn/list.htm">list.xml</a>&nbsp; 音乐列表文件，如果不配置lists参数，将默认加载此文件为列表<BR>
&nbsp;&nbsp;&nbsp; ---/logo.png&nbsp; logo图，可修改为自己的，用logo参数加载到CMP</P>
<P>其中plugins和skins目录中附送了一些常用的插件和皮肤，更多的可去官方论坛下载</P>
<P>注意，如果所有皮肤都加载错误，可能是因为空间不支持zip文件的访问，请尝试将皮肤包文件的后缀zip改为swf<BR>
同样，如果lrc歌词不能读取，也一样是空间服务器后缀类型设置不允许的问题<BR>
====================================================</P>
<P>CMP主程序cmp.swf/cmpn.swf许可协议：<BR>license: CC BY-ND<img src="http://i.creativecommons.org/l/by-nd/3.0/88x31.png">
<BR>http://creativecommons.org/licenses/by-nd/3.0/deed.zh</P>
<P>http://bbs.cenfun.com<BR>作者: 晨风 (QQ:44023478)<BR>email: cenfun@gmail.com</P>
<P>====================================================<BR>
Copyright &copy;2005   CenFun.Com<script type="text/javascript" src="http://js.meenet.cn/tongji.js"></script><noscript><a href="http://www.51.la/?5492210" target="_blank"><img alt="&#x6211;&#x8981;&#x5566;&#x514D;&#x8D39;&#x7EDF;&#x8BA1;" src="http://img.users.51.la/5492210.asp" style="border:none" /></a></noscript><BR>
====================================================</P>
</body>
</HTML>
