# table-demo

## el-table使用案例：列自定义筛选，时间控件筛选
#### 1.克隆项目至本地
#### 2.cd到项目根目录，运行如下命令下载依赖：
```
npm install
```

#### 3.下载完成后运行
```
npm run serve
```
当表头时间控件条件变化时，在下面函数中做筛选（如请求后端）操作

```javascript
timeChangeAction(){
    console.log(this.value1);
}
```