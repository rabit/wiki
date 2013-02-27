# Adaptive HTTP Streaming

## 現況

HTML5 Video

1. http://html5video.org/wiki/HTML5_Video_Wiki
2. http://www.longtailvideo.com/html5/
3. http://stackoverflow.com/questions/1735933/streaming-via-rtsp-or-rtp-in-html5

Adaptive HTTP Streaming

[簡介](http://blog.nkbit.com/2011/11/http-live-streaming.html)

現有方案

* Apple: HTTP Live Streaming
* MS: IIS Smooth Streaming
* Adobe: Dynamic Streaming
* OPEN IPTVForum: HTTP Adaptive Streaming
* 3GPP: Adaptive HTTP Streaming

未來標準草案

* [ISO: Dynamic Adaptive Streaming over HTTP](http://web.cs.wpi.edu/~claypool/mmsys-2011/Day2-1_3GPPPDynamic.pdf)
* [IETF: Apple HTTP Live Streaming](http://tools.ietf.org/html/draft-pantos-http-live-streaming-07)

相關文章

1. [浅谈HTTP Adaptive Streaming技术及其前景](http://blog.sina.com.cn/s/blog_4db1790b0100srlv.html)
2. [后Flash时代HTML视频的考验和磨难](http://www.webapptrend.com/2011/12/746.html)
3. [HTML5 and Video Streaming](http://techblog.netflix.com/2010/12/html5-and-video-streaming.html)
4. [Adaptive HTTP Streaming Standardization ](http://www.w3.org/2010/11/web-and-tv/slides/microsoft-john-simmons.pdf)
5. [Video Delivery in HTTP](http://www.roman10.net/video-delivery-in-http)

## MPEG DASH

Overview

1. http://www.w3.org/2011/09/webtv/slides/W3C-Workshop.pdf
2. http://dashpg.com/documents/DASHPG-MPEG-DASH-Overview.pdf
3. [MPEG DASH: The File Format of the Future?](http://www.streamingmedia.com/Articles/ReadArticle.aspx?ArticleID=78835)

推廣小組: http://dashpg.com, 成員: Microsoft, Adobe, ... 等等   
但是 Apple 不在推廣小組中, 它有自己的標準 [HTTP Live Streaming](http://tools.ietf.org/html/draft-pantos-http-live-streaming-08)

1. http://www.streaminglearningcenter.com/blogs/apple-to-adobe--microsoft-with-friends-like-you-who-needs-enemies.html
2. http://www.streamingmedia.com/Articles/ReadArticle.aspx?ArticleID=78835
3. http://mashable.com/2011/12/09/apple-mobile-video/
4. http://issuu.com/andruby/docs/http_live_streaming_presentatino

介紹文章

1. http://dashpg.com/?page_id=25
2. http://www.streamingmedia.com/Articles/ReadArticle.aspx?ArticleID=79041
3. http://www.slideshare.net/christian.timmerer/dynamic-adaptive-streaming-over-http-dash
4. http://mpeg.chiariglione.org/working_documents/mpeg-dash/MPEG-DASH-Tutorial.pdf
5. http://www.cash.idv.tw/wordpress/?p=6588
6. http://blog.sina.com.cn/s/blog_4db1790b0100srlv.html
7. http://www.hhi.fraunhofer.de/fields-of-competence/image-processing/research-groups/multimedia-communications/advanced-mpeg-dash.html
8. https://cs.uwaterloo.ca/~brecht/courses/854/readings/mpeg-dash-standard-ieee-mm-2011.pdf

簡報

1. http://www.slideshare.net/cconcolato/live-streaming-of-video-and-subtitles-with-mpegdash
2. http://www.slideshare.net/christian.timmerer/dynamic-adaptive-streaming-over-http-dash
3. http://www.slideshare.net/christian.timmerer/http-streaming-of-mpeg-media
4. http://www.slideshare.net/schellkenig/dash-at-the-acm-multimedia-2011
5. http://www.slideshare.net/christian.timmerer/an-evaluation-of-dynamic-adaptive-streaming-over-http-in-vehicular-environments
6. http://www.slideshare.net/christian.timmerer/a-seamless-web-integration-of-adaptive-http-streaming

### 各種瀏覽器對MPEG DASH的支援狀況

1. Google Chrome 

   Chrome plans to support DASH by using javascript library and MediaSource API \[[1][]\]

   [1]: http://code.google.com/p/chromium/issues/detail?id=109652 
   "Chrome Support MPEG-DASH"

   [MPEG-DASH support in Google Chrome](http://gpac.wp.mines-telecom.fr/2012/08/23/mpeg-dash-support-in-google-chrome)   
   [ASH-JS – A JavaScript- and WebM-based DASH library for Google Chrome](http://www-itec.uni-klu.ac.at/dash/?page_id=746)

2. Opera
 
   [Opera use Javascript extension and Opera Device SDK to support for DASH](http://media.opera.com/media/b2b/tv/201201/Opera_Media_Streaming.pdf)

3. Mozilla Firefox

   Mozilla firefox only plan to support DASH (WebM)   
   https://wiki.mozilla.org/Platform/Roadmap   
   https://bugzilla.mozilla.org/show_bug.cgi?id=702122   
   https://bugzilla.mozilla.org/show_bug.cgi?id=734546   
   [Mozilla adds DASH support (WebM) based on libdash](http://www-itec.uni-klu.ac.at/dash/?p=833)

4. Others

   **vlc**   
   http://www-itec.uni-klu.ac.at/dash/?p=243   

   **MP4Box**   
   http://gpac.wp.mines-telecom.fr/2011/02/02/mp4box-fragmentation-segmentation-splitting-and-interleaving/

   **gstreamer**   
   https://bugzilla.gnome.org/show_bug.cgi?id=675625

   **WebM adaptive streaming**   
   https://groups.google.com/a/webmproject.org/group/webm-discuss/browse_thread/thread/7d2d1faeb2832b94   
   [Instructions to Playback a WebM DASH Presentation](https://sites.google.com/a/webmproject.org/wiki/adaptive-streaming/instructions-to-playback-a-webm-dash-presentation)

### HTML5 相關標準

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
2. MPD Type 為 Dynamic, GPAC 的 MP4Box 支援問題\[[2][]\]\[[3][]\]

[2]: http://sourceforge.net/projects/gpac/forums/forum/327349/topic/5116440
"MPEG Dash: Adding support for MPD.Location"

[3]: http://sourceforge.net/projects/gpac/forums/forum/327349/topic/5439022
"Osmo4 support of dynamic Dash MPD?"

### MPEG DASH DEMO

1. http://dash-mse-test.appspot.com/
2. http://www-itec.uni-klu.ac.at/dash/?page_id=1097
3. http://lists.w3.org/Archives/Public/public-web-and-tv/2012May/0014.html
4. http://wiki.webmproject.org/adaptive-streaming/instructions-to-playback-a-webm-dash-presentation
5. GPAC 提供的各種 MPEG DASH Sequences [http://gpac.wp.mines-telecom.fr/2012/02/23/dash-sequences/](http://gpac.wp.mines-telecom.fr/2012/02/23/dash-sequences/)

### 相關工具

1. http://www.bitmovin.net/libdash/
2. http://www-itec.uni-klu.ac.at/dash/?page_id=746
3. [libdash](http://www-itec.uni-klu.ac.at/dash/?p=553)
4. [MPD Validator](http://www-itec.uni-klu.ac.at/dash/?page_id=605)
5. [DASHEncoder](http://www-itec.uni-klu.ac.at/dash/?page_id=282)

### 相關論文

1. [A Dynamic Adaptive HTTP Streaming Video Service for Google Android](http://web.it.kth.se/~maguire/DEGREE-PROJECT-REPORTS/111006-Luciano-Rubio-with-cover.pdf), [html version](http://dat.etsit.upm.es/~luciano/en/thesis)
2. [Dynamic adaptive streaming over HTTP --: standards and design principles]( http://dl.acm.org/citation.cfm?id=1943572)
3. [A VLC media player plugin enabling dynamic adaptive streaming over HTTP](http://dl.acm.org/citation.cfm?id=2072429)
4. [A Test Bed for DASH over Featuring Session Mobility](http://www-itec.uni-klu.ac.at/bib/files/mueller_A_Test_Bed_for_DASH_featuring_Session_Mobility.pdf)
5. [Usages of DASH for rich media services](http://dl.acm.org/citation.cfm?id=1943587)
6. [Dynamic adaptive HTTP streaming of live content](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5986186&tag=1)
7. [The MPEG-DASH Standard for Multimedia Streaming Over the Internet](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6077864)
8. http://polyu.academia.edu/RickyKPMok/Papers/1161278/QDASH_A_QoE-aware_DASH_system


## HLS

1. http://en.wikipedia.org/wiki/HTTP_Live_Streaming
2. http://tools.ietf.org/html/draft-pantos-http-live-streaming-07
3. http://www-itec.uni-klu.ac.at/dash/?page_id=282
4. http://www.php-oa.com/2010/12/10/http-live-streaming-hls.html

## Others

1. http://www.html5rocks.com/en/tutorials/webgl/typed_arrays/?redirect_from_locale=pt
2. http://sourceforge.net/apps/trac/matroska/wiki/DASH_Profile
3. http://sourceforge.net/projects/gpac/forums/forum/327349/topic/5116440
4. http://en.wikipedia.org/wiki/Dynamic_Adaptive_Streaming_over_HTTP
5. http://en.wikipedia.org/wiki/Helix_Universal_Server
6. https://github.com/DDVTECH/mistlib
7. http://sourceforge.net/apps/mediawiki/osmf.adobe/index.php?title=Customizing_HTTP_Dynamic_Streaming

