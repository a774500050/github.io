---
layout:     post
title:      THBWikiMultiUploadIntro
subtitle:   THBWiki多文件上传工具介绍
date:       2020-05-06
author:     SunCL
header-img: img/post-bg-WBaWC.jpg
catalog: true
tags:
    - MediaWiki
    - THBWiki
    - Python
---


# THBWiki Multi Upload Tool
[THBWikiMultiUpload](https://github.com/a774500050/THBWikiMultiUpload)  
A simple python tool to upload files to THBWiki  
Note that this tool will upload every file in the directory.
## Requirements
just need module [Requests](https://github.com/psf/requests)
```
pip install requests
```

## Start
You need to create a [BotPassword](https://thwiki.cc/Special:BotPasswords).
>Bot passwords allow access to a user account via the
> API without using the account's main login credentials.
> The user rights available when logged in with a bot password may be restricted.

Since you need to upload files, you will need at least those permissions:
* Basic rights (granted default 基本权限 默认已授权)
* Create, edit, and move pages (创建、编辑和移动页面)
* Upload new files (上传新文件)
* Upload, replace, and move files (上传，替换和移动文件)

After creating the bot, just create a **BotToken.txt** in the **main.py** file's
same directory.  
The **BotToken.txt** file should be encoded in UTF-8 and like this:
```
botusername=XXXXX
botpassword=XXXXX
```

Then you can run the python file.
## Run
Run the python file.  
If you set the bot correctly, you will see the terminal shows:
```
Login Success
```

Then you need to input the directory path that contains files you need to upload.  
The program will upload **everything** in the directory.

After inputting the directory, you can input the upload comment for all files 
onetime, or you can just leave it blank. It also supports **WikiText**.  
For example:
```
[[分类:poprication]][[分类:周边图片]]
``` 
Terminal will show the status of each file.
## Uploading Example
![example](../../../../img/post-img-thbwikimultiupload-runexample.jpg)
## About
If you have any problem, just contact [User:SunCL](https://thwiki.cc/User:SunCL).
