# note163checkin
代码复制的别人的，我只是稍作修改，不能用了我也不会修

## 今日签到状态

![有道云笔记签到](https://github.com/HiJohnDoe/my_checkin_actions/workflows/%E6%9C%89%E9%81%93%E4%BA%91%E7%AC%94%E8%AE%B0%E7%AD%BE%E5%88%B0/badge.svg)


## 目前暂时能用
仓库源码 https://github.com/jsk18/note163checkin.git  
python源码copy于(https://github.com/lepecoder/checkin)

##下面的说明也是复制的别人项目的

# Github Actions说明
## 一、代码
签到代码为：note163/note163.py  
github action 执行代码为：.github/workflows/note_163.yml
## 二、设置账号密码的secrets
添加名为**NOTE_163_USER**、**NOTE_163_PWD**的secrets  
值分别为**账号**、**密码**  
## 密码需用MD5加密工具加密，加密格式为32位[小]:(https://tool.chinaz.com/tools/md5.aspx)
支持多账号，账号之间与密码之间用**半角逗号**分隔，账号于密码的个数要对应  
示例：**NOTE_163_USER:123456,24678**，**NOTE_163_PWD:cxkjntm,jntmcxk**
![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)

## 三、启用Action
1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
2 修改任意文件后提交一次  
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)

## 四、查看运行结果
Actions > 有道云笔记签到 > build  
能看到如下图所示，表示成功  
![](http://note.youdao.com/yws/public/resource/17edb8861d2106a5c39ec94d91919150/xmlnote/48958A4994D64C20867281B67B7CDAFD/1059)

此后，将会在北京时间每天上午9:00签到一次  
若有需求，可以在[.github/workflows/note163.yml]中自行修改
