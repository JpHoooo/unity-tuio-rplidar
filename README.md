# 🔥 Unity connects RPLidar A2M6-R3 through TUIO protocol 🔥

Unity version: `2020.2.6 f1`

### ⭐ Step 1：Install the port driver

- Install [RPLidar SDK](https://download.slamtec.com/api/download/rplidar-sdk/1.11.0?lang=netural)
- Unzip the `rplidar_sdk_v1.11.0.zip`, find the `CP210x_Windows_Drivers.zip` under the `.../rplidar_sdk-release-v1.11.0\tools` folder
- unzip `CP210x_Windows_Drivers.zip`
- Install the `CP210xVCPInstaller.exe` according to the number of system bits
- After the ridar is successfully connected, the adapter of the ridar will turn on a green light, open the 'Device Manager', the following port will appear `Silicon Labs CP210x USB to UART Bridge(COM(port number))`

### ⭐ Step 2：Install the Demo_TUIO file

|Cloud Disk Name|URL|Password|
|:---:|:---:|:---:|
|百度云盘|[BaiduURL](https://pan.baidu.com/s/1HQlIvJQmCekOLij68EWW2Q)|tuio|
|Google Cloud Disk|[GoogleURL](https://drive.google.com/file/d/1g8julT8AvS8T78rENHXxvgM1pD7uEdcQ/view?usp=sharing)|-|

### ⭐ Step 3：Configure Calibration.exe
- Open `calibration_app.exe` under the `...\demo_TUIO\multitouch_Server\multitouch_Server\workspaces\vc10\calibration_project\bin` folder
- (if you lose `msvcp110d.dll` or `msvcr110d.dll`, click [here](https://pan.baidu.com/s/1prwVwWJjMHFaeA02CqSPBQ), password: `dll0`)
- Click `Load` icon  
- Open `multi_touch.json` Under the `...\demo_TUIO\multitouch_Server\multitouch_Server\workspaces\vc10\server_project\bin` folder
- At this time you will find that the radar starts to rotate, and the following interface appears. If it does not rotate, please see Json instructions

### ⭐ Step 4：Json instructions
- All the pictures below are thumbnails, and the high-resolution pictures are in the project file.
  > ![Json说明](https://github.com/JpHoooo/unity-tuio-rplidar/blob/master/Assets/imgs/LDImgs/JsonRM.png)

### ⭐ Step 5：Open the server
- Open `MultiTouch_Server.exe` under the `...\demo_TUIO\multitouch_Server\multitouch_Server\workspaces\vc10\server_project\bin` folder 
- If you have an object within the range set in calibration, the following interface will pop up, indicating that the configuration is normal   
  > ![server](https://github.com/JpHoooo/unity-tuio-rplidar/blob/master/Assets/imgs/LDImgs/server.png)
- Please do not shut down the server, keep it always on at this time

### ⭐ Step 6：Open Unity Project
- Open `Main`, Run it
- This scene already adds `TUIO Input` Script  
  > ![TUIO Input](https://github.com/JpHoooo/unity-tuio-rplidar/blob/master/Assets/imgs/LDImgs/settings.png)
- If the cursor is moved to the object and the shape name of the object appears in the console, it means that the scene runs successfully 
  > ![Unity](https://github.com/JpHoooo/unity-tuio-rplidar/blob/master/Assets/imgs/LDImgs/Unity.png)
