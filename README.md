# test-project

> this is a vuejs-test-project

## create a vue-project
- # 创建一个基于 webpack 模板的新项目
- $ vue init webpack my-project
- # 安装依赖，走你
- $ cd my-project
- $ npm install
- $ npm run dev

## use github
- 打开Git Bash输入以下命令
- 如果还没输入全局配置就先把这个全局配置输入上去
- Git 全局设置:
- git config --global user.name "gaoxiaohui1" 
- git config --global user.email "648282572@qq.com"
- git config --global credential.helper store //在vs中每次更新代码都会要输入账号密码，方便起见，可以配置一下让GIT记住密码账号。

- cd d:/wamp/www/mall360/wap              //首先指定到你的项目目录下
- git init
- touch README.md
- git add README.md
- git commit -m "first commit"
- git remote add origin https://github.com/gaoxiaohui1/test.git   //用你仓库的url
- git push -u origin master  //提交到你的仓库

# Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
