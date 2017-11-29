---
title: 命令行 aria2 命令行下的下载神器
---

# 简介（Introduction）：
# 安装（Installation）：
主页:http://aria2.github.io/
# 快速上手（Getting Started）：
Download from WEB:
```bash
$ aria2c 'http://example.org/mylinux.iso'
```
Download from 2 sources:
```bash
$ aria2c 'http://a/f.iso' 'ftp://b/f.iso'
```
Download using 2 connections per host:
```bash
$ aria2c -x2 'http://a/f.iso'
```
BitTorrent:
```bash
$ aria2c 'http://example.org/mylinux.torrent'
```
BitTorrent Magnet URI:
```bash
$ aria2c 'magnet:?xt=urn:btih:248D0A1CD08284299DE78D5C1ED359BB46717D8C'
```
Metalink:
```bash
$ aria2c 'http://example.org/mylinux.metalink'
```
Download URIs found in text file:
```bash
$ aria2c -i uris.txt
```
# 进阶篇（Advanced)：
```bash
aria2c --enable-rpc --rpc-listen-all
```
webui-aria2: Web browser interface for aria2 (2012 GSOC project)
uGet: the Linux Download Manager

# API（Reference）：
- [open](#open)
- [close](#close)
- [onsend and onmessage](#onsend-and-onmessage)
- [aria2 methods](#aria2-methods)
    - [addUri](https://aria2.github.io/manual/en/html/aria2c.html#aria2.addUri)
    - [addTorrent](https://aria2.github.io/manual/en/html/aria2c.html#aria2.addTorrent)
    - [addMetaLink](https://aria2.github.io/manual/en/html/aria2c.html#aria2.addMetalink)
    - [remove](https://aria2.github.io/manual/en/html/aria2c.html#aria2.remove)
    - [forceRemove](https://aria2.github.io/manual/en/html/aria2c.html#aria2.forceRemove)
    - [pause](https://aria2.github.io/manual/en/html/aria2c.html#aria2.pause)
    - [pauseAll](https://aria2.github.io/manual/en/html/aria2c.html#aria2.pauseAll)
    - [forcePause](https://aria2.github.io/manual/en/html/aria2c.html#aria2.forcePause)
    - [forcePauseAll](https://aria2.github.io/manual/en/html/aria2c.html#aria2.forcePauseAll)
    - [unpause](https://aria2.github.io/manual/en/html/aria2c.html#aria2.unpause)
    - [unpauseAll](https://aria2.github.io/manual/en/html/aria2c.html#aria2.unpauseAll)
    - [tellStatus](https://aria2.github.io/manual/en/html/aria2c.html#aria2.tellStatus)
    - [getUris](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getUris)
    - [getFiles](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getFiles)
    - [getPeers](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getPeers)
    - [getServers](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getServers)
    - [tellActive](https://aria2.github.io/manual/en/html/aria2c.html#aria2.tellActive)
    - [tellWaiting](https://aria2.github.io/manual/en/html/aria2c.html#aria2.tellWaiting)
    - [tellStopped](https://aria2.github.io/manual/en/html/aria2c.html#aria2.tellStopped)
    - [changePosition](https://aria2.github.io/manual/en/html/aria2c.html#aria2.changePosition)
    - [changeUri](https://aria2.github.io/manual/en/html/aria2c.html#aria2.changeUri)
    - [getOption](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getOption)
    - [changeOption](https://aria2.github.io/manual/en/html/aria2c.html#aria2.changeOption)
    - [getGlobalOption](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getGlobalOption)
    - [changeGlobalOption](https://aria2.github.io/manual/en/html/aria2c.html#aria2.changeGlobalOption)
    - [getGlobalStat](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getGlobalStat)
    - [purgeDownloadResult](https://aria2.github.io/manual/en/html/aria2c.html#aria2.purgeDownloadResult)
    - [removeDownloadResult](https://aria2.github.io/manual/en/html/aria2c.html#aria2.removeDownloadResult)
    - [getVersion](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getVersion)
    - [getSessionInfo](https://aria2.github.io/manual/en/html/aria2c.html#aria2.getSessionInfo)
    - [shutdown](https://aria2.github.io/manual/en/html/aria2c.html#aria2.shutdown)
    - [forceShutdown](https://aria2.github.io/manual/en/html/aria2c.html#aria2.forceShutdown)
    - [saveSession](https://aria2.github.io/manual/en/html/aria2c.html#aria2.saveSession)
    - [system.multicall](https://aria2.github.io/manual/en/html/aria2c.html#system.multicall)
    - [system.listMethods](https://aria2.github.io/manual/en/html/aria2c.html#system.listMethods)
    - [system.listNotifications](https://aria2.github.io/manual/en/html/aria2c.html#system.listNotifications)
- [aria2 events](#aria2-events)
    - [onDownloadStart](https://aria2.github.io/manual/en/html/aria2c.html#aria2.onDownloadStart)
    - [onDownloadPause](https://aria2.github.io/manual/en/html/aria2c.html#aria2.onDownloadPause)
    - [onDownloadStop](https://aria2.github.io/manual/en/html/aria2c.html#aria2.onDownloadStop)
    - [onDownloadComplete](https://aria2.github.io/manual/en/html/aria2c.html#aria2.onDownloadComplete)
    - [onDownloadError](https://aria2.github.io/manual/en/html/aria2c.html#aria2.onDownloadError)
    - [onBtDownloadComplete](https://aria2.github.io/manual/en/html/aria2c.html#aria2.onBtDownloadComplete)
