## 安装 Dev-C++

Dev-C++ 是一个开盒即用的 C++ IDE，非常适合新手使用，如果你使用的是 Linux 或者 Mac 操作系统，需要自行选择别的IDE，Clion 或者配置 vscode 环境（上网搜教程）

[下载链接](https://sourceforge.net/projects/orwelldevcpp/)

点开后会看到这样的界面

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204021220.png" alt="image-20250730204021220" style="zoom: 33%;" />

点 OK

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204044623.png" alt="image-20250730204044623" style="zoom:50%;" />

点 `I Agree`

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204113456.png" alt="image-20250730204113456" style="zoom:50%;" />

点 `Next`

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204138683.png" alt="image-20250730204138683" style="zoom:50%;" />

这里选择一个你想要安装的路径，可以默认，然后点击 `Install`

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204446146.png" alt="image-20250730204446146" style="zoom:50%;" />

选择 `Finish` 完成安装

第一次启动会让你选择语言，选择简体中文即可，如果没有也可以手动设置成中文

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204700413.png" alt="image-20250730204700413" style="zoom:50%;" />

点击 工具（tool）-> 点第二个环境选项（Environment option），选中文

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730204748915.png" alt="image-20250730204748915" style="zoom:50%;" />

编译器装好了，如何开始我们的第一段代码呢？

编译器装好了，在上面一栏的文件这里，选择新建->源代码，或者用快捷键 `Ctrl+N` 

之后就会出现一个 `未命名1`

在 `未命名1` 复制如下代码

```cpp
#include<bits/stdc++.h> 
using namespace std;
int main() {

cout<<"hello world!"<<endl;

return 0; }
```

<img src="https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730205027687.png" alt="image-20250730205027687" style="zoom:50%;" />

填入之后还不能运行呢，我们需要保存该文件

点击 **文件->保存** ，或者是用快捷键 `Ctrl+s` 保存一下这个文件。

会弹出这个保存框，保存的地点自己选，文件名中前面自己随便改，后面的 `.cpp` 后缀要保留

![image-20250730205244111](https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730205244111.png)

在这里我们的文件名为 `test.cpp` 位置为桌面

保存成功之后，点这里的编译运行，或者使用快捷键 `F11`

![image-20250730205351840](https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730205351840.png)

如果这里弹出一个黑框，上面显示 `hello world!` 说明代码运行成功了

![image-20250730205655862](https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250730205655862.png)

> 转载自华中师范大学新生资料
