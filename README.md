# 资源简介

基于Anki23.12.1和《标准日本语》制作的日语卡牌，含语法、短语和单词。
其中，日语声调来源于“[Moji辞书](https://www.mojidict.com/)”，部分释义、词性也参考了这个。
目前还在学习中，所以陆陆续续更新，这个更新日志就暂定保留最新5条吧，也当作自己的学习打卡记录了。

文章：https://zhuanlan.zhihu.com/p/682555712

# 用到的插件清单

+ 742319784（Reset Review Stats）：用于清空学习记录，主要用于调试卡牌，不太常用，可以只是用卡牌预览功能来测试卡牌功能。
+ 1344485230（AJT Japanese）：主要用于自动生成振假名（假名注音），可以节省一部分精力。
+ 1436550454（AwesomeTTS - Add speech to your flashcards）：主要用于根据单词、短语、句子生成mp3的朗读语音（TTS）。

## AJT Japanese补充说明

可以在AJT Japanese的Japanese Options中设置自动化操作，添加或使用一个现有配置，设置好卡牌、源字段、目标字段（可以和源字段一样，但是需要勾选“override destination”选项）等，录入卡片时，输入完成后通过tab键可以自动添加注音、发音等。

# 用到的脚本

## 服务器启动脚本

```bat
@echo off

set SYNC_USER1=user:pass
set SYNC_BASE=C:\Users\user\Dropbox\AnkiServer\
::set SYNC_PORT=8080
C:\Users\user\AppData\Local\Programs\Anki\anki.exe --syncserver
```

## 桌面客户端设置代理

```bat
@echo off

set "http_proxy=http://proxy_ip:65533"
set "https_proxy=http://proxy_ip:65534"

cd C:\Users\user\AppData\Local\Programs\Anki
anki.exe
```

# 更新记录

+ 第7次更新（20240302）：对单词、短语、语法增加一个名为“隐藏内容”的字段，为手工填写的日本汉字（即kanji，去掉假名注音后的部分），仅参与排序，不用于显示，便于搜索功能的使用。另外准备给单词另外增加一个“隐藏内容2”，用于保存手工填写的假名（即kana，去掉汉字部分的注音），仅用于纯假名搜索。目前正在探索相关的自动填充插件，有知道的可以告知！
+ 第8次更新（20240303）：更新了TTS单词发音，能用词典发音（由AJT Japanese插件提供）的均进行了替换（为了公平原则，有些感觉怪怪的也进行了替换，比如“<ruby>語<rt>ご</rt></ruby>”在xx语中大多读作了“mo”音，“<ruby>一人<rt>ひとり</rt></ruby><ruby>暮<rt>ぐ</rt></ruby>らし”中的“ひ”明显没有发音等）。补充了AJT插件说明。
+ 第9次更新（20240304）：S01E04后面的“家”相关单词已添加。
+ 第10次更新（20240308）：5、6号因故未能更新，7号更新，于8号凌晨提交，主要进度为S01E05的语法部分。
+ 地11次更新（20240308）：卡在语法部分了，“は”的“对比”用法没有学会，记录进度在“时刻”。

# TODO LIST

1. 补充S01E03中表示某某柜台的短语。
2. 补充完善“は”的“对比”用法。