# QtPackTool
a sample tool for collect most of the depend dll for the executable file

## 步骤
* 使用 `Qt` 打开项目，`F5` 运行，鼠标右键打开 `Debugger Log` 窗口， 复制左侧日志内容到 `logs.txt` 文本文件中
* 新建文件夹，放入可执行文件和 `logs.txt` 文本文件
* 输入 `logs.txt` 文件的路径到输入框中
* 点击 `开始打包` 按钮
&nbsp;
## 说明

* `log.txt` 文件中内容为 `Qt` 生成的 `Debugger Log` 内容
* `Windows` 系统下默认不附带 `C:/Windows/System32` 目录中的动态库
* `Linux` 系统下默认不附带 `/lib/x86_64-linux-gnu/` 目录中的动态库
* `Linux` 系统下，打包后要修改 `/etc/ld.so.conf` 来添加动态库检索目录
* 程序无法收集配置文件、qrc以外的资源等，需要手动拷贝
