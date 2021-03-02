# 爱奇艺会员签到
代码复制的别人的，我只是稍作修改，不能用了我也不会修

### 今日签到状态

![爱奇艺会员签到](https://github.com/HiJohnDoe/my_checkin_actions/actions/workflows/iqiyi.yml/badge.svg)

### 目前暂时能用
nodejs源码copy于[iqiyi.js](https://github.com/BlueskyClouds/My-Actions/blob/master/function/iqiyi.js)  
  
  
## Github Actions说明  
### 一、代码  
程序代码为：[iqiyi.js](./iqiyi.js)  
Github Action 执行代码为：[iqiyi.yml](../.github/workflows/iqiyi.yml)  

### 二、设置账号密码的secrets  
添加名为**IQIYI_COOKIE**的secrets  
配置：  
| secrets | content |              detail                    |
|---------|---------|----------------------------------------|
| IQIYI_COOKIE	| authcookie	| 爱奇艺 COOKIE中的authcookie,只要不注销,有效期三个月|  
 
*不支持多账号*  

### 三、启用Action  
1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
2 修改任意文件后提交一次  
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)

*若有需求，可以在[iqiyi.yml](../.github/workflows/iqiyi.yml)中自行修改*

