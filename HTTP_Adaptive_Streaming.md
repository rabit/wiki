# Adaptive HTTP Streaming

## 現況

HTML5 Video

1. http://html5video.org/wiki/HTML5_Video_Wiki
2. http://www.longtailvideo.com/html5/
3. http://stackoverflow.com/questions/1735933/streaming-via-rtsp-or-rtp-in-html5

HTTP Adaptive Streaming 簡介

![HTTP Adaptive Streaming](http://image.slidesharecdn.com/dashinflash-121101132505-phpapp01/95/slide-6-1024.jpg?1351794742)

1. [黃瓜切片: HTTP Live Streaming 原理簡介](http://blog.nkbit.com/2011/11/http-live-streaming.html)
2. [HTTP Live Streaming: A Review of Apple's new streaming specification](http://issuu.com/andruby/docs/http_live_streaming_presentatino)

舊有方案

* Apple: HTTP Live Streaming
* MS: IIS Smooth Streaming
* Adobe: Dynamic Streaming
* OPEN IPTVForum: HTTP Adaptive Streaming
* 3GPP: Adaptive HTTP Streaming

![Adaptive HTTP Streaming的演進](http://image.slidesharecdn.com/webmontag-dash-110503041342-phpapp01/95/slide-6-728.jpg?1304414085)

國際標準

* [ISO MPEG Dynamic Adaptive Streaming over HTTP 的相關標準]   
   [The lastest MPEG-DASH specification \(ISO/IEC DIS 23009-1:2\)](http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=57623)   
   [The ISO Base Media File Format specification \(ISO/IEC 14496-12\)](http://www.iso.org/iso/catalogue_detail?csnumber=51533)   
   [The Common Encryption specification \(ISO.IEC 23001-7\)](http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=60398)
* IETF: HTTP Live Streaming [草案][draft-pantos-http-live-streaming]

相關文章

1. [浅谈HTTP Adaptive Streaming技术及其前景](http://blog.sina.com.cn/s/blog_4db1790b0100srlv.html)
2. [后Flash时代HTML视频的考验和磨难](http://www.webapptrend.com/2011/12/746.html)
3. [HTML5 and Video Streaming](http://techblog.netflix.com/2010/12/html5-and-video-streaming.html)
4. [Adaptive HTTP Streaming Standardization ](http://www.w3.org/2010/11/web-and-tv/slides/microsoft-john-simmons.pdf)
5. [Video Delivery in HTTP](http://www.roman10.net/video-delivery-in-http)

## ISO標準: MPEG DASH

Overview

[維基百科的介紹](http://en.wikipedia.org/wiki/Dynamic_Adaptive_Streaming_over_HTTP)   
[Overview of MPEG-DASH Standard](http://dashpg.com/?page_id=25)

![DASH的架構](http://dashif.org/w/2011/11/MPEG-DASHScope.png)   
![DASH Data Model](http://image.slidesharecdn.com/webmontag-dash-110503041342-phpapp01/95/slide-10-728.jpg?1304414085)   
![DASH Segment Indexing](http://image.slidesharecdn.com/webmontag-dash-110503041342-phpapp01/95/slide-14-728.jpg?1304414085)   

MPEG DASH的推廣組織 http://dashif.org, 其中的成員有: Microsoft, Adobe, ... 等等   
但是 Apple 不在推廣小組中, 它有自己的[標準][draft-pantos-http-live-streaming]

相關文章

1. http://www.w3.org/2011/09/webtv/slides/W3C-Workshop.pdf
2. http://dashpg.com/documents/DASHPG-MPEG-DASH-Overview.pdf
3. [MPEG DASH: The File Format of the Future?](http://www.streamingmedia.com/Articles/ReadArticle.aspx?ArticleID=78835)
4. [Dynamic Adaptive Streaming over HTTP – Design Principles and Standards](http://web.cs.wpi.edu/~claypool/mmsys-2011/Day2-1_3GPPPDynamic.pdf)
5. http://www.streamingmedia.com/Articles/ReadArticle.aspx?ArticleID=79041
6. http://mpeg.chiariglione.org/working_documents/mpeg-dash/MPEG-DASH-Tutorial.pdf
7. http://www.cash.idv.tw/wordpress/?p=6588
8. http://blog.sina.com.cn/s/blog_4db1790b0100srlv.html
9. http://www.hhi.fraunhofer.de/fields-of-competence/image-processing/research-groups/multimedia-communications/advanced-mpeg-dash.html
10. https://cs.uwaterloo.ca/~brecht/courses/854/readings/mpeg-dash-standard-ieee-mm-2011.pdf

簡報

1. http://www.slideshare.net/christian.timmerer/dynamic-adaptive-streaming-over-http-dash
2. http://www.slideshare.net/christian.timmerer/http-streaming-of-mpeg-media
3. http://www.slideshare.net/cconcolato/live-streaming-of-video-and-subtitles-with-mpegdash
4. http://www.slideshare.net/schellkenig/dash-at-the-acm-multimedia-2011
5. http://www.slideshare.net/christian.timmerer/an-evaluation-of-dynamic-adaptive-streaming-over-http-in-vehicular-environments
6. http://www.slideshare.net/christian.timmerer/a-seamless-web-integration-of-adaptive-http-streaming

### 各種瀏覽器對MPEG DASH的支援狀況

1. Google Chrome 

   Chrome plans to support DASH by using javascript library and MediaSource API \[[chrome-dash][]\]

   [chrome-dash]: http://code.google.com/p/chromium/issues/detail?id=109652 
   "Chrome Support MPEG-DASH"

   [MPEG-DASH support in Google Chrome](http://gpac.wp.mines-telecom.fr/2012/08/23/mpeg-dash-support-in-google-chrome)   
   [ASH-JS – A JavaScript- and WebM-based DASH library for Google Chrome](http://www-itec.uni-klu.ac.at/dash/?page_id=746)

2. Opera
 
   [Opera use Javascript extension and Opera Device SDK to support for DASH](http://media.opera.com/media/b2b/tv/201201/Opera_Media_Streaming.pdf)

3. Mozilla Firefox

   Mozilla firefox only plan to support DASH (WebM)   
   [Mozilla adds DASH support (WebM) based on libdash](http://www-itec.uni-klu.ac.at/dash/?p=833)   
   https://wiki.mozilla.org/Platform/Roadmap   
   相關討論 \[[mozilla-bug702122][]\] \[[mozilla-bug734546][]\]
   
   [mozilla-bug702122]: https://bugzilla.mozilla.org/show_bug.cgi?id=702122
   [mozilla-bug734546]: https://bugzilla.mozilla.org/show_bug.cgi?id=734546

4. Others

   **vlc**   
   http://www-itec.uni-klu.ac.at/dash/?p=243   

   **MP4Box**   
   http://gpac.wp.mines-telecom.fr/mp4box/dash/

   **gstreamer**   
   https://bugzilla.gnome.org/show_bug.cgi?id=675625

   **WebM adaptive streaming**   
   https://groups.google.com/a/webmproject.org/group/webm-discuss/browse_thread/thread/7d2d1faeb2832b94   
   [Instructions to Playback a WebM DASH Presentation](https://sites.google.com/a/webmproject.org/wiki/adaptive-streaming/instructions-to-playback-a-webm-dash-presentation)

### HTML5 與MPEG DASH相關的標準

MediaSource Extensions API

1. http://updates.html5rocks.com/2011/11/Stream-video-using-the-MediaSource-API
2. http://html5-demos.appspot.com/static/media-source.html
3. https://dvcs.w3.org/hg/html-media/raw-file/tip/media-source/media-source.html
4. http://html5-mediasource-api.googlecode.com/svn/tags/0.4/draft-spec/mediasource-draft-spec.html
5. http://stackoverflow.com/questions/9316859/mediasource-api-and-mp4
6. http://yt-dash-mse-test.commondatastorage.googleapis.com/unit-tests/links.html
7. http://www.ioncannon.net/utilities/1515/segmenting-webm-video-and-the-mediasource-api/

WebSocket + getUserMedia API 

1. http://rosario.github.com/2012/06/04/html5-video-streaming-over-websockets-using-pusher.html
2. http://timtaubert.de/blog/2012/10/building-a-live-green-screen-with-getusermedia-and-mediastreams/
3. http://creativejs.com/2012/03/getting-started-with-getusermedia/
4. https://github.com/ebidel/html5can/tree/master/demos/audio_streamer

### MPEG DASH 支援 即時轉播

MPD 的格式為 Dynamic 是指 MPD 中的 Segment URL 會依據 SegmentTemplate 指定的規則變化, 而 MPEG DASH Profle 為 Live( 正式
名稱為 urn : mpeg : dash : profile : isoff-live : 2011 表示
其封裝的格式為 ISO BMFF Live, 參考[範例](http://download.tsi.telecom-paristech.fr/gpac/DASH_CONFORMANCE/TelecomParisTech/mp4-live/mp4-live-mpd-V-NBS.mpd)

1. [First Live MPEG-DASH Large Scale Demonstration](http://dashif.org/first-live-mpeg-dash-large-scale-demonstration-2/) 使用 DASH Profile: Live
2. GPAC 的 MP4Box 支援問題:   
   DASH Live Profile \[[dash-profile-live][]\]   
   MPD Type 為 Dynamic \[[dash-mpd-dynamic][]\]

[dash-profile-live]: http://sourceforge.net/projects/gpac/forums/forum/327349/topic/5116440
"MPEG Dash: Adding support for MPD.Location"

[dash-mpd-dynamic]: http://sourceforge.net/projects/gpac/forums/forum/327349/topic/5439022
"Osmo4 support of dynamic Dash MPD?"

### MPEG DASH DEMO

1. http://dash-mse-test.appspot.com/
2. http://www-itec.uni-klu.ac.at/dash/?page_id=1097
3. http://lists.w3.org/Archives/Public/public-web-and-tv/2012May/0014.html
4. http://wiki.webmproject.org/adaptive-streaming/instructions-to-playback-a-webm-dash-presentation
5. GPAC 提供的各種 MPEG DASH Sequences [http://gpac.wp.mines-telecom.fr/2012/02/23/dash-sequences/](http://gpac.wp.mines-telecom.fr/2012/02/23/dash-sequences/)

### 相關工具

MPEG DASH 推廣組織提供的[工具](http://dashif.org/demos/)

1. [libdash](http://www.bitmovin.net/libdash/), [簡介投影片](http://www.slideshare.net/schellkenig/libdash-20)
2. [DASH-JS](http://www-itec.uni-klu.ac.at/dash/?page_id=746)
3. [MPD Validator](http://www-itec.uni-klu.ac.at/dash/?page_id=605)
4. [DASHEncoder](http://www-itec.uni-klu.ac.at/dash/?page_id=282)
5. [MP4BOX](http://gpac.wp.mines-telecom.fr/player/features/dash/)

### MPEG DASH for H.264 

[Guidelines for Implementation: DASH264 Interoperability Points](http://dashif.org/guidelines/DASH264-base-v09.pdf)

### 相關論文

1. [A Dynamic Adaptive HTTP Streaming Video Service for Google Android](http://web.it.kth.se/~maguire/DEGREE-PROJECT-REPORTS/111006-Luciano-Rubio-with-cover.pdf), [html version](http://dat.etsit.upm.es/~luciano/en/thesis)
2. [Dynamic adaptive streaming over HTTP --: standards and design principles]( http://dl.acm.org/citation.cfm?id=1943572)
3. [A VLC media player plugin enabling dynamic adaptive streaming over HTTP](http://dl.acm.org/citation.cfm?id=2072429)
4. [A Test Bed for DASH over Featuring Session Mobility](http://www-itec.uni-klu.ac.at/bib/files/mueller_A_Test_Bed_for_DASH_featuring_Session_Mobility.pdf)
5. [Usages of DASH for rich media services](http://dl.acm.org/citation.cfm?id=1943587)
6. [Dynamic adaptive HTTP streaming of live content](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5986186&tag=1)
7. [The MPEG-DASH Standard for Multimedia Streaming Over the Internet](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6077864)
8. [QDASH: A QoE-aware DASH system](http://polyu.academia.edu/RickyKPMok/Papers/1161278/QDASH_A_QoE-aware_DASH_system)


## IETF標準: HTTP Live Streaming

[標準草案][draft-pantos-http-live-streaming]

1. http://en.wikipedia.org/wiki/HTTP_Live_Streaming
2. http://www.php-oa.com/2010/12/10/http-live-streaming-hls.html

## Others

1. http://multimediacommunication.blogspot.tw/2010/05/http-streaming-of-mpeg-media.html
2. http://sourceforge.net/apps/trac/matroska/wiki/DASH_Profile
3. [透過CDN的方式來散佈MPEG DASH](http://www.slideshare.net/christian.timmerer/distributed-dash-dataset)
4. http://sourceforge.net/apps/mediawiki/osmf.adobe/index.php?title=Customizing_HTTP_Dynamic_Streaming
5. http://en.wikipedia.org/wiki/Helix_Universal_Server
6. https://github.com/DDVTECH/mistlib
7. http://www.html5rocks.com/en/tutorials/webgl/typed_arrays/?redirect_from_locale=pt

[draft-pantos-http-live-streaming]: http://tools.ietf.org/html/draft-pantos-http-live-streaming
"HTTP Live Streaming"
