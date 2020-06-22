# Ladon for Cobalt Strike
![](https://k8gege.github.io/k8img/Ladon/Dragon.jpg)

[![Author](https://img.shields.io/badge/Author-k8gege-blueviolet)](https://github.com/k8gege) 
[![Ladon](https://img.shields.io/badge/Ladon-6.6-yellowgreen)](https://github.com/k8gege/Ladon) 
[![Bin](https://img.shields.io/badge/Ladon-Bin-ff69b4)](https://github.com/k8gege/Ladon/releases) 
[![GitHub issues](https://img.shields.io/github/issues/k8gege/Ladon)](https://github.com/k8gege/Ladon/issues) 
[![Github Stars](https://img.shields.io/github/stars/k8gege/Ladon)](https://github.com/k8gege/Ladon) 
[![GitHub forks](https://img.shields.io/github/forks/k8gege/Ladon)](https://github.com/k8gege/Ladon)
[![GitHub license](https://img.shields.io/github/license/k8gege/Ladon)](https://github.com/k8gege/Ladon)

### Cobalt Strike
<img src=https://k8gege.github.io/k8img/Ladon/CS_Ladon.gif></img>

### 程序简介

Ladon一款用于大型网络渗透的多线程插件化综合扫描神器，含端口扫描、服务识别、网络资产、密码爆破、高危漏洞检测以及一键GetShell，支持批量A段/B段/C段以及跨网段扫描，支持URL、主机、域名列表扫描。6.6版本内置74个功能模块,外部模块17个,通过多种协议以及方法快速获取目标网络存活主机IP、计算机名、工作组、共享资源、网卡地址、操作系统版本、网站、子域名、中间件、开放服务、路由器、数据库等信息，漏洞检测包含MS17010、SMBGhost、Weblogic、ActiveMQ、Tomcat、Struts2系列等，密码爆破12种含数据库(Mysql、Oracle、MSSQL)、FTP、SSH、VNC、Windows(LDAP、SMB/IPC、WMI、SmbHash、WmiHash、Winrm)、BasicAuth、Tomcat、Weblogic、Rar等，远程执行命令包含(wmiexe/psexec/atexec/sshexec/jspshell),Web指纹识别模块可识别75种（Web应用、中间件、脚本类型、页面类型）等，可高度自定义插件POC支持.NET程序集、DLL(C#/Delphi/VC)、PowerShell等语言编写的插件,支持通过配置INI批量调用任意外部程序或命令，EXP生成器可一键生成漏洞POC快速扩展扫描能力。Ladon支持Cobalt Strike插件化扫描快速拓展内网进行横向移动。

### 使用文档

ID | 主题 |  URL 
-|-|-
0 | Ladon文档主页 | https://k8gege.org/Ladon/
1 | Ladon基础文档 | http://k8gege.org/p/648af4b3.html
2 | Ladon用法例子 | http://k8gege.org/Ladon/example.html
3 | 基础用法详解 | https://github.com/k8gege/Ladon/wiki/Ladon-Usage
4 | Cobalt Strike | https://github.com/k8gege/Aggressor
5 | Exp生成器使用 | https://github.com/k8gege/Ladon/wiki/LadonExp-Usage
6 | 高度自定义插件 | https://github.com/k8gege/Ladon/wiki/Ladon-Diy-Moudle
7 | 外部模块参考 | https://github.com/k8gege/K8CScan/wiki
8 | PowerLadon | https://github.com/k8gege/powerladon
9 | PythonLadon | https://github.com/k8gege/PyLadon
10 | LinuxLadon | https://github.com/k8gege/KaliLadon
12 | 漏洞演示视频 | https://github.com/k8gege/K8CScan/tree/master/Video
13 | Ladon6.0文档 | http://k8gege.org/p/56393.html
14 | Ladon6.2文档 | http://k8gege.org/p/39070.html
13 | Ladon6.4文档 | http://k8gege.org/p/55476.html
16 | Ladon6.5文档 | http://k8gege.org/Ladon/WinShell.html

### DownLoad
New Version：https://k8gege.org/Download <br>
All Version: https://github.com/k8gege/Ladon/releases/


### 0.Cobalt Strike联动
![](https://github.com/k8gege/K8CScan/blob/master/Images/CobaltStrike.gif)
### 1.SmbScan MS17-010漏洞扫描
IP、SMB漏洞、机器名、操作系统版本<br>
![SmbScan](https://github.com/k8gege/K8CScan/blob/master/Images/MS17010.PNG)
### 2.OSscan 操作系统探测
通过SMB、多端口、Banner等方式探测（存活主机、主机名、域名、操作系统版本、开放服务等）<br>
![OSscan](https://github.com/k8gege/K8CScan/blob/master/Images/OSscan.PNG)
### 3.OnlinePC 存活主机扫描
也支持检测主机名/域名是否存活,结果IP、Mac、机器名<br>
![OnlinePC](https://github.com/k8gege/K8CScan/blob/master/Images/OnlinePC.PNG)
### 4.WebScan Web扫描
内网站点扫描，获取服务器Banner、网页标题<br>
![WebScan](https://github.com/k8gege/K8CScan/blob/master/Images/WebScan.PNG)
### 5.FtpScan FTP密码扫描
需上传user.txt和pass.txt至beacon工作目录<br>
![FtpScan](https://github.com/k8gege/K8CScan/blob/master/Images/FtpScan.PNG)
### 6.WmiScan Win方式爆破Windows密码（IPC被拒绝时可尝试WMI）
Wmi方式批量爆破内网主机帐密,需上传user.txt和pass.txt至工作目录<br>
![WmiScan](https://github.com/k8gege/K8CScan/blob/master/Images/WmiScan.PNG)
### 7.CiscoScan 思科设备扫描
(IP、设备型号、主机名、Boot、硬件版本)<br>
![CiscoScan](https://github.com/k8gege/K8CScan/blob/master/Images/CiscoScan.PNG)
### 8.UrlScan C段域名URL扫描
通过源码获取域名或URL，但不验证IP,适用于内网扫描时，目标域名指向外网IP<br>
或者通过域名判断内网站点是何产品，比如出现cisco.com域名，说明此为cisco设备<br>
![UrlScan](https://github.com/k8gege/K8CScan/blob/master/Images/UrlScan.PNG)
### 9.SameWeb C段旁站扫描
通过源码获取域名并验证IP，返回正确的同服站点,非bing或爱站等方式,即内网不可上网也可扫描<br>
验证IP主要适用于，外网扫描时旁站，因为获取的域名指向外网时，无法通过IP判断是否属于同服<br>
![SameWeb](https://github.com/k8gege/K8CScan/blob/master/Images/SameWeb.PNG)
### 10.WeblogicExp & WeblogicPoc
Weblogic漏洞扫描两个模块,一个是只扫描是否存在漏洞，另一个是扫描并且GetShell<br>
![WeblogicExp](https://github.com/k8gege/K8CScan/blob/master/Images/WeblogicExp.PNG)
### 11.EnumMSSQL 枚举局域网MS SQL SERVER数据库主机
和PowerUpSql一样不一定能获取到SQL版本
![](https://github.com/k8gege/K8CScan/blob/master/Images/EnumMSSQL.PNG)
### 12.EnumShare 枚举局域网共享资源
![](https://github.com/k8gege/K8CScan/blob/master/Images/EnumShare.PNG)
### 13.MssqlScan MSSQL数据库密码爆破
![](https://github.com/k8gege/K8CScan/blob/master/Images/MssqlScan.PNG)
### 14.MysqlScan MySQL数据库密码爆破
![](https://github.com/k8gege/K8CScan/blob/master/Images/MysqlScan.PNG)
### 15.SSHscan SSH主机密码爆破
![](https://github.com/k8gege/K8CScan/blob/master/Images/SSHscan.PNG)
### 16.OracleScan Oracle数据库密码爆破
![](https://github.com/k8gege/K8CScan/blob/master/Images/OracleScan.PNG)
### 17.HostIP 域名解析/主机名转IP
![](https://github.com/k8gege/K8CScan/blob/master/Images/HostIP.PNG)
### 18.WhatCMS 指纹识别支持62种CMS
url.txt指定站点或批量站点扫描,也可扫描整个C段部分web端口对应CMS
![](https://github.com/k8gege/K8CScan/blob/master/Images/WhatCMS.png)
### 19.IpcScan Windows密码爆破(Wmi被拒绝时可尝试Ipc)
![](https://github.com/k8gege/K8CScan/blob/master/Images/IpcScan.PNG)
### 20.WebScan2 Web信息扫描含CMS识别
url.txt指定站点或批量站点扫描,也可扫描整个C段中Web信息
![](https://github.com/k8gege/K8CScan/blob/master/Images/WebScan2.PNG)
### 21.EnBase64/DeBase64  Base64密码批量加密解密
![](https://github.com/k8gege/K8CScan/blob/master/Images/Base64.PNG)
### 22.EnHex/DeHex  Hex密码批量加密解密(3种格式)
![](https://github.com/k8gege/K8CScan/blob/master/Images/DeHex.PNG)
### 23.SmbScan Windows密码爆破(Wmi被拒绝时可尝试,记录错误日志)
![](https://github.com/k8gege/K8CScan/blob/master/Images/SmbScan.png)
### 24.PhpStudyPoc PhpStudy后门检测
![](https://github.com/k8gege/K8CScan/blob/master/Images/PhpStudyPoc.PNG)
### 25.DomainIP 域名解析
![](https://github.com/k8gege/K8CScan/blob/master/Images/DomainIP.gif)
### 26.SubDomain 子域名爆破
需域名字典SubDomain.dic<br>
例子: Cscan baidu.com SubDomain<br>
![](https://github.com/k8gege/K8CScan/blob/master/Images/SubDomain.gif)
### 27.WebDir Web目录扫描
![](https://github.com/k8gege/K8CScan/blob/master/Images/WebDir.PNG)
