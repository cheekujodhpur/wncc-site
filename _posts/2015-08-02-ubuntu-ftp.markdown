---
layout:     post
title:      "Ubuntu Repository Settings"
subtitle:   "How to use Ubuntu FTP repositories inside IITB"
date:       2015-08-02 17:34:00
author:     "Kumar Ayush"
header-img: ""
---

<p>After joining IIT, a vast majority shift to Ubuntu, Linux being a major requirement for a lot of projects and courses. But a few know that IITB happens to be one of three servers to maintain Ubuntu repositories across the nation, the other two being IITK and IITM. Thus, users on IITB network can use apt software repositories hosted on institute's ftp servers.</p>

<p>Follow the steps:<br />
<ul>
  <li>Make sure you have <b>no FTP proxy</b> in <b>/etc/apt/apt.conf</b> file.</li>
  <li>Make a backup of <b>/etc/apt/sources.list</b> if you want to.</li>
  <li>Open <b>Terminal</b></li>
  <li>Type and hit enter</li>
  <pre>sudo gedit /etc/apt/sources.list</pre>
  <li>A file will open in gedit. Replace all the contents by</li>
  <pre>##### Warning: Instead of maverick, use the name of your distribution in following lines

deb ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick main restricted
deb-src ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick main restricted

deb ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick-updates main restricted
deb-src ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick-updates main restricted

deb ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick universe
deb-src ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick universe
deb ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick-updates universe
deb-src ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick-updates universe

deb ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick multiverse
deb-src ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick multiverse
deb ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick-updates multiverse
deb-src ftp://ftp.iitb.ac.in/os/ubuntu/archives/ maverick-updates multiverse</pre>
  <li>Save the file.</li>
  <li>Run <b>sudo apt-get update</b> in Terminal. You are done.</li>
  <li>Now you can install softwares from IITB FTP repositories. THey are very fast as compared to HTTP repositories.
</ul></p>

<p>Reposted from <a href = "http://www.stab-iitb.org/wiki/Ubuntu_Repository_Settings">STAB Wiki</a></p>
