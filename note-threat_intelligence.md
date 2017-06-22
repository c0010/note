<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Threat Intelligence</a>
<ul>
<li><a href="#sec-1-1">1.1. source introduction</a>
<ul>
<li><a href="#sec-1-1-1">1.1.1. source add</a></li>
<li><a href="#sec-1-1-2">1.1.2. alexa.com</a></li>
<li><a href="#sec-1-1-3">1.1.3. reputation.alienvault.com</a></li>
<li><a href="#sec-1-1-4">1.1.4. osint.bambenekconsulting.com</a></li>
<li><a href="#sec-1-1-5">1.1.5. blocklist.de</a></li>
<li><a href="#sec-1-1-6">1.1.6. umbrella.cisco.com</a></li>
<li><a href="#sec-1-1-7">1.1.7. csirtg.io</a></li>
<li><a href="#sec-1-1-8">1.1.8. danger.rulez.sk</a></li>
<li><a href="#sec-1-1-9">1.1.9. dataplane.org</a></li>
<li><a href="#sec-1-1-10">1.1.10. emergingthreats.net</a></li>
<li><a href="#sec-1-1-11">1.1.11. feodotracker.abuse.ch</a></li>
<li><a href="#sec-1-1-12">1.1.12. malc0de.com</a></li>
<li><a href="#sec-1-1-13">1.1.13. mirc.com</a></li>
<li><a href="#sec-1-1-14">1.1.14. netlab.360.com</a></li>
<li><a href="#sec-1-1-15">1.1.15. nothink.org</a></li>
<li><a href="#sec-1-1-16">1.1.16. openphish.com</a></li>
<li><a href="#sec-1-1-17">1.1.17. packetmail.net</a></li>
<li><a href="#sec-1-1-18">1.1.18. phishtank.com</a></li>
<li><a href="#sec-1-1-19">1.1.19. ransomware.abuse.ch</a></li>
<li><a href="#sec-1-1-20">1.1.20. isc.sans.edu</a></li>
<li><a href="#sec-1-1-21">1.1.21. spamhaus.org</a></li>
<li><a href="#sec-1-1-22">1.1.22. sslbl.abuse.ch</a></li>
<li><a href="#sec-1-1-23">1.1.23. vxvault.net</a></li>
<li><a href="#sec-1-1-24">1.1.24. zeustracker.abuse.ch</a></li>
</ul>
</li>
<li><a href="#sec-1-2">1.2. CIF</a>
<ul>
<li><a href="#sec-1-2-1">1.2.1. Bearded-Avenger install</a></li>
<li><a href="#sec-1-2-2">1.2.2. csirtg-smrt-py</a></li>
<li><a href="#sec-1-2-3">1.2.3. source list use</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</div>
</div>

# Threat Intelligence<a id="sec-1" name="sec-1"></a>

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="left" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="left" />

<col  class="right" />

<col  class="right" />

<col  class="left" />

<col  class="left" />

<col  class="left" />

<col  class="left" />

<col  class="left" />

<col  class="right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="left">&#xa0;</th>
<th scope="col" class="right">scanner</th>
<th scope="col" class="right">spam</th>
<th scope="col" class="right">botnet</th>
<th scope="col" class="right">malware</th>
<th scope="col" class="left">phishing</th>
<th scope="col" class="right">whitelist</th>
<th scope="col" class="right">darknet</th>
<th scope="col" class="left">exploit</th>
<th scope="col" class="left">honeypot</th>
<th scope="col" class="left">hijacked</th>
<th scope="col" class="left">suspicious</th>
<th scope="col" class="left">data<sub>type</sub></th>
<th scope="col" class="right">sum</th>
</tr>
</thead>

