## 创建脚手架
     cd react-route/ 进入到要创建项目的目录
     yarn create react-app react-emm-ts --scripts-version=react-scripts-ts 创建名为react-emm-ts的项目
     cd react-emm-ts/ 进入到目录
     yarn add antd 添加antd库
     yarn add react-app-rewired --dev 添加ts,需要修改package.json
     yarn add ts-import-plugin --dev 添加插件懒加载, 添加config-overrides.js
     yarn add react-app-rewire-less --dev 添加主题覆盖插件
     yarn add lite-server -g 安装全局服务器,添加bs-config.json
     sudo ln -s ~/fuybooofile/programfile/node-v6.10.1-linux-x64/bin/lite-server /usr/local/bin/lite-server 赋命令权限
     yarn build 构建
     lite-server 启动服务器
   ***
     使项目支持scss
     yarn eject 弹出默认配置--准备进行个性化配置
     yarn add sass-loader --dev scss编译器
     yarn add node-sass --dev scss编译器
     修改部分代码
     1.脚本:
         "start": "node scripts/start.js",
         "build": "node scripts/build.js",
         "test": "node scripts/test.js",
     2.配置文件:
         添加 test: /\.scss$/, require.resolve('sass-loader'), 即可
         
### 开始开发项目
    1. 安装路由
        yarn add react-router-dom
        yarn add @types/react-router-dom
### 开发火拼俄罗斯
    yarn add socket.io socket通信
    yarn add jquery 使用jquery绑定事件
    yarn add @types/jquery 使typescript使用jquery时有类型提示?
    yarn add @types/node 使用typescript编写node程序
    yarn add express @types/express 使用typescript编写express
    yarn add @types/socket.io-client 使用typescript编写socket.io
    yarn add gulp gulp-typescript 监听node服务器端typescript变化,编译为JavaScript
    supervisor -v