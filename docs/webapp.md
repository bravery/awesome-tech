**Table of Contents**
<!-- MarkdownTOC -->

- [WebApp](#webapp)
	- [HTTP/2](#http2)
	- [WebSockets](#websockets)
	- [AMP Accelerated Mobile Pages](#amp-accelerated-mobile-pages)
	- [HTTP Status Codes](#http-status-codes)
	- [Enterprise Search Platforms](#enterprise-search-platforms)
		- [Elasticsearch](#elasticsearch)
	- [Caching](#caching)
	- [Apache and Tomcat](#apache-and-tomcat)
		- [Using JMX to monitor an Application Server running on Docker](#using-jmx-to-monitor-an-application-server-running-on-docker)
	- [ModSecurity Web Application Level Firewall](#modsecurity-web-application-level-firewall)
	- [Nginx](#nginx)
	- [F5 Load Balancer](#f5-load-balancer)
	- [GlassFish](#glassfish)
	- [Wordpress and other CMS solutions like Tiki](#wordpress-and-other-cms-solutions-like-tiki)
	- [WebLogic](#weblogic)
		- [Oracle Blogs: Middleware and Java](#oracle-blogs-middleware-and-java)
		- [WebLogic Resources](#weblogic-resources)
			- [WebLogic and Docker](#weblogic-and-docker)
	- [WebSphere](#websphere)
	- [JVM Latency: Caching, Off Heap, Data Grid](#jvm-latency-caching-off-heap-data-grid)
		- [Java Garbage Collection: Changes in Java 8. JMX monitoring](#java-garbage-collection-changes-in-java-8-jmx-monitoring)
	- [E-Mail](#e-mail)
	- [DNS](#dns)
	- [Video](#video)
	- [JCA Connectors \(TCP/IP resource adapter\). Choosing among JCA, JMS, and web services for Enterprise Application Integration \(EAI\)](#jca-connectors-tcpip-resource-adapter-choosing-among-jca-jms-and-web-services-for-enterprise-application-integration-eai)
	- [Distributed Messaging System. Message oriented middleware](#distributed-messaging-system-message-oriented-middleware)

<!-- /MarkdownTOC -->
[![dilbert](images/dilbert.jpg)](http://dilbert.com/)

<center>

|[![code_org_video](images/code_org_video.jpg)](https://www.youtube.com/user/CodeOrg)|[![codecademy_video](images/codecademy_video.jpg)](https://www.youtube.com/channel/UC5CMtpogD_P3mOoeiDHD5eQ)|[![liferay_video](images/liferay_video.jpg)](https://www.youtube.com/user/liferayinc)|[![tibco_videos](images/tibco_videos.jpg)](https://www.youtube.com/user/TIBCOSoftware)|
|:---:|:---:|:---:|:---:|

|[![svrtech_videos](images/svrtech_videos.jpg)](https://www.youtube.com/user/svrtechnologies)|[![was_videos](images/was_videos.jpg)](https://www.youtube.com/channel/UCjOtFEHSAXN-1MBLW_sMASw)|[![ibm_support_tv](images/ibm_support_tv.jpg)](https://www.youtube.com/user/WebSphereEducation)|[![ibm_messaging](images/ibm_messaging.jpg)](https://www.youtube.com/user/IBMmessagingMedia)|[![ibm_integration_video](images/ibm_integration_video.jpg)](https://www.youtube.com/user/IBMintegrationMedia)|
|:---:|:---:|:---:|:---:|:---:|

|[![oracle_fusion_apps_videos](images/oracle_fusion_apps_videos.jpg)](https://www.youtube.com/user/FADeveloperRelations)|[![adf_essentials_videos](images/adf_essentials_videos.jpg)](https://www.youtube.com/user/ADFInsiderEssentials)|[![oracle_adf_java_video](images/oracle_adf_java_video.jpg)](https://www.youtube.com/channel/UCX7PJW3a2qvEoBgBlm8jE_g)|[![oracle_learning_library_video](images/oracle_learning_library_video.jpg)](https://www.youtube.com/user/OracleLearning)|[![c2b2_videos](images/c2b2_videos.jpg)](https://www.youtube.com/user/C2B2Consulting)|[![oracle_testlab_video](images/oracle_testlab_video.jpg)](https://www.youtube.com/channel/UCR3WQHwHzCBRYC42lBFqtfA)|
|:---:|:---:|:---:|:---:|:---:|:---:|

</center>

# WebApp
## HTTP/2
- [SPDY & HTTP 2 with Akamai CTO Guy Podjarny](https://www.youtube.com/watch?v=WkLBrHW4NhQ)
	- [cURL mantainer: http2 explained 🌟](http://http2-explained.haxx.se/)
	- [cURL mantainer: curl and HTTP/2 by default](http://daniel.haxx.se/blog/2015/12/14/curl-and-http2-by-default/)
	- [cURL mantainer: A 2015 retrosprective](http://daniel.haxx.se/blog/2015/12/20/a-2015-retrospective/)
	- [http2.github.io HTTP/2 🌟](https://http2.github.io)
	- [http2.github.io HTTP/2 Frequently Asked Questions 🌟](https://http2.github.io/faq/)
	- [HTTP/2 resources](https://pinboard.in/u:rmurphey/t:http2/)
	- [A Simple Performance Comparison of HTTPS, SPDY and HTTP/2 🌟](https://blog.httpwatch.com/2015/01/16/a-simple-performance-comparison-of-https-spdy-and-http2/comment-page-1/)
	- [blog.cloudflare.com - Tools for debugging, testing and using HTTP/2](https://blog.cloudflare.com/tools-for-debugging-testing-and-using-http-2/)
	- [blog.cloudflare.com - HTTP/2 For Web Developers](https://blog.cloudflare.com/http-2-for-web-developers/)
- [HTTP/2 With JBoss EAP 7 - Tech Preview](http://blog.eisele.net/2015/11/http2-with-jboss-eap-7.html)
	- [Dzone - HTTP/2 With JBoss EAP 7: Tech Preview](https://dzone.com/articles/http2-with-jboss-eap-7-tech-preview)
- [simple-talk.com: Script Loading between HTTP/1.1 and HTTP/2](https://www.simple-talk.com/dotnet/asp.net/script-loading-between-http1.1-and-http2/)
- [5 Tips to Boost the Performance of Your Apache Web Server](http://www.tecmint.com/apache-performance-tuning/)
- [DZone: How HTTP/2 Is Changing Web Performance Best Practices](https://dzone.com/articles/how-http2-is-changing-web-performance-best-practic-2) For people who write code for the web, transitioning to HTTP/2 isn’t always straightforward, and a speed boost isn’t automatically guaranteed. This article is an introduction to HTTP/2 and how it changes web performance best practices.

[![dzone_refcard_introduction_http](images/dzone_refcard_introduction_http.png)](https://dzone.com/refcardz/http-hypertext-transfer-0)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/WkLBrHW4NhQ?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/t9iH0GHtiPuf6q" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/lmacvittie/http2-changes-everything" title="HTTP/2 Changes Everything" target="_blank">HTTP/2 Changes Everything</a> </strong> from <strong><a href="//www.slideshare.net/lmacvittie" target="_blank">Lori MacVittie</a></strong> </div>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">The day Google Chrome disabled HTTP/2 for nearly everyone: May 15th, 2016<a href="https://t.co/C6YU50urdv">https://t.co/C6YU50urdv</a></p>&mdash; ma.ttias.be (@mattiasgeniar) <a href="https://twitter.com/mattiasgeniar/status/731463130698678273">14 de mayo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

[![middleware_market](images/middleware_market.png)](http://bushorn.com/middleware-market-revisited/)

## WebSockets
- [WebSocket](https://en.wikipedia.org/wiki/WebSocket)
- [The State of Real-Time Web in 2016](https://banksco.de/p/state-of-realtime-web-2016.html)
- [SPDY and WebSocket Support at Akamai](https://blogs.akamai.com/2012/07/spdy-and-websocket-support-at-akamai.html)

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/dGwSJnsiEBOLQF" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/MarkRoden/websockets-pushing-the-web-forward" title="Websockets: Pushing the web forward" target="_blank">Websockets: Pushing the web forward</a> </strong> from <strong><a href="//www.slideshare.net/MarkRoden" target="_blank">Mark Roden</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/J3GFdDQf8wm4fW" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/ramisayar/state-of-web-sockets" title="The State of WebSockets in Django" target="_blank">The State of WebSockets in Django</a> </strong> from <strong><a href="//www.slideshare.net/ramisayar" target="_blank">Rami Sayar</a></strong> </div>
</div>
<br/>

## AMP Accelerated Mobile Pages
- A free, open source service that does all the work to make sites load fast
- [Google’s plan to speed up the mobile Web: Burn it down 🌟](http://thenextweb.com/insider/2015/10/07/googles-plan-to-speed-up-the-mobile-web-burn-it-down/)
- [ampproject.org](https://www.ampproject.org) Accelerated Mobile Pages Project
- [github.com/ampproject](https://github.com/ampproject)
- [Introducing the Accelerated Mobile Pages Project, for a faster, open mobile web](https://googleblog.blogspot.com.es/2015/10/introducing-accelerated-mobile-pages.html)
- [How AMP Speeds Up Performance](https://www.ampproject.org/docs/get_started/technical_overview.html)
- [Google to Roll Out Accelerated Mobile Pages to Everyone, Get Your Content Ready Now](https://www.searchenginejournal.com/google-to-roll-out-accelerated-mobile-pages-to-everyone-get-your-content-ready-now/)
- [Google Rolls Out The Accelerated Mobile Pages Project To Help Webpages Load Instantaneously On Your Phone Or Tablet](http://www.androidpolice.com/2015/10/07/google-rolls-out-the-accelerated-mobile-pages-project-to-help-webpages-load-instantaneously-on-your-phone-or-tablet/)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Accelerated Mobile Pages (AMP): Open or closed? <a href="https://t.co/ekMXovhcjC">https://t.co/ekMXovhcjC</a> <a href="https://twitter.com/matthewtift">@matthewtift</a> <a href="https://t.co/tGHdZxWdSi">pic.twitter.com/tGHdZxWdSi</a></p>&mdash; Open Source Way (@opensourceway) <a href="https://twitter.com/opensourceway/status/717715489250607104">6 de abril de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## HTTP Status Codes
- [wikipedia: List of HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)
- [slideshare: Http Status Code Errors in SEO](http://www.slideshare.net/AdelaRoger/http-status-code-errors-in-seo)

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/gYWUVIcqW40OUn" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/mainstreethost/http-status-codes-cheat-sheet" title="HTTP Status Codes Cheat Sheet: An Exhaustive List" target="_blank">HTTP Status Codes Cheat Sheet: An Exhaustive List</a> </strong> from <strong><a href="//www.slideshare.net/mainstreethost" target="_blank">Mainstreethost</a></strong> </div>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Awesome 404 page <a href="https://t.co/yN5Yj5se0d">https://t.co/yN5Yj5se0d</a> <a href="https://twitter.com/hashtag/sysadmin?src=hash">#sysadmin</a> <a href="https://twitter.com/hashtag/humor?src=hash">#humor</a> <a href="https://twitter.com/hashtag/apache?src=hash">#apache</a> <a href="https://twitter.com/hashtag/Linux?src=hash">#Linux</a> <a href="https://twitter.com/hashtag/Redhat?src=hash">#Redhat</a> <a href="https://t.co/1Z4aMRpgr1">pic.twitter.com/1Z4aMRpgr1</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/711098719425265664">19 de marzo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Web server 404 page ;) Them vs us. <a href="https://twitter.com/hashtag/sysadmin?src=hash">#sysadmin</a> <a href="https://twitter.com/hashtag/devops?src=hash">#devops</a> <a href="https://t.co/fJxXDqK1qr">pic.twitter.com/fJxXDqK1qr</a></p>&mdash; nixCraft # (@nixcraft) <a href="https://twitter.com/nixcraft/status/787248098024108032">15 de octubre de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## Enterprise Search Platforms
- [Apache Solr vs ElasticSearch](http://solr-vs-elasticsearch.com/)
- [javacodegeeks.com: Apache Lucene Fundamentals Tutorial](http://www.javacodegeeks.com/2015/09/apache-lucene-fundamentals.html)

### Elasticsearch
- [Elasticsearch](elasticsearch.md)

## Caching
- [Caching](caching.md)

## Apache and Tomcat
- [code.tutsplus.com: An Introduction to Apache](https://code.tutsplus.com/tutorials/an-introduction-to-apache--net-25786)
- [5 Tips to Boost the Performance of Your Apache Web Server](http://www.tecmint.com/apache-performance-tuning/)
- [How to set up a cluster with Tomcat 8, Apache and mod_jk.Tomcat Performance Monitoring and Tuning](http://blog.c2b2.co.uk/2014/05/tomcat-performance-monitoring-and-tuning.html)
- [scriptrock.com: 15 Ways To Secure Apache Tomcat 8](https://www.scriptrock.com/articles/15-ways-to-secure-apache-tomcat-8)
- [middlewaresnippets.blogspot.com - Working with Apache HTTP Server](http://middlewaresnippets.blogspot.com/2015/05/working-with-apache-http-server.html)
	- [middlewaresnippets.blogspot.com - Working some more with Apache HTTP Server](http://middlewaresnippets.blogspot.com/2015/09/working-some-more-with-apache-http.html)
- [nixCraft: PHP-fpm Too Many Open Files 24 Error (set open file descriptor limit)](http://www.cyberciti.biz/faq/php-5-7-fpm-set-open-file-descriptor-limit-on-linux-unix/)
- [unixmen.com: Apache Performance Tuning](https://www.unixmen.com/apache-performance-tuning/)
- [askapache.com: htaccess - Ultimate Apache .htaccess file Guide](http://www.askapache.com/htaccess/htaccess.html)
- [creativebloq.com: Protect WordPress sites with .htaccess](http://www.creativebloq.com/wordpress/protect-your-wordpress-site-htaccess-4122793)
- [codular.com: Introduction to .htaccess](http://codular.com/htaccess-introduction)
- [moz.com: 10 .htaccess File Snippets You Should Have Handy](https://moz.com/blog/htaccess-file-snippets-for-seos)
- [unixmen.com: Setup Apache Virtual Hosts On Ubuntu 15.10](https://www.unixmen.com/setup-apache-virtual-hosts-on-ubuntu-15-10/)
- [Apache httpd Reverse Proxy 🌟](http://jimjag.com/imo/index.php?/archives/266-Apache-httpd-Reverse-Proxy.html)
- [httpd.apache.org: Apache Module mod_proxy_hcheck](https://httpd.apache.org/docs/trunk/mod/mod_proxy_hcheck.html)
- [cvedetails.com: Apache » Http Server : Security Vulnerabilities 🌟](http://www.cvedetails.com/vulnerability-list/vendor_id-45/product_id-66/Apache-Http-Server.html)
- [Tecmint: GoAccess (A Real-Time Apache and Nginx) Web Server Log Analyzer 🌟🌟🌟](http://www.tecmint.com/goaccess-a-real-time-apache-and-nginx-web-server-log-analyzer/)
- [Tecmit: httpstat – A Curl Statistics Tool to Check Website Performance](http://www.tecmint.com/httpstat-curl-statistics-tool-check-website-performance/)
- [Apache Authentication with System Accounts? (PAM authentication)](http://www.spinics.net/linux/fedora/fedora-users/msg473705.html)
- [reddit.com: httpd web authentication using ac/dc sssd credentials 🌟](https://www.reddit.com/r/linuxadmin/comments/56fx3i/httpd_web_authentication_using_acdc_sssd/)

[![How Apache Is Losing The Web To NGINX 2](images/nginx-w3techs-data.jpg)](http://www.nextplatform.com/2016/02/24/how-apache-is-losing-the-web-to-nginx/)

[![dzone_refcard_essential_apache](images/dzone_refcard_essential_apache.png)](https://dzone.com/refcardz/essential-apache-http-server)

[![dzone_refcard_apache_tomcat](images/dzone_refcard_apache_tomcat.png)](https://dzone.com/refcardz/getting-started-with-apache-tomcat)

<div class="container">
<iframe src="https://player.vimeo.com/video/62427114" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen class="video"></iframe>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">25 Apache Interview Questions for Beginners and Intermediates <a href="https://t.co/6TdTK3j3wC">https://t.co/6TdTK3j3wC</a> … RT <a href="https://twitter.com/linuxtoday">@linuxtoday</a> <a href="https://twitter.com/hashtag/linux?src=hash">#linux</a> <a href="https://t.co/YPbRItIRdH">pic.twitter.com/YPbRItIRdH</a></p>&mdash; TecMint.com (@tecmint) <a href="https://twitter.com/tecmint/status/748452881087422464">30 de junio de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr"><a href="https://t.co/RDFES9fHG6">https://t.co/RDFES9fHG6</a> - easily strace all your apache processes (gormux) <a href="https://twitter.com/hashtag/awk?src=hash">#awk</a> <a href="https://twitter.com/hashtag/grep?src=hash">#grep</a> <a href="https://twitter.com/hashtag/ps?src=hash">#ps</a> <a href="https://twitter.com/hashtag/strace?src=hash">#strace</a></p>&mdash; CommandLineFu (@commandlinefu) <a href="https://twitter.com/commandlinefu/status/761154707767238657">4 de agosto de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">How to Password Protect Web Directories in Apache Using .htaccess File<a href="https://t.co/oXdulivljg">https://t.co/oXdulivljg</a><br>RT <a href="https://twitter.com/linuxtoday">@linuxtoday</a> <a href="https://twitter.com/hashtag/apache?src=hash">#apache</a> <a href="https://twitter.com/hashtag/Linux?src=hash">#Linux</a> <a href="https://t.co/D1DyiDbGN3">pic.twitter.com/D1DyiDbGN3</a></p>&mdash; Linux Inside (@tecmint) <a href="https://twitter.com/tecmint/status/787880606478667776">17 de octubre de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

### Using JMX to monitor an Application Server running on Docker
- [software.dell.com: Using JMX to monitor an Application Server running on Docker](https://software.dell.com/blog/en/using-jmx-to-monitor-an-application-server-running-on-docker)
	- [youtube - JMX Monitoring for Java Application running on Docker (Apache Tomcat Example) ](https://www.youtube.com/watch?v=tVL3hkA149o)

## ModSecurity Web Application Level Firewall
- [modsecurity.org](https://www.modsecurity.org/) ModSecurity is an open source, cross-platform web application firewall (WAF) module. Known as the "Swiss Army Knife" of WAFs, it enables web application defenders to gain visibility into HTTP(S) traffic and provides a power rules language and API to implement advanced protections.

[![modsecurity_logo](images/modsecurity_logo.png)](https://www.modsecurity.org/)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/AqNWLms7zvw?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

## Nginx
- [Nginx](nginx.md)

## F5 Load Balancer
- [F5 Load Balancer](f5lb.md)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Setting Up Web Servers Load Balancing Using ‘POUND’ on RHEL/CentOS<a href="https://t.co/wQaPsLUzbn">https://t.co/wQaPsLUzbn</a><br>RT <a href="https://twitter.com/linuxtoday">@linuxtoday</a> <a href="https://twitter.com/hashtag/Linux?src=hash">#Linux</a> <a href="https://t.co/HwKdBKcKQh">pic.twitter.com/HwKdBKcKQh</a></p>&mdash; Linux Inside (@tecmint) <a href="https://twitter.com/tecmint/status/789331376839401472">21 de octubre de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## GlassFish
- [GlassFish](https://glassfish.java.net/)
- [twitter.com/glassfish](https://twitter.com/glassfish)

## Wordpress and other CMS solutions like Tiki
- [stosu.com](https://stosu.com) Free How-To Tutorials for WordPress and Windows Users
- [How to install WordPress on a CentOS 7/RHEL 7 server](http://bach-online.de/2016/07/25/how-to-install-wordpress-on-a-centos-7-rhel-7-server/)
- [DZone: Customizing User Roles in WordPress](https://dzone.com/articles/explaining-user-roles-in-wordpress) There are five default user roles in WordPress with their own set of configurable capabilities. Let's look at what they are and how to customize them.
- [unixmen.com: Install Tiki CMS Groupware On Ubuntu 15.10](https://www.unixmen.com/install-tiki-cms-groupware-ubuntu-15-10/)

## WebLogic
### Oracle Blogs: Middleware and Java
- [WebLogic Community](http://weblogiccommunity.com)
- [Oracle EMEA Partner Community for WebLogic (WLS)](http://www.oracle.com/partners/goto/wls-emea)
- [Oracle Middleware Blog](http://oraclemiddlewareblog.com/)
- [oraclejavamagazine-digital.com - Java Magazine](http://www.oraclejavamagazine-digital.com)
- [javacodegeeks.com](http://www.javacodegeeks.com/)
- [Oracle Community](https://community.oracle.com)
	- [Oracle Community - WebLogic](https://community.oracle.com/community/fusion_middleware/weblogic)
- [middlewaresnippets.blogspot.com](http://middlewaresnippets.blogspot.com)
- [Unversioned.blogspot.gr](http://unversioned.blogspot.gr/) Open Source, Linux, Java, WebLogic, DevOps, FMW, SOA
- [multikoop.blogspot.com - Practical experience on Oracle products. WebLogic, ADF, MAF, SOA, WebCenter, JDeveloper, Oracle Cloud](http://multikoop.blogspot.com)
	- [multikoop.blogspot.com - WebLogic](http://multikoop.blogspot.com/search/label/weblogic)
- [avanttic blog](http://blog.avanttic.com/)
	- [avanttic blog - weblogic](http://blog.avanttic.com/tag/weblogic/)

### WebLogic Resources
- [WebLogic 12c Enterprise Deployment Architecture in the Amazon Cloud](http://oraclemiddlewareblog.com/2015/10/13/weblogic12c-architecture-in-the-amazon-cloud/)
- [SlideShare - 12 Things You Should Know About WebLogic Server 12.2.1](http://www.slideshare.net/FrankMunz1/12-things-you-should-know-about-weblogic-server-1221-oow2015)
- [middlewaresnippets.blogspot.com - WebLogic Server on Linux 7](http://middlewaresnippets.blogspot.com/2015/04/weblogic-server-on-linux-7.html)
	- [middlewaresnippets.blogspot.com - WebLogic Domain Partitioning](http://middlewaresnippets.blogspot.com/2015/11/weblogic-domain-partitioning.html)
	- [middlewaresnippets.blogspot.com - Monitoring Domain Partitions](http://middlewaresnippets.blogspot.com/2015/11/monitoring-domain-partitions.html)
	- [middlewaresnippets.blogspot.com - Deploying Applications to Domain Partitions](http://middlewaresnippets.blogspot.com/2015/11/deploying-applications-to-domain.html)
	- [middlewaresnippets.blogspot.com - Security Recovery - LDAP server](http://middlewaresnippets.blogspot.com/2015/07/security-recovery.html)
- [blogs.oracle.com - WLST Scripting to Get WebLogic Libraries and Deployed Applications](https://blogs.oracle.com/practicalbpm/entry/wlst_scripting_to_get_weblogic)
- [Java Serialization Vulnerability Threatens Millions of Applications . Contrast security is promoting their solution for a vulnerability that affects WebLogic, WebSphere, JBoss, Jenkins, and OpenNMS.](https://dzone.com/articles/java-serialization-vulnerability-threatens-million)
- [Oracle WebLogic Server 12c Advanced Administration Cookbook](http://it-ebooks.info/book/3020/)
- [weblogiccommunity.com: WLS 12.2.1 Oracle Universal Connection Pool (UCP) Datasource](http://weblogiccommunity.com/2015/12/26/wls-ucp-datasource-by-steve-felts/)
- [Deploying to the Oracle Java Cloud Service using FlexDeploy](http://flexagon.com/2015/07/deploying-to-the-oracle-java-cloud-service-using-flexdeploy/)
- [javacodegeeks.com: Weblogic Server Administration Tutorial](http://examples.javacodegeeks.com/core-java/weblogic-server-administration-tutorial/)
- [Automated Software Testing of Fusion Middleware applications with FlexDeploy](http://adfpractice-fedor.blogspot.com.br/2015/10/automated-software-testing-of-fusion.html)
- [WLSDM | Native WebLogic Smart Dashboard & Monitoring](http://www.wlsdm.com) WLSDM is a WebLogic console extension which enables monitoring for WebLogic MBean metrics. It is very easy to create alarms and notifications by using WLSDM metric browser. WLSDM can store any WebLogic metric values historically and also can generate graphical reports.
	- [Advanced WebLogic Monitoring: Develop JMX MBeans and Automate with WLSDM Metric Actions 🌟](http://www.wlsdm.com/tutorials/advanced-weblogic-monitoring-develop-jmx-mbeans-and-automate-with-wlsdm-metric-actions/)
- [DZone: WebLogic Performance and Tuning: Part 1 🌟🌟🌟](https://dzone.com/articles/weblogic-performance-and-tuning-part-1) The Java Virtual machine, or JVM, on which WebLogic server runs, is the single most important software component of your system. Fortunately, it is not terribly difficult to properly configure your JVM.

#### WebLogic and Docker
- [WebLogic and Docker](docker.md#weblogic-via-docker)

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/tUDLzhM0sgSgcp" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/FrankMunz1/12-things-you-should-know-about-weblogic-server-1221-oow2015" title="12 Things You Should Know About WebLogic Server 12.2.1 #oow2015 " target="_blank">12 Things You Should Know About WebLogic Server 12.2.1 #oow2015 </a> </strong> from <strong><a href="//www.slideshare.net/FrankMunz1" target="_blank">Frank Munz</a></strong> </div>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">JDK 8 and WebLogic 12.2.1 by Frank Munz <a href="https://t.co/rByhPDsB7v">https://t.co/rByhPDsB7v</a></p>&mdash; WebLogic Community (@wlscommunity) <a href="https://twitter.com/wlscommunity/status/696229275150602240">febrero 7, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## WebSphere

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/COnHzzVxCpw?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

## JVM Latency: Caching, Off Heap, Data Grid
- [dzone.com - Refcard: Java Caching. JCache and other caching APIs, as well as multiple strategies for implementing temporary data storage in your application](http://bit.ly/1RbGgms)
- [Reminder: JDK 7 will be EOL soon. Oracle won't publish any Public Updates to JDK 7 after April 2015](http://www.oracle.com/technetwork/java/javase/downloads/eol-135779.html)
- [Free eGuide: JVM Troubleshooting Guide](http://freepromagazine.blogspot.de/2014/07/free-eguide-jvm-troubleshooting-guide.html)
- [Tecnologías de Heap-Offloading son EHcache, Memcached, Jillegal library, etc.](http://ehcache.org/)
- [Jillegal OffHeap Module](https://github.com/serkan-ozal/jillegal)
- [vogella.com: Java Performance - Memory and Runtime Analysis - Tutorial](http://www.vogella.com/tutorials/JavaPerformance/article.html)
- [On heap vs off heap memory usage](http://www.javacodegeeks.com/2014/12/on-heap-vs-off-heap-memory-usage.html)
- [Dr. Low Latency or: How I Learned to Stop Worrying about Pauses and Love the Memory](http://www.c2b2.co.uk/javazone-2013-low-latency)
- [What is a Data Grid?](http://www.c2b2.co.uk/what_is_data_grid_webinar)

### Java Garbage Collection: Changes in Java 8. JMX monitoring
- [How Garbage Collection differs in the three big JVMs](http://apmblog.dynatrace.com/2011/05/11/how-garbage-collection-differs-in-the-three-big-jvms/)
- [One important change in Memory Management in Java 8](http://karunsubramanian.com/websphere/one-important-change-in-memory-management-in-java-8/)
	- [PermGen removed](http://www.infoq.com/articles/Java-PERMGEN-Removed)
	- [Mi análisis: cambios en la gestión de memoria de Java 8. Diferencias en distintas implementaciones de JVM](jvm-mem.md)
- [middlewaresnippets.blogspot.com - Monitoring with JMX](http://middlewaresnippets.blogspot.com/2014/10/monitoring-with-jmx.html)
- [Cambios importantes en la gestión de memoria de Java 8 de Oracle](http://karunsubramanian.com/websphere/one-important-change-in-memory-management-in-java-8/)
	- [PermGen eliminado](http://www.infoq.com/articles/Java-PERMGEN-Removed)
- [cubrid.org: How to Tune Java Garbage Collection](http://www.cubrid.org/blog/dev-platform/how-to-tune-java-garbage-collection)
- [DZone: Revisiting the Advanced Theories of ‘Java Garbage Collection’ 🌟🌟🌟](https://dzone.com/articles/revisiting-the-advanced-theories-of-java-garbage-c)
- [DZone: Understanding the Java Memory Model and Garbage Collection 🌟🌟🌟](https://dzone.com/articles/understanding-the-java-memory-model-and-the-garbag) In this article we will try to understand the Java memory model and how garbage collection works. In this article I have used JDK8 Oracle Hot Spot 64 bit JVM. First let me depict the different memory areas available for Java processes.

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/n2WeaBLq1lzQcN" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/ihji/jvm-garbage-collection-tuning" title="JVM Garbage Collection Tuning" target="_blank">JVM Garbage Collection Tuning</a> </strong> from <strong><a href="//www.slideshare.net/ihji" target="_blank">ihji</a></strong> </div>
</div>
<br/>

## E-Mail
- [tech-faq.com: How Does the Email System Work?](http://www.tech-faq.com/how-the-email-system-works.html)
- [Best Transactional Email Service Comparison](http://socialcompare.com/en/comparison/transactional-emailing-providers-mailjet-sendgrid-critsend)
- [Google Improves Gmail’s Spam Filters, Launches New Analytics Tool For Bulk Senders](http://techcrunch.com/2015/07/09/google-improves-gmails-spam-filters-launches-new-analytics-tool-for-bulk-senders/)
- [five.sentenc.es: email productivity](http://five.sentenc.es/)
- [Amazon’s Email And Calendaring Service, Amazon WorkMail, Exits Preview](http://techcrunch.com/2016/01/05/amazons-own-email-calendaring-service-amazon-workmail-exits-preview/)
- [How the US Military Fails to Protect Its Soldiers' Emails](http://motherboard.vice.com/read/how-the-us-military-fails-to-protect-soldiers-emails)

[![email service comparison](images/email_service_comparison.png)](http://socialcompare.com/en/comparison/transactional-emailing-providers-mailjet-sendgrid-critsend)

[![email socialcompare](images/email_socialcompare.png)](http://socialcompare.com/en/comparison/transactional-emailing-providers-mailjet-sendgrid-critsend)

<center>
<div class="tumblr-post" data-href="https://embed.tumblr.com/embed/post/Y6ORssbcHF5P4Puns-jRoA/135651440303" data-did="71388c85aaa3dbabd324ee9a8d32e830cc3a9972"><a href="http://securityreactions.tumblr.com/post/135651440303/nmap-has-discovered-an-open-smtp-relay">http://securityreactions.tumblr.com/post/135651440303/nmap-has-discovered-an-open-smtp-relay</a></div><script async src="https://secure.assets.tumblr.com/post.js"></script>
</center>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Internet Draft: SMTP Strict Transport Security <a href="https://twitter.com/hashtag/infosec?src=hash">#infosec</a> <a href="https://twitter.com/hashtag/email?src=hash">#email</a> <a href="https://twitter.com/hashtag/sysadmin?src=hash">#sysadmin</a>  <a href="https://t.co/SNiwaGZ2xH">https://t.co/SNiwaGZ2xH</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/711739784637521921">21 de marzo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Even the FBI, DNI and the CIA don’t implement STARTTLS on their email server, but The NSA, on the other hand, does 🤔 <a href="https://t.co/xSTsR0NATY">https://t.co/xSTsR0NATY</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/713581832625754112">26 de marzo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## DNS
- [DNS: What Can Go Wrong and How You Can Fix It | @DevOpsSummit #APM #Agile #DevOps](http://java.sys-con.com/node/3884842) DNS enables users of all skill sets and technical knowledge levels to use this incredibly advanced resource on a daily basis
- [DZone: How to Configure Your DNS With Cloud 66 for High Availability](https://dzone.com/articles/how-to-configure-your-dns-with-cloud-66-for-high-a) If you're using Cloud 66, here's a quick and easy tutorial to show you how to set your site up for high availability.
- [How To Flush Linux/UNIX DNS Cache](http://www.cyberciti.biz/faq/rhel-debian-ubuntu-flush-clear-dns-cache/)
- [unixmen.com: How To Setup DNS Server In Ubuntu 15.10](http://www.unixmen.com/how-to-setup-dns-server-in-ubuntu-15-10/)
- [linux.com: Dig Into DNS: Part 1](https://www.linux.com/learn/dig-dns-part-1)
- [datapath.io: What is Domain Name System (DNS)?](https://datapath.io/resources/blog/what-is-domain-name-system-dns)

[![dzone_refcard_practical_dns](images/dzone_refcard_practical_dns.png)](https://dzone.com/refcardz/dns)

## Video
- [List of streaming media systems](https://en.wikipedia.org/wiki/List_of_streaming_media_systems)
- [Wikipedia: Wowza Streaming Engine](https://en.wikipedia.org/wiki/Wowza_Streaming_Engine)
- [wowza.com](https://www.wowza.com)
- [slideshare: Wowza installation](http://www.slideshare.net/AstinChoi/wowza-installation-16296376)
- [slideshare: Live Audio Broadcast with Wowza Media Server](http://www.slideshare.net/neevtech/live-audio-broadcast-with-wowza-media-server)
- [slideshare: AWS Webcast - Live Streaming using Amazon CloudFront and Wowza Media Server](http://www.slideshare.net/AmazonWebServices/2013-1023wowzalivestreamingwebinarniharchris)
- [slideshare: Video Streaming Services](http://www.slideshare.net/oodlestech/video-streaming-26933089)
- [kaltura.org](http://www.kaltura.org)
- [BBC R&D: H.265/HEVC vs H.264/AVC: 50% bit rate savings verified](http://www.bbc.co.uk/rd/blog/2016/01/h-dot-265-slash-hevc-vs-h-dot-264-slash-avc-50-percent-bit-rate-savings-verified) A research team from the BBC has done a series of tests to confirm earlier computations showing a ~50% savings in bit rate for H.265/HEVC compared to video using H.264/AVC at comparable quality. 
- [Build your own live streaming app in 5 minutes! 🌟🌟](https://www.nanocosmos.de/blog/2016/03/build-your-own-app-stream-like-periscope/)
- [emezeta.com: Cómo usar ffmpeg para editar video](http://www.emezeta.com/articulos/como-usar-ffmpeg-para-editar-video)
- [unixmen.com: Setup A Centralized Media Server Using Emby Server](https://www.unixmen.com/setup-a-centralized-media-server-using-emby-server/)
- [DZone: How Netflix Changed Streaming](https://dzone.com/articles/how-netflix-is-so-versatile) Everyone knows about Netflix's move to the cloud. But it's staggering to realize just how much that philosophy has trickled down into every part of the business.

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Why HBO is so scared of Netflix <a href="https://t.co/AVwt6IfP72">https://t.co/AVwt6IfP72</a> <a href="https://t.co/ZmBfSkE1Dg">pic.twitter.com/ZmBfSkE1Dg</a></p>&mdash; Business Insider (@businessinsider) <a href="https://twitter.com/businessinsider/status/699642563486203904">febrero 16, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="es" dir="ltr">¿Supondrá Google el fin de la televisión local? <a href="https://t.co/z2sv5JcWcF">https://t.co/z2sv5JcWcF</a></p>&mdash; Cinco Días (@CincoDiascom) <a href="https://twitter.com/CincoDiascom/status/737361608393916417">30 de mayo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/x1wiZ4pS36i1b" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/AmazonWebServices/2013-1023wowzalivestreamingwebinarniharchris" title="AWS Webcast - Live Streaming using Amazon CloudFront and Wowza Media Server" target="_blank">AWS Webcast - Live Streaming using Amazon CloudFront and Wowza Media Server</a> </strong> from <strong><a target="_blank" href="//www.slideshare.net/AmazonWebServices">Amazon Web Services</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/nIkst07HidQ?list=PL0PgyVP0Ux_L4W13d5WEtlZrqCBrrSWdR" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">YouTube’s new Director tools allow small businesses to create video ads on their phones <a href="https://t.co/7OOZeT4KoX">https://t.co/7OOZeT4KoX</a> by <a href="https://twitter.com/anthonyha">@anthonyha</a></p>&mdash; TechCrunch (@TechCrunch) <a href="https://twitter.com/TechCrunch/status/743096005105590273">15 de junio de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Audio music streams just surpassed video streams for the 1st time in history <a href="https://t.co/FRHDCSEqbq">https://t.co/FRHDCSEqbq</a> <a href="https://t.co/Q7goNhWrz9">pic.twitter.com/Q7goNhWrz9</a></p>&mdash; Forbes (@Forbes) <a href="https://twitter.com/Forbes/status/751516459449417729">8 de julio de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## JCA Connectors (TCP/IP resource adapter). Choosing among JCA, JMS, and web services for Enterprise Application Integration (EAI)
- [Choosing among JCA, JMS, and web services for EAI](http://www.ibm.com/developerworks/library/ws-jcajms/) This article discusses criteria for choosing among J2C Connector Architecture (JCA), Java Message Service (JMS), and web services implementations, depending on your existing environments, the patterns you want to implement, and the your preset requirements for loose or tight coupling.
- [JBoss EAP 6: Configure the Java Connector Architecture (JCA) Subsystem](https://access.redhat.com/documentation/en-US/JBoss_Enterprise_Application_Platform/6/html/Administration_and_Configuration_Guide/Configure_the_Java_Connector_Architecture_JCA_Subsystem.html)
- [Netty JCA Connector](https://en.wikipedia.org/wiki/Netty_(software))

## Distributed Messaging System. Message oriented middleware 
- [RabbitMQ](https://www.rabbitmq.com/)
- [Apache Kafka](http://kafka.apache.org/)
- [Setting Up and Running Apache Kafka on Windows OS](https://dzone.com/articles/running-apache-kafka-on-windows-os)
- [Lose the Lock While Embracing Concurrency](https://dzone.com/articles/lose-the-lock-while-embracing-concurrency-brave-ne) Adopting concurrency? You may want to lose the lock. Here's a look at basics with message routing, such as concurrent timelines, linearizability​, and more!
- [DZone refcard: AMQP Essentials](https://dzone.com/refcardz/amqp-essentials) The Binary Transfer Protocol for Enterprise Applications and IoT
- [Simple job queue in Bash using a FIFO](http://blog.garage-coding.com/2016/02/05/bash-fifo-jobqueue.html)
- [DZone: Diving Into MQTT](https://dzone.com/articles/mqtt-protocol-tutorial) MQTT can make communication in the world of IoT a lot easier. Read on to find out what it is and how to use it.

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/egsQRPlbfRcgTt" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/PovilasBalzaravicius/reducing-load-with-rabbitmq" title="Reducing load with RabbitMQ" target="_blank">Reducing load with RabbitMQ</a> </strong> from <strong><a href="//www.slideshare.net/PovilasBalzaravicius" target="_blank">Povilas Balzaravičius</a></strong> </div>
</div> 
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/4LiXl3TsDw9N9O" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/opensourcementor/webinar-maximize" title="Maximize information exchange in your enterprise with AMQP" target="_blank">Maximize information exchange in your enterprise with AMQP</a> </strong> from <strong><a href="//www.slideshare.net/opensourcementor" target="_blank">Kenneth Peeples</a></strong> </div>
</div> 
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Explore the fundamentals of <a href="https://twitter.com/hashtag/MQTT?src=hash">#MQTT</a>, including message types, QoS levels &amp; security. <a href="https://t.co/wNE6LGfIqJ">https://t.co/wNE6LGfIqJ</a> <a href="https://t.co/aTvvSFddOn">pic.twitter.com/aTvvSFddOn</a></p>&mdash; DZone (@DZone) <a href="https://twitter.com/DZone/status/710065762497634304">16 de marzo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>