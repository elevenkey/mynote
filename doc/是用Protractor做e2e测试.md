# 是用Protractor做e2e测试
## 安装Protractor

### 全局安装protractor
    npm install -g protractor

### 升级webdriver-manager（protractor 依赖的组建）
    webdriver-manager update

### 启动webdriver-manager
    webdriver-manager start

## 运行protractor至少需要一个测试文件，一个配置文件
参考：http://angular.github.io/protractor/#/tutorial

## 执行测试
    protractor conf.js
