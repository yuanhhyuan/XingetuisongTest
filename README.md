接入信鸽SDK


一、信鸽Android项目环境搭建
Xg-Push-SDK-Android-3.2.2\Xg-Push-SDK-Android\libs下的文件全部拷贝到app/libs目录

App. Buildgradle配置：
defaultConfig {
        applicationId "com.hy.features"
        ......
        sourceSets {
            main{
                jniLibs.srcDirs=['libs']}
        }
    }

Androidmanifest文件的配置：
注意一些组件的下面的配置要改为响应包名的。

二、注册项目信鸽ID以及Key。
1、注册地址：http://xg.qq.com/xg/apps/ctr_app/reg
2、按照提示完成注册，注册成功后在“配置信息”中找到ACCESS ID和ACCESS KEY的值。
3、将得到的ACCESS ID和ACCESS KEY的值更换到AndroidManifest.xml中。

如，我的example中：
Features
package="com.hy.features"

ACCESS ID 2100280904
ACCESS KEY A93K14QAJE1B
SECRET KEY 14b46a5facf8e02ff37d64218b5fa394

三、代码开发

四、信鸽Web推送步骤
注意：客户端需要通过wifi或者4G联网。
登陆：http://xg.qq.com/apps/ctr_app/reg，即可以在web向移动端推送消息


参考资料：
https://blog.csdn.net/u012721519/article/details/52403030
