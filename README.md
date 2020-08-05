# unity通过TUIO协议连接思岚雷达A2M6-R3。
***
## Step1：安装端口驱动
1. 安装[思岚雷达SDK](https://download.slamtec.com/api/download/rplidar-sdk/1.11.0?lang=netural)
2. 解压安装包，找到`.../rplidar_sdk-release-v1.11.0\tools\cp2102_driver`文件夹下的`CP210xVCPInstaller_xxx.exe`，根据系统位数下载相对应的应用程序  
![driver](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/driver.png)  
3. 连接雷达成功后，雷达的转接头会亮绿色的灯，打开设备管理器，会出现下图端口  
![COM](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/port.jpg)
*** 
## Step2：下载Demo_TUIO
下载[Demo_TUIO附件](https://pan.baidu.com/s/1sJn9BTAyEqMLxU8daHJvxg),密码:`nuwk`
***
## Step3：配置Calibration.exe
1. 打开`...\demo_TUIO\multitouch_Server\multitouch_Server\workspaces\vc10\calibration_project\bin`文件夹下的`calibration_app.exe`
2. 点击Load图标  
![Load](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/load.jpg)
3. 选择打开`...\demo_TUIO\multitouch_Server\multitouch_Server\workspaces\vc10\server_project\bin`文件夹下的`multi_touch.json`  
![Json](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/json.jpg)  
4. 这个时候你会发现雷达开始转动，并且出现如下界面。如果没有转动，请看Json说明
![calibration](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/calibration.jpg)  
***
## Step4：Json说明
![Json说明](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/JsonRM.jpg)
***
## Step5：打开服务器
1. 选择打开`...\demo_TUIO\multitouch_Server\multitouch_Server\workspaces\vc10\server_project\bin`文件夹下的`MultiTouch_Server.exe`  
2. 打开发现，如果你有物体在calibration中设置的范围内，会弹出如下界面，则表示配置正常   
![server](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/server.jpg)
3. 请不要关闭服务器，这时候保持其一直打开状态
***
## Step6：打开Unity工程文件
1. 打开`Sample Scene`,直接运行
2. 区别于其他TouchScript场景，这个场景加入了`TUIO Input`   
![TUIO Input](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/inputTUIO.jpg)
3. 场景正常运行的画面   
![Unity](https://jp-github.oss-cn-shenzhen.aliyuncs.com/unity-tuio-rplidar/Unity.jpg)
***
# 发现这里面有不到位的地方，欢迎指正