<tbody>
<tr>
<td class="left">alexa.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">5</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">URL</td>
<td class="right">1529</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">reputation.alienvault.com</td>
<td class="right">7</td>
<td class="right">6</td>
<td class="right">&#xa0;</td>
<td class="right">6</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">31978</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">osint.bambenekconsulting.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">9</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">865311</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">blocklist.de</td>
<td class="right">7</td>
<td class="right">&#xa0;</td>
<td class="right">7</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">68711</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">umbrella.cisco.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">5</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">1134</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">csirtg.io</td>
<td class="right">9</td>
<td class="right">9</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">9</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">IP,URL,</td>
<td class="right">1037</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">danger.rulez.sk</td>
<td class="right">9</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">1254</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">dataplane.org</td>
<td class="right">9</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">46710</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">emergingthreats.net</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">8</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">1289</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">feodotracker.abuse.ch</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">8</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">URL ,IP</td>
<td class="right">903</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">malc0de.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">9</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">URL,IP,MD5</td>
<td class="right">0</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">mirc.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">8</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">URL</td>
<td class="right">191</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">netlab.360.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">7</td>
<td class="right">7</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">7</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">889955</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">nothink.org</td>
<td class="right">7</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">193</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">openphish.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">9</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">URL</td>
<td class="right">5352</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">packetmail.net</td>
<td class="right">8</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">8</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">16424</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">phishtank.com</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">9</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">27128</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">ransomware.abuse.ch</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">9</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">12850</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">isc.sans.edu</td>
<td class="right">8</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">7-9</td>
<td class="left">&#xa0;</td>
<td class="right">0</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">spamhaus.org</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">9</td>
<td class="left">&#xa0;</td>
<td class="left">ASN,IPv6,Network</td>
<td class="right">1241</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">sslbl.abuse.ch</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">10</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">2384</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">vxvault.net</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">9</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">196</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="left">zeustracker.abuse.ch</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">9</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">MD5 ,URL ,IP</td>
<td class="right">673</td>
</tr>
</tbody>
</table>

## source introduction<a id="sec-1-1" name="sec-1-1"></a>

-   tags :

<p class="verse">
scanner: reputation.alienvault.com<br  />
spam: reputation.alienvault.com<br  />
botnet:<br  />
exploit:<br  />
malware: reputation.alienvault.com<br  />
phishing:<br  />
whitelist: alexa.com<br  />
suspicious:<br  />
feodo:<br  />
gozi:<br  />
hijacked:<br  />
rdata:<br  />
search:<br  />
zeus:<br  />
dga:<br  />
<br  />
</p>

-   confidence

