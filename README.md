gradle-eclipse-multi-channel-build
==================================

基于友盟的gradle多渠道打包工具的改进版本<br />

<h2>专为Eclipse工程定制的多渠道多依赖项目的打包脚本<h2>

==================================
感谢友盟的多渠道打包工具：
https://github.com/umeng/umeng-muti-channel-build-tool/tree/master/Gradle

我提交的版本主要修复以下问题：<br />
1、次版本是为了适配Eclipse的多项目依赖工程的打包。<br />
2、修复打包过程中文显示乱码问题。<br />
3、修改apk的名字以及指定apk存放的文件夹。<br />
4、增加签名的机制<br />

使用方法：<br />
1、将build.gradle和settings.gradle拷贝到目标工程下面，修改里面的路径、文件名等相关参数。<br />
2、将lib.gradle拷贝到lib工程下面。<br />

然后在目标root工程的下面运行命令：<br />
gradle -PSTOREPASS='你的keystore密码' -PKEYPASS='你的alias密码' clean --stacktrace <br />
gradle -PSTOREPASS='你的keystore密码' -PKEYPASS='你的alias密码' aR --stacktrace <br />


=================================

Copyright infsafe 2014

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
