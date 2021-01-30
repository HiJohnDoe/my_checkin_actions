# Note163Checkin

**并非全自动，需要使用Fiddler或其他抓包工具获取到Cookie**

## 一、Fork 仓库

**点击右上角的`Fork`**
![Fork.png](https://upload-images.jianshu.io/upload_images/9262602-4cb33e032c4b7488.png)

## 二、添加 Secret

**`Settings`->`Secrets`->`New secret`，添加以下Secret：**
- `Conf`：其值如下：
    ```json
    {
    	"Users": [{
    			"Name": "CC", //自定义名字，选填
    			"Cookie": "YNOTE_LOGIN=true; YNOTE_SESS=v2|abc" //有道云笔记客户端抓包的cookie
    		}, {
    			"Name": "MM",
    			"Cookie": "YNOTE_LOGIN=true; YNOTE_SESS=v2|123"
    		}
    	],
    	"ScKey": "", //server酱sckey，不填不开启
    	"ScType": "Failed" //通知类型. Always:始终通知; Failed:失败时通知; 不填/其他:不通知;
    }
    ```

**步骤图示如下：**
![Secret.png](https://upload-images.jianshu.io/upload_images/9262602-41557a686a52b62f.png)

## 三、启用 Action

**点击`Actions`，再点击`I understand my workflows, go ahead and enable them`**

注意：Fork 的仓库上的 GitHub Actions 的**定时任务不会自动执行**，必须要手动触发一次后才能正常工作。

所以 Fork 之后，点击自己仓库右上角的`Star`，`Star`你的仓库，这是为了触发 Github Action 第一次执行，之后就会自动执行定时任务。

**步骤图示如下：**
![Action.png](https://upload-images.jianshu.io/upload_images/9262602-07b7daea56914f85.png)

![Star.png](https://upload-images.jianshu.io/upload_images/9262602-09bbc99eb0bf5d98.png)

## 四、查看运行结果

**`Actions`->`Checkin`->`build`**，能看到下图，表示运行成功（注意：由于 .NET Core会输出默认日志，请**滚动到最下面查看实际运行结果**）

![image.png](https://upload-images.jianshu.io/upload_images/9262602-a8554266c3f7c1a3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 注意事项

并非全自动，需要使用Fiddler或其他抓包工具获取到Cookie。

每天运行一次，在上午9:00-9:45之间。

也可以点击右上角的`Star`手动运行。

![Star.png](https://upload-images.jianshu.io/upload_images/9262602-09bbc99eb0bf5d98.png)

## 参考

参考了以下项目：
- [ydao](https://github.com/yygtboy/ydao/)
- [node-script](https://github.com/SunSeekerX/node-script)
- [youdaoyun](https://github.com/hezhizheng/youdaoyun)
