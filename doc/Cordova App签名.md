# Cordova APP 签名方法

## 1、是用keytool生成签名文件

        keytool -genkey -v -keystore xxx.keystore -alias yyy -keyalg RSA -keysize 2048 -validity 10000. 
        注：xxx.keystore 为keystore文件名   yyy为alias名，可以自己设定 -validity 10000 为有效期

        运行上面命令后，会运行一个交互式的程序，需要填写一些相关问题，其中密码一定要记住。

## 2、将生成的签名文件用于APP
        
        这里采用cordova文档推荐的方法：在运行 cordova build或者run命令时，采用--buildConfig参数。需要自己写一个配置文件。参考下面的官方文档即可。
        参考：https://cordova.apache.org/docs/en/5.0.0/guide/platforms/android/tools.html Signing the App小节
