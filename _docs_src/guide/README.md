---
sidebar: auto
---

# 指南
## 介绍
Stream Downloader是一个以NodeJs驱动的网络媒体资源下载工具，为了支持更方便地从网络下载公开资源而创建并开源的。
当你浏览网页发现一个有趣的资源时，你就可以使用它下载该资源以用于学习和研究。

### 特性
### 路线图
## 起步
### 安装
#### npm安装

```sh
npm install -g stream-downloader
```
使用上面的命令安装好后，即可使用`stream-downloader`或者`stream-dl`命令了
```sh
## 查看命令帮助
stream-dl -h
```
#### 二进制文件

|  操作系统  |         二进制包          |
| :----: | :-------------------: |
| winx64 |   [stream-downloader-winx64-v0.0.16](https://github.com/lunnlew/stream-downloader/releases/download/v0.0.16/stream-downloader-winx64.exe)   |

### 使用
当你想下载某个站点页面的视频时,可以使用如下的方式

```sh
stream-dl 'https://v.qq.com/x/cover/mzc00200f995x6t/b0032n9h1lp.html'
```
结果

	$ stream-dl 'https://v.qq.com/x/cover/mzc00200f995x6t/b0032n9h1lp.html'
	stream-downloader - One stream downloader
	debug: urls total 1
	debug: matching video info
	debug: Requesting https://v.qq.com/x/cover/mzc00200f995x6t/b0032n9h1lp.html
	debug: vid b0032n9h1lp
	debug: title 外交风云_05
	debug: matching video completed
	================================================
	-- title:外交风云_05
	-- url:https://v.qq.com/x/cover/mzc00200f995x6t/b0032n9h1lp.html
	debug: auto selected SD
	================================================
	Downloading streaming content with Request, press ctrl + c to stop recording...
	debug: will downloading 1,2,3,4,5,6,7,8,9
	debug: downloading url http://211.162.173.149/vlive.qqvideo.tc.qq.com/AeXmx_Lyf8NTKyranHW63b0gcNIqVYyXRNquS1JVP524/uwMROfz2r5zAoaQXGdGnC2dfKb8lyKS1sskNZcPDHZeE8qgJ/l00326604nv.p203.1.mp4?vkey=FD7D16544575547CAAB0AD8A13714F3CE9F237F177A52FC76FCB9FFA1226C6567AA28553FDE74B25EEBDFEC581D1E09F61537ACA7C2845A426633DECAB8088FF45FA8F9A277229D6F59FCF172F411CCA6A5B490888B0EA4AC1A7D27671F221B954631CB2B2E01D8ABF2E4BFE4ED973BA
	debug: statusCode 200 contentType video/mp4
	process: totalSize=14.28MB receivedSize=14.28MB percentage=100%
	........
	........
	debug: downloading url http://211.162.173.149/vlive.qqvideo.tc.qq.com/AeXmx_Lyf8NTKyranHW63b0gcNIqVYyXRNquS1JVP524/uwMROfz2r5zAoaQXGdGnC2dfKb8lyKS1sskNZcPDHZeE8qgJ/l00326604nv.p203.9.mp4?vkey=DB74F3326CCEC3AE09D4B2C7AE1B4A179229A54E25E77884C9390CAD4E01A408FBCF8F739A3CD2606DA8403D8A6A99AB23D861B670CFE1DCF330FA260168CAFC68B221920A14ED51BF3C1DA17412F2F41B13A8ADF5AF726280167ED7678F697D889E7DF8DE08D4DB9BA1C6A18074865D
	debug: statusCode 200 contentType video/mp4
	process: totalSize=10.35MB receivedSize=10.35MB percentage=100%
	debug: downloaded result true
	debug: ffmpegPath bin\ffmpeg.exe
	debug: starting merge video
	debug: Ffmpeg with command: ffmpeg -i concat:300ffa1f9cef71781b6fdfa78a0740cb/1.mp4.ts|....|300ffa1f9cef71781b6fdfa78a0740cb/9.mp4.ts -y -c copy -bsf:a aac_adtstoasc 外交风云_05.mp4
	debug: merge completed

## 进阶

## 限制
当前，不支持`加密的媒体片段`，例如drm加密版权视频等。

## 技术栈

## 开源许可
基于 [MIT license](https://opensource.org/licenses/MIT) 许可进行开源。