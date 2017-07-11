
Based on webpack2, support Ejs and Scss.

## Build
```sh
# install build and dev tools
npm install -g webpack webpack-dev-server

# install local dependencies
npm install

# to build (Development)
npm start

# to build (Production)
npm run prod
```

## Support ES6+ 
1.Run 
```sh
npm i -D babel-core babel-preset-latest babel-preset-stage-2 babel-runtime babel-plugin-transform-runtime babel-loader
``` 

2.Create ```.babelrc```:
```
{
  "presets": ["latest", "stage-2"],
  "plugins": ["transform-runtime"]
}
```

3.```webpack-config/base.js``` Add:
```
{
    test: /\.js$/,
    loader: 'babel-loader'
},
```

