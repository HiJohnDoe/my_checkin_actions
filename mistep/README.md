source from: https://github.com/Squaregentleman/mimotion.git

# 小米运动自动刷步数

## 今日签到状态  
![小米刷步数](https://github.com/HiJohnDoe/my_checkin_actions/workflows/%E5%B0%8F%E7%B1%B3%E5%88%B7%E6%AD%A5%E6%95%B0/badge.svg)  


> 小米运动自动刷步数

## Github Actions 部署指南

### 一、Fork 此仓库

### 二、设置账号密码

添加名为  **SCKEY**、**MI_USER**、**MI_PWD**、**MI_STEP** 的变量，值分别为 **server酱推送key（0关闭）**、 **账号（仅支持手机号）**、**密码**、**步数（0则为1w-2w之间随机 或自定义随机范围[18000-25000]）**

> Settings-->Secrets-->New secret

### 三、多账户(用不上请忽略)

多账户请用 **#** 分割 然后保存到变量 
多变量  **MI_USER** 、 **MI_PWD** 和 **MI_STEP**
server酱推送 只开启了单一推送 **SCKEY** 不能填多个，只能填一个server酱推送码

#### 例如

**13800138000#13800138001** 变量 **MI_USER**

**abc123qwe#abcqwe2** 变量 **MI_PWD**

**19256-19856#19888-19999** 变量 **MI_STEP**

**sfsdegdvcabc123qwe** 变量 **SCKEY**

### 四、自定义启动时间

编辑 **.github/workflows/run.yml**

找到 cron: 0 10 * * *

修改其中的10为你要的时间

需要运行的时间-8就是UTC时间

## 注意事项

1. 每天运行一次，在下午 6 点

2. 多账户的数量和密码请一定要对上 不然无法使用!!!

3. 启动时间得是UTC时间!

4. server酱注册地址 [点我](http://sc.ftqq.com/)

5. 如果支付宝没有更新步数,到小米运动->设置->账号->注销账号->清空数据,然后重新登录,重新绑定第三方