<p class="verse">
(9-10）Certain<br  />
(7-8) Very Confident<br  />
(6-7) Somewhat Confident<br  />
(5-6) Not Confident<br  />
(5) "50/50 shot"<br  />
(0-4) Informational Data<br  />
</p>

### source add<a id="sec-1-1-1" name="sec-1-1-1"></a>

1.  spamhaustech
    <https://www.spamhaustech.com/protecting-mail-streams/>
2.  abusix
    <https://www.abusix.com/>
3.  apwg.org
    <https://apwg.org/>
    2003年创建的国际跨行业情报联盟 出网络钓鱼的报告可供下载
    
    没找到feed源
    
    提供数据分享的方式 <https://sourceforge.net/projects/ecrisp-x/>
4.  <http://txt.proxyspy.net/proxy.txt>

### alexa.com<a id="sec-1-1-2" name="sec-1-1-2"></a>

亚马逊的alexa提供站点排名
sum：1529

1.  top-1000

    -   tags: whitelist
    -   confidence ：5
    -   source url : <http://s3.amazonaws.com/alexa-static/top-1m.csv.zip>
    -   total : 1529
    -   cycle : 1 day
    -   incremental : 100+ /day
    
        {
        "_id" : ObjectId("593ba272256c1046ad056f91"),
        "confidence" : 5,
        "count" : 1,
        "description" : "alexa #972",//站点排名
        "group" : "everyone",
        "indicator" : "11st.co.kr", //域名信息
        "lasttime" : "",
        "provider" : "alexa.com",
        "rdata" : "",
        "tags" : "whitelist",
        "tlp" : "green"
        }

### reputation.alienvault.com<a id="sec-1-1-3" name="sec-1-1-3"></a>

[alienvault-labs](https://www.alienvault.com/who-we-are/alienvault-labs) 实验室每天扫描获取全球的威胁与漏洞,付费产品每三十分钟更新一次数据
产品提供14天免费试用
Unified Security Management™ Simplifies Security in the Cloud & On-Premises
AlienVault unifies all of your essential security tools in one location and combines them with real-time threat intelligence.
数据源文件包过大爬去下载失败
sum: 31978

1.  scanners

    -   tags: scanner
    -   confidence ：7
    -   source url : <https://reputation.alienvault.com/reputation.data>
    -   total : 0
    -   cycle : 1 day
    -   incremental : 0 /day

2.  spammers

    -   tags: spam
    -   confidence ：6
    -   source url : <https://reputation.alienvault.com/reputation.data>
    -   total : 0
    -   cycle : 1 day
    -   incremental : 0 /day

3.  malware

    -   tags: malware/suspicious
    -   confidence ：6
    -   source url : <https://reputation.alienvault.com/reputation.data>
    -   total : 0
    -   cycle : 1 day
    -   incremental : 0 /day

### osint.bambenekconsulting.com<a id="sec-1-1-4" name="sec-1-1-4"></a>

数据源爬去规则过老，需要修改规则或者重写爬虫
目前库内只有7w
C&C 被规整到了botnet内
<http://osint.bambenekconsulting.com/feeds/c2-dommasterlist.txt>

sum: 865311

1.  cryptolocker<sub>fqdn</sub>

    -   tags: botnet
    -   confidence ：9
    -   source url : <http://osint.bambenekconsulting.com/feeds/dga-feed.txt>
    -   total : 6000
    -   cycle : 1 day
    -   incremental : - /day

2.  zeus<sub>fqdn</sub>

    -   tags: botnet
    -   confidence ：9
    -   source url : <http://osint.bambenekconsulting.com/feeds/dga-feed.txt>
    -   total : 2000
    -   cycle : 1 day
    -   incremental : - /day

3.  tinba<sub>fqdn</sub>

    -   tags: botnet
    -   confidence ：9
    -   source url : <http://osint.bambenekconsulting.com/feeds/dga-feed.txt>
    -   total : 13w
    -   cycle : 1 day
    -   incremental : - /day
    
        {
        "_id" : ObjectId("593be9091d41c83f6aa07ba9"),
        "count" : 1,
        "indicator" : "209.15.13.134",
        "tlp" : "white",
        "group" : "everyone",
        "description" : "suppobox c&c",
        "tags" : "botnet",
        "rdata" : "",
        "confidence" : 6.5,
        "provider" : "osint.bambenekconsulting.com",
        "lasttime" : "2017-06-10T00:11:00.000000Z"
        }

### blocklist.de<a id="sec-1-1-5" name="sec-1-1-5"></a>

数据源提供 botnet scanner 数据
扫描数据扫描端口
sum : 68711

1.  scanner

    -   tags: scanner
    -   confidence ：7
    -   source url : 
        1.  <http://lists.blocklist.de/lists/ssh.txt>
        2.  <http://lists.blocklist.de/lists/mail.txt>
        3.  <http://lists.blocklist.de/lists/apache.txt>
        4.  <http://lists.blocklist.de/lists/imap.txt>
        5.  <http://lists.blocklist.de/lists/ftp.txt>
        6.  <http://lists.blocklist.de/lists/sip.txt>
        7.  <http://lists.blocklist.de/lists/bruteforcelogin.txt>
    -   total : -
    -   cycle : 1 day
    -   incremental : - /day

2.  botnet

    -   tags: scanner
    -   confidence ：7
    -   source url : <http://lists.blocklist.de/lists/bots.txt>
    -   total : -
    -   cycle : 1 day
    -   incremental : - /day
    
        {
        "_id" : ObjectId("593be9071d41c83f53a07bd4"),
        "confidence" : 7,
        "count" : 1,
        "description" : "",
        "group" : "everyone",
        "indicator" : "5.189.168.152",
        "lasttime" : "",
        "provider" : "blocklist.de",
        "rdata" : "",
        "tags" : "scanner",
        "tlp" : "green"
        }

### umbrella.cisco.com<a id="sec-1-1-6" name="sec-1-1-6"></a>

一级域名
sum：1134

1.  top-1000

    -   tags: whitelist
    -   confidence ：5
    -   source url : <http://s3-us-west-1.amazonaws.com/umbrella-static/top-1m.csv.zip>
    -   total : 1134
    -   cycle : 1 day
    -   incremental : 100+ /day
    
        {
        "_id" : ObjectId("593be90a1d41c83fa8a07c1b"),
        "confidence" : 5,
        "count" : 1,
        "description" : "cisco umbrella #401",
        "group" : "everyone",
        "indicator" : "t.co",
        "lasttime" : "",
        "provider" : "umbrella.cisco.com",
        "rdata" : "",
        "tags" : "whitelist",
        "tlp" : "green"
        }

### csirtg.io<a id="sec-1-1-7" name="sec-1-1-7"></a>

Unsolicited Commercial Email(UCE)商业垃圾邮件
<https://csirtg.io/users/csirtgadgets/feeds/uce-urls>
feed有限制250条 需要继续观察数据量
sum: 1037

1.  scanner

    -   tags: scanner
    -   confidence ：9
    -   source url : <https://csirtg.io/api/users/csirtgadgets/feeds/port-scanners.csv>
    -   total : -
    -   cycle : 1 day
    -   incremental :  /day

2.  uce

    -   tags: spam
    -   confidence ：9
    -   source url : 
        1.  <https://csirtg.io/api/users/csirtgadgets/feeds/uce-urls.csv>
        2.  <https://csirtg.io/api/users/csirtgadgets/feeds/uce-email-addresses.csv>
        3.  <https://csirtg.io/api/users/csirtgadgets/feeds/uce-ip.csv>
    -   total : -
    -   cycle : 1 day
    -   incremental :  /day

3.  darknet

    -   tags: darknet
    -   confidence ：9
    -   source url :<https://csirtg.io/api/users/wes/feeds/darknet.csv>
    -   total : -
    -   cycle : 1 day
    -   incremental :  /day

### danger.rulez.sk<a id="sec-1-1-8" name="sec-1-1-8"></a>

sum : 1254

1.  scanner

    -   tags: scanner
    -   confidence ：9
    -   source url :<http://danger.rulez.sk/projects/bruteforceblocker/blist.php>
    -   total : 1254
    -   cycle : 1 day
    -   incremental :  /day

### dataplane.org<a id="sec-1-1-9" name="sec-1-1-9"></a>

sum : 46710

1.  scanner

    -   tags: scanner
    -   confidence ：9
    -   source url :
        1.  <https://dataplane.org/sshclient.txt>
        2.  <https://dataplane.org/sshpwauth.txt>
        3.  <https://dataplane.org/sipquery.txt>
        4.  <https://dataplane.org/sipinvitation.txt>
        5.  <https://dataplane.org/sipregistration.txt>
    -   total : 1254
    -   cycle : 1 day
    -   incremental :  /day

### emergingthreats.net<a id="sec-1-1-10" name="sec-1-1-10"></a>

sum: 1289

1.  compromised-ips

    -   tags: scanner
    -   confidence ：8
    -   source url :<http://rules.emergingthreats.net/blockrules/compromised-ips.txt>
    -   total : 1254
    -   cycle : 1 day
    -   incremental :  /day

2.  

### feodotracker.abuse.ch<a id="sec-1-1-11" name="sec-1-1-11"></a>

sum : 903

1.  botnet

    -   tags: botnet
    -   confidence ：6-8
    -   source url :
        1.  <https://feodotracker.abuse.ch/blocklist/?download=domainblocklist> 8 domain
        2.  <https://feodotracker.abuse.ch/blocklist/?download=ipblocklist>  6 ip
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### malc0de.com<a id="sec-1-1-12" name="sec-1-1-12"></a>

提取代码出现问题
sum : 0

1.  malware

    -   tags: malware
    -   confidence ：9
    -   source url :<http://malc0de.com/rss/>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### mirc.com<a id="sec-1-1-13" name="sec-1-1-13"></a>

sum : 191

1.  domains

    -   tags: whitelist
    -   confidence ：8
    -   source url :<http://www.mirc.com/servers.ini>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### netlab.360.com<a id="sec-1-1-14" name="sec-1-1-14"></a>

Domain generation algorithms (DGA)
botnet 和 C&C 放在一起了

1.  exploit malware

    -   tags:exploit malware
    -   confidence ：7
    -   source url :<http://data.netlab.360.com/feeds/ek/magnitude.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

2.  botnet

    -   tags:botnet
    -   confidence ：7
    -   source url :
        <http://data.netlab.360.com/feeds/dga/bamital.txt>
        <http://data.netlab.360.com/feeds/dga/banjori.txt>
        <http://data.netlab.360.com/feeds/dga/banjori.txt>
        <http://data.netlab.360.com/feeds/dga/chinad.txt>
        <http://data.netlab.360.com/feeds/dga/conficker.txt>
        <http://data.netlab.360.com/feeds/dga/cryptolocker.txt>
        <http://data.netlab.360.com/feeds/dga/dircrypt.txt>
        <http://data.netlab.360.com/feeds/dga/dyre.txt>
        <http://data.netlab.360.com/feeds/dga/fobber.txt>
        <http://data.netlab.360.com/feeds/dga/gameover.txt>
        <http://data.netlab.360.com/feeds/dga/gspy.txt>
        <http://data.netlab.360.com/feeds/dga/locky.txt>
        <http://data.netlab.360.com/feeds/dga/madmax.txt>
        <http://data.netlab.360.com/feeds/dga/mirai.txt>
        <http://data.netlab.360.com/feeds/dga/murofet.txt>
        <http://data.netlab.360.com/feeds/dga/necurs.txt>
        <http://data.netlab.360.com/feeds/dga/nymaim.txt>
        <http://data.netlab.360.com/feeds/dga/proslikefan.txt>
        <http://data.netlab.360.com/feeds/dga/pykspa.txt>
        <http://data.netlab.360.com/feeds/dga/qadars.txt>
        <http://data.netlab.360.com/feeds/dga/ranbyus.txt>
        <http://data.netlab.360.com/feeds/dga/rovnix.txt>
        <http://data.netlab.360.com/feeds/dga/shifu.txt>
        <http://data.netlab.360.com/feeds/dga/simda.txt>
        <http://data.netlab.360.com/feeds/dga/suppobox.txt>
        <http://data.netlab.360.com/feeds/dga/symmi.txt>
        <http://data.netlab.360.com/feeds/dga/tempedreve.txt>
        <http://data.netlab.360.com/feeds/dga/tinba.txt>
        <http://data.netlab.360.com/feeds/dga/tofsee.txt>
        <http://data.netlab.360.com/feeds/dga/vawtrak.txt>
        <http://data.netlab.360.com/feeds/dga/vidro.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### nothink.org<a id="sec-1-1-15" name="sec-1-1-15"></a>

1.  scanner

    -   tags:exploit malware
    -   confidence ：7
    -   source url :<http://www.nothink.org/blacklist/blacklist_ssh_day.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### openphish.com<a id="sec-1-1-16" name="sec-1-1-16"></a>

1.  phishing

    -   tags:phishing
    -   confidence ：9
    -   source url :<https://openphish.com/feed.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### packetmail.net<a id="sec-1-1-17" name="sec-1-1-17"></a>

1.  scanner honeynet

    -   tags: honeynet
    -   confidence ：8
    -   source url :
        1.  <https://www.packetmail.net/iprep.txt>
        2.  <https://www.packetmail.net/iprep_mail.txt>
        3.  <https://www.packetmail.net/iprep_ramnode.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### phishtank.com<a id="sec-1-1-18" name="sec-1-1-18"></a>

1.  phishing

    -   tags:phishing
    -   confidence ：9
    -   source url : <http://data.phishtank.com/data/%7Btoken%7D/online-valid.json.gz>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### ransomware.abuse.ch<a id="sec-1-1-19" name="sec-1-1-19"></a>

1.  botnet

    -   tags:botnet
    -   confidence ：9
    -   source url :<http://ransomwaretracker.abuse.ch/feeds/csv>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### isc.sans.edu<a id="sec-1-1-20" name="sec-1-1-20"></a>

1.  scanner

    -   tags: scanner
    -   confidence ：7-9
    -   source url :
        1.  <https://isc.sans.edu/feeds/suspiciousdomains_Low.txt>
        2.  <https://isc.sans.edu/feeds/suspiciousdomains_High.txt>
        3.  <https://isc.sans.edu/feeds/suspiciousdomains_Medium.txt>
        4.  <https://isc.sans.edu/feeds/block.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### spamhaus.org<a id="sec-1-1-21" name="sec-1-1-21"></a>

1.  hijacked

    -   tags: hijacked
    -   confidence ：9
    -   source url :
        1.  <http://www.spamhaus.org/drop/drop.txt>
        2.  <http://www.spamhaus.org/drop/edrop.txt>
        3.  <https://www.spamhaus.org/drop/dropv6.txt>
        4.  <https://www.spamhaus.org/drop/asndrop.txt>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### sslbl.abuse.ch<a id="sec-1-1-22" name="sec-1-1-22"></a>

1.  botnet

    -   tags: botnet
    -   confidence ：10
    -   source url :
        1.  <https://sslbl.abuse.ch/blacklist/sslipblacklist.csv>
        2.  <https://sslbl.abuse.ch/blacklist/dyre_sslipblacklist.csv>
        3.  <https://sslbl.abuse.ch/blacklist/sslblacklist.csv>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### vxvault.net<a id="sec-1-1-23" name="sec-1-1-23"></a>

爬虫有问题

1.  malware

    -   tags: botnet
    -   confidence ：10
    -   source url :<http://vxvault.net/URL_List.php>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

### zeustracker.abuse.ch<a id="sec-1-1-24" name="sec-1-1-24"></a>

1.  malware

    -   tags: botnet
    -   confidence ：9
    -   source url :
        <http://zeustracker.abuse.ch/monitor.php?urlfeed=configs>
        <http://zeustracker.abuse.ch/monitor.php?urlfeed=configs>
        <http://zeustracker.abuse.ch/monitor.php?urlfeed=dropzones>
        <http://zeustracker.abuse.ch/blocklist.php?download=domainblocklist>
        <http://zeustracker.abuse.ch/blocklist.php?download=ipblocklist>
    -   total :
    -   cycle : 1 day
    -   incremental :  /day

## CIF<a id="sec-1-2" name="sec-1-2"></a>

### Bearded-Avenger install<a id="sec-1-2-1" name="sec-1-2-1"></a>

[Collective Intelligence Framework](http://csirtgadgets.org/collective-intelligence-framework/):
CIF是网络威胁情报管理系统，一个开源的框架，能帮助我们解析:规范化:存储:查询:共享和生成

威胁情报的数据集。最主要的情报形式是：IP:Domain:URL

![img](//7xpyfe.com1.z0.glb.clouddn.com/blog/20170606/160335989.png)

情报收集框架包括：
-   CIF Client
-   CIF-Router
-   CIF-Smrt
-   CIF-Tokens
-   CIF-Worker

[CIF Architecture Overview:](https://github.com/csirtgadgets/massive-octo-spice/wiki/CIF-Architecture-Overview)

<p class="verse">
CIF 设计框架介绍<br  />
How CIF fetches, parses and normalizes data<br  />
How CIF post-processes data<br  />
How CIF stores data<br  />
How the CIF API allows data to be queried and submitted<br  />
How CIF permissions data<br  />
How CIF produces feeds of data<br  />
</p>

[Bearded-Avenger](https://github.com/csirtgadgets/bearded-avenger-deploymentkit/wiki):
作为CIF的替代品，bearde-Avenger 安装很容易

<p class="verse">
$ tar -zxvf bearded-avenger-deploymentkit-3.0.x.tar.gz<br  />
$ cd bearded-avenger-deploymentkit-3.0.x<br  />
$ sudo bash easybutton.sh<br  />
</p>

ubuntu14.04正常安装报错，折腾了半天没时间搞了，官方提供Docker install

<p class="verse">
$ docker pull csirtgadgets/cif:latest<br  />
$ docker run &#x2013;name cif -d -p 5000:5000 csirtgadgets/cif<br  />
$ docker ps<br  />
$ docker exec -it 9121af6cabed /bin/bash<br  />
</p>

执行cif命令报下面的错误

    root@9121af6cabed:/bearded-avenger-3.0.0a13# cif --tags malware --limit 5
    Unable to read /root/.cif.yml config file

先读取cif.yml

    CONFIG_PATH = os.environ.get('CIF_CONFIG_PATH', os.path.join(os.getcwd(), 'cif.yml'))
    if not os.path.isfile(CONFIG_PATH):
        CONFIG_PATH = os.path.join(os.path.expanduser('~'), '.cif.yml')

查看README.md 执行下面语句 CIFv3并不需要参考[文档](https://github.com/csirtgadgets/bearded-avenger-deploymentkit/wiki/Docker) 中所说的创建/root/.cif.yml文件 

<p class="verse">
$ mkdir -p log && cp hacking/develop.conf hacking/local.conf<br  />
$ cif-store -d &#x2013;token-create-admin cif.yml<br  />
$ cif-store -d &#x2013;token-create-hunter cif-router.yml<br  />
$ cif-store -d &#x2013;token-create-smrt csirtg-smrt.yml<br  />
</p>

执行后还是不能使用 官方docker源很坑

docker search cif 找到了 ventz/cif 可以使用，但是安装后发现系统过于庞大

对于我只想使用smrt抓取数据的来说，我更需要cif-smrt功能，好在官方把这部分

功能提取出来了[csirtg-smrt-py](https://github.com/csirtgadgets/csirtg-smrt-py) 项目

### csirtg-smrt-py<a id="sec-1-2-2" name="sec-1-2-2"></a>

使用YAML来规范数据，爬取feed数据源

sudo pip install csirtg-smrt
![img](//7xpyfe.com1.z0.glb.clouddn.com/blog/20170608/144738024.png)

测试了几个数据源如果feed为zip的压缩包，网络不是很顺畅的情况下无法正常下载爬取数据

总的来说CIF不是很稳定，也不太适合我们公司情报收集，但是[数据源](https://github.com/csirtgadgets/bearded-avenger/tree/master/rules) 可以作为扩充

下载github project中的单个目录 可以通过[DownGit](https://github.com/MinhasKamal/DownGit) 创建下载链接

### source list use<a id="sec-1-2-3" name="sec-1-2-3"></a>

利用pyyaml解析yml

sudo pip install pyyaml

使用官方提供的yml配置文件定时抓取feed数据

脚本每小时跑一遍
代码如下：[github](https://github.com/Nanue1/csirtg-smrt/blob/master/smrt.py)

    import yaml
    import time
    import json
    import os
    import sys
    import logging
    import requests
    import traceback
    import subprocess
    import pymongo
    from multiprocessing import Process,Queue,Value
    
    
    CONF_PATH = os.path.abspath('.')+"/rule"
    log_xpath="/tmp/%s.log" % os.path.basename(__file__)
    PROCESS_NUM = 200
    
    
    def init_log(log_xpath):
        logging.basicConfig(level=logging.DEBUG,
                    format='%(asctime)s %(filename)s[line:%(lineno)d] %(levelname)s %(message)s',
                    datefmt='%Y %b %d %H:%M:%S',
                    filename=log_xpath,
                    filemode='w')
    
    def bulk_upsert_mongo(arg_list,coll):
        for dict_data in arg_list:
            #coll.update({"indicator":dict_data["indicator"]},{"$set":{"count":dict_data["count"],"tlp":dict_data["tlp"],"group":dict_data["group"],"description":dict_data["description"],"tags":dict_data["tags"],"rdata":dict_data["rdata"],"confidence":dict_data["confidence"],"provider":dict_data["provider"],"lasttime":dict_data["lasttime"]}},upsert=True)
            coll.insert(dict_data)
            #logging.info('insert %s' % dict_data["indicator"] )
    
    
    def cmd_exc(flag):
        conn=pymongo.MongoClient('Mongo_IP',27017)
        db=conn["threat_cif"]
        coll=db["smrt"]
        while True:
            if cmds_queue.empty() and flag.value==1: 
                break
            else:
                try:
                    cmd_smrt= cmds_queue.get(timeout=8)
                    p = subprocess.Popen(cmd_smrt, shell=True,stdout=subprocess.PIPE)
                    p.wait()
                    time.sleep(10)
                    logging.info('%s status: %s' % (cmd_smrt,p.poll()))
                    if p.poll() == 0:
                        content= json.loads(p.stdout.read())
                        bulk_upsert_mongo(content,coll)
                    elif p.poll() is  None:
                        p.kill()
                        logging.error('%s  returncode: %s timeout over 10s' % (cmd_smrt,p.returncode))
                    else:
                        logging.error('%s status:%s, returncode: %s' % (cmd_smrt,p.poll(),p.returncode))
                except:
                    logging.info(traceback.format_exc().splitlines())
                    pass
        sys.exit()
    
    def parse_yml():
        for yml_name in os.listdir(CONF_PATH): 
            if yml_name.endswith(".yml"):
                dic_yml = yaml.load(open(yml_name))['feeds']
                for key in dic_yml :
                    cmd_smrt = "/usr/local/bin/csirtg-smrt -r " + yml_name + " -f " + key + " --format json"
                    cmds_queue.put(cmd_smrt)
    
    def run():
        end_flag = Value('i', 0)
        ps = [Process(target=cmd_exc,args=(end_flag,)) for x in xrange(PROCESS_NUM)]
        for p in ps:
            p.start()
        parse_yml()
        end_flag.value = 1
        for p in ps:
            p.join()
    
    if '__main__' == __name__:
        if not os.path.exists(CONF_PATH):
            print "conf file not exists"
            sys.exit()
        else:
            os.system("rm -rf /tmp/smrt/")
            os.chdir(CONF_PATH)
        init_log(log_xpath)
        cmds_queue = Queue(100)
        session = requests.Session()
        run()