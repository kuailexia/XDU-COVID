# XDU 晨午晚检自动填报 GitHub Actions 版本

## 食用方法

### 获取代码（必须）
首先fork本仓库到自己的GitHub账户

### 设置账号密码（必须）
在Fork后的仓库中点击设置，点击Secret，点击New repository secret分别设置以下变量：

* USER
* PASSWORD
* WXID
  
注意USER和PASSWORD为一站式账号密码，WXID随意填写

### 启用GitHub Actions（必须）
由于仓库是Fork而来的，需要你手动开启Actions才可以定时填报。

点击Actions连续点击**至少两次**启用即可启动自动填报了。

### 测试填报（可选）

如果不确定是否已经启动定时填报，你可以编辑任意一个文件（推荐编辑`/.github/workflows/main.yml`文件），提交之后可以查看Actions中是否有填报记录。

### 修改填报时间（推荐，可选）

编辑`/.github/workflows/main.yml`文件第12行

原文为`- cron: '11 0,4,11 * * *'`表示UTC时间0时11分、4时11分、11时11分填报三次，您可以按需修改。

***注意：UTC时间早北京时间8小时***

## 其他

### 本仓库代码参考

* https://github.com/PauperZ/XduCheckIn

### 个人博客

* https://blog.ylwind.cn
