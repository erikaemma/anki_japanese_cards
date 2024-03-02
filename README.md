# 资源简介

基于Anki23.12.1和《标准日本语》制作的日语卡牌，含语法、短语和单词。
其中，日语声调来源于“[Moji辞书](https://www.mojidict.com/)”，部分释义、词性也参考了这个。
目前还在学习中，所以陆陆续续更新，这个更新日志就暂定保留最新5条吧，也当作自己的学习打卡记录了。

文章：https://zhuanlan.zhihu.com/p/682555712

# 用到的插件清单

+ 742319784（Reset Review Stats）：用于清空学习记录，主要用于调试卡牌，不太常用，可以只是用卡牌预览功能来测试卡牌功能。
+ 1344485230（AJT Japanese）：主要用于自动生成振假名（假名注音），可以节省一部分精力。
+ 1436550454（AwesomeTTS - Add speech to your flashcards）：主要用于根据单词、短语、句子生成mp3的朗读语音（TTS）。

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

+ 第2次更新（20240224）：补充插件清单和一些脚本。
+ 第3次更新（20240225）：S01E03基本完成，下次会补充一些正文的短语。日语挺有意思的，咱们说“卖手表的柜台”，那么日语会说“手表柜台”，所以觉得这部分需要补充进去。
+ 第4次更新（20240226）：S01E04的语法完成，单词未完成。
+ 第5次更新（20240227）：S01E04的单词添加完成，单词表后面图文的生词尚未添加。明天出差，暂停更新。
+ 第6次更新（20240302）：正在补充“家”里面涉及的物品单词。然后突然发现几个问题，详见TODO。

# TODO LIST

1. 补充S01E03中表示某某柜台的短语。
2. 目前准备使用AJT Japanese插件自带的单词发音替换单词或/短语部分的TTS，比如NHK的。
3. 准备添加一个不显示字段，用于存放“kanji”，因为目前受Anki振假名语法限制，无法使用搜索功能。

所以，目前**暂停更新**，准备重做。还好目前只有453张卡牌。