npm install -g babel-cli

npm install -g babel-cli --save-dev

.bablelrc配置
{
  "presets": ["es2015"],
  "plugins": [] 
}


 npm install --save-dev babel-preset-es2015
 $ babel a.js --out-file b.js
 #### 或者
 $ babel a.js -o b.js
  
  #### 整个目录转码
  #### --out-dir 或 -d 参数指定输出目录
  #### babel src --out-dir lib
  #### 或者
 $ babel src -d lib
  
 #### -s 参数生成source map文件
 $ babel src -d lib -s
 在package.json配置  可自动化编译
  "build": "babel src -d lib"