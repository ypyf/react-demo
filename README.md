#安装 npm + typescript + react

###1.安装ts：

```
npm install -g typescript@next
```

###2.安装react和react-dom

```
npm install --save react react-dom
```

###3.安装 browserify

```
npm install --save browserify
```

###4.安装 tsd:

```
npm install -g tsd
```

###5.生成tsd文件:

```
tsd install node --save
tsd install react --save
tsd install react-dom --save
```

###6.配置工程的tsconfig.json文件,注意jsx编译选项设置为"react"（参看demo)

###7.构建tsx文件为js。如果上一步将jsx的设置为"preserve"，生成的将是jsx文件。

###8.打包成浏览器文件:

```
browserify -t babelify main.js -o bundle.js
```