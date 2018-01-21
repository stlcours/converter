[TOC]

通过calibre将html转成epub、mobi、pdf等文档

## 安装calibre
- 下载地址：https://calibre-ebook.com/download
- 根据自己的系统安装对应的calibre（需要注意的是，calibre要安装3.x版本的，2.x版本的功能不是很强大。反正安装最新的准没错。）
- 安装完calibre之后，将calibre加入到系统的path中，执行下面的命令之后显示3.x的版本即表示安装成功。
```
ebook-convert --version
```
## 使用示例


## 配置文件

### json配置示例
```json
{
	"charset": "utf-8",
	"cover": "",
	"date": "2018-01-21",
	"description": "Gogs 的目标是打造一个最简单、最快速和最轻松的方式搭建自助 Git 服务。使用 Go 语言开发使得 Gogs 能够通过独立的二进制分发，并且支持 Go 语言支持的 所有平台，包括 Linux、Mac OS X、Windows 以及 ARM 平台。",
	"footer": "<p style='color:#8E8E8E;font-size:12px;'>本文档使用 <a href='http://www.bookstack.cn' style='text-decoration:none;color:#1abc9c;font-weight:bold;'>书栈(BookStack.CN)</a> 构建 <span style='float:right'>- _PAGENUM_ -</span></p>",
	"header": "<p style='color:#8E8E8E;font-size:12px;'>_SECTION_</p>",
	"identifier": "",
	"language": "zh-CN",
	"creator": "书栈(BookStack.CN)",
	"publisher": "书栈(BookStack.CN)",
	"contributor": "书栈(BookStack.CN)",
	"title": "Gogs中文文档",
	"format": ["epub", "mobi", "pdf"],
	"font_size": "14",
	"paper_size": "a4",
	"margin_left": "",
	"margin_right": "",
	"margin_top": "",
	"margin_bottom": "",
	"more": ["--pdf-page-margin-bottom", "72", "--pdf-page-margin-left", "72", "--pdf-page-margin-right", "72", "--pdf-page-margin-top", "72"],
	"toc": [{
		"id": 709800000,
		"link": "statement.html",
		"pid": 0,
		"title": "致谢"
	}, {
		"id": 539,
		"link": "539.html",
		"pid": 538,
		"title": "5.1 配置文件手册"
	}, {
		"id": 545,
		"link": "545.html",
		"pid": 543,
		"title": "4.1 自定义模板"
	}, {
		"id": 549,
		"link": "549.html",
		"pid": 548,
		"title": "2.1 注册 Windows 服务"
	}, {
		"id": 554,
		"link": "554.html",
		"pid": 0,
		"title": "1. 简介"
	}, {
		"id": 555,
		"link": "555.html",
		"pid": 554,
		"title": "1.1 变更日志"
	}, {
		"id": 540,
		"link": "540.html",
		"pid": 538,
		"title": "5.2 公告与高阶指南"
	}, {
		"id": 547,
		"link": "547.html",
		"pid": 543,
		"title": "4.2 Web 钩子"
	}, {
		"id": 548,
		"link": "548.html",
		"pid": 0,
		"title": "2. 下载安装"
	}, {
		"id": 556,
		"link": "556.html",
		"pid": 554,
		"title": "1.2 常见问题"
	}, {
		"id": 559,
		"link": "559.html",
		"pid": 558,
		"title": "3.1 二进制升级"
	}, {
		"id": 546,
		"link": "546.html",
		"pid": 543,
		"title": "4.3 多国语言支持"
	}, {
		"id": 550,
		"link": "550.html",
		"pid": 548,
		"title": "2.2 配置与运行"
	}, {
		"id": 557,
		"link": "557.html",
		"pid": 554,
		"title": "1.3 故障排查"
	}, {
		"id": 558,
		"link": "558.html",
		"pid": 0,
		"title": "3. 版本升级"
	}, {
		"id": 560,
		"link": "560.html",
		"pid": 558,
		"title": "3.2 源码升级"
	}, {
		"id": 543,
		"link": "543.html",
		"pid": 0,
		"title": "4. 功能介绍"
	}, {
		"id": 544,
		"link": "544.html",
		"pid": 543,
		"title": "4.4 授权认证"
	}, {
		"id": 551,
		"link": "551.html",
		"pid": 548,
		"title": "2.3 二进制安装"
	}, {
		"id": 538,
		"link": "538.html",
		"pid": 0,
		"title": "5. 高级用法"
	}, {
		"id": 552,
		"link": "552.html",
		"pid": 548,
		"title": "2.4 包管理安装"
	}, {
		"id": 542,
		"link": "542.html",
		"pid": 0,
		"title": "6. 捐赠我们"
	}, {
		"id": 553,
		"link": "553.html",
		"pid": 548,
		"title": "2.5 源码安装"
	}]
}
```

### json配置说明
1.  如果封面cover配置项为图片，则程序自动生成titlepage.xhtml文件；如果封面cover为html或者xhtml，则不会生成titlepage.xhtml.在处理的时候，判断cover前后是否相同再决定文件的删减
1.  文件名，统一用book.pdf、book.epub等标识

## 使用案例

## 精神上支持我