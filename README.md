# b-danmakus
get danmakus from Bilibili, and generate a report from the data.

## How to USE

### Step 1 （从B站获取目标视频的弹幕数据）
```
// 安装最新版本python，注意在安装前，在弹框下方勾选：Add Python 3.9 to PATH
Install Python 3.x >=3.6 

// 安装第三方模块
pip install bilibili-api

// 设置目标视频的bvid
编辑 bvid.py 文件

// 执行脚本：生成视频信息文件+3种格式的弹幕文件
python index.py
```

### Step 2 （循环弹幕数据，从百度智能云获取每条弹幕的情感值）
```
// 需要提前安装最新版本的Node.js
Install Node.js

// 安装项目依赖：Axios模块
npm install 

// 执行脚本：生成附带情感值的弹幕数据JSON文件
node request.js
```

### Step 3 （分析数据，生成弹幕情感报告）
```
// 执行脚本：生成分析报告
node report.js
```

## Useful Links
1. [bilibili-api](https://github.com/Passkou/bilibili-api)
2. [b站弹幕系统改版后爬虫方法](https://www.bilibili.com/read/cv9762979/)

## Notes
1. B站最新版的弹幕接口是：https://api.bilibili.com/x/v2/dm/web/seg.so
