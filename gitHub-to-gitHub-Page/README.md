## Step


### 推送程式碼至git專案


### 安裝套件 gh-pages
```npm
 npm i gh-pages
```


### 修改package.json (Script)

將Sctipt新增兩行程式碼
```json
"predeploy": "npm run build",
"deploy": "gh-pages -d build",
```

整行程式碼如下方
```json
"scripts": {
	"predeploy": "npm run build", 
	"deploy": "gh-pages -d build",

	"start": "react-scripts start",
	"build": "react-scripts build",
	"test": "react-scripts test",
	"eject": "react-scripts eject",
    // ...
  }
  ```


### 修改package.json (新增 homepage)
在 package.json裡加上 Github Page 網址，此**username**為帳戶名，**porjectname**為gitHub上專案名稱
```json
  "homepage": "https://username.github.io/porjectname",
```

程式碼如下方
```json
{
  "name": "realtime-weather-app",
  "homepage": "https://username.github.io/porjectname",
  "version": "0.1.0",
  "private": true,
  // ...
}
  ```

## 發布至gitHub
```npm
npm run deploy
```



## 參考網址
https://rexhung0302.github.io/2021/09/28/20210928/