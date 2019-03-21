
### 含义
```
  rimraf 包的作用：以包的形式包装rm -rf命令，用来删除文件和文件夹的，不管文件夹是否为空，都可删除.
```
### 安装
```
  npm install rimraf --save-dev
```
### 使用
```
  const rimraf = require('rimraf');
  rimraf('./test.txt', function (err) { // 删除当前目录下的 test.txt
    console.log(err);
  });

or
  // package.json:
  ...
  "scripts": {
      ...
      "build": "webpack --progress --hide-modules --config build/webpack.build.js && rimraf dist && node build/build.js"
    },
    
```
