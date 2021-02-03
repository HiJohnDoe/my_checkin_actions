# WPS 自动邀请
代码复制的别人的，我只是稍作修改，不能用了我也不会修

### 今日签到状态

![WPS自动邀请](https://github.com/HiJohnDoe/my_checkin_actions/workflows/WPS%E8%87%AA%E5%8A%A8%E9%82%80%E8%AF%B7/badge.svg)

### 目前暂时能用
python源码copy于[wps_invitation.py](https://github.com/BlueskyClouds/My-Actions/blob/master/function/wps_invitation.py)  
  
  
## Github Actions说明  
### 一、代码  
程序代码为：[wps_invitation.py](./wps_invitation.py)  
Github Action 执行代码为：[wps.yml](../.github/workflows/wps.yml)  

### 二、设置账号密码的secrets  
添加名为**WPS_KEY**的secrets  
配置：  
| secrets | content |              detail                    |
|---------|---------|----------------------------------------|
| WPS_KEY	| WPS_SID	| http://zt.wps.cn COOKIE中的wps_sid,只要不注销,10年过期|  
 
*不支持多账号*  

### 三、启用Action  
1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
2 修改任意文件后提交一次  
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)

*若有需求，可以在[wps.yml](../.github/workflows/wps.yml)中自行修改*

