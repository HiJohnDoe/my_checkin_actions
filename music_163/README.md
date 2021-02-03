# 网易云音乐自动签到 + 刷歌
> 网易云音乐自动登录签到 + 刷歌 310 首

## 今日签到状态

![网易云音乐签到](https://github.com/HiJohnDoe/my_checkin_actions/workflows/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90%E7%AD%BE%E5%88%B0/badge.svg)

## Github Actions 部署指南
## 一、代码
签到代码为：music_163/music_163.py  
github action 执行代码为：.github/workflows/music_163.yml
## 二、设置账号密码的secrets
添加名为**MUSIC_163_USER**、**MUSIC_163_PWD**的secrets  
值分别为**账号**、**密码**  
支持多账号，账号之间与密码之间用**半角逗号**分隔，账号于密码的个数要对应  
示例：**MUSIC_163_USER:123456,24678**，**MUSIC_163_PWD:cxkjntm,jntmcxk**
![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)

## 三、启用Action
1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
2 修改任意文件后提交一次  
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)

## 四、查看运行结果
Actions > 网易云音乐签到 > build  
能看到如下图所示，表示成功  

![image-20200727143009081](https://i.loli.net/2020/07/27/kvV31BJKYDp9MRm.png)

## 注意事项

每天运行两次，在上午 6 点和晚上 22 点
若有需求，可以在[.github/workflows/music_163.yml]中自行修改
