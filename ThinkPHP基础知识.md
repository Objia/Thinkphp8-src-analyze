# 框架中通用变量

```php
$rootPath	=项目目录/
$thinkPath	=项目目录/vendor/topthink/framwork/src/think/
$libPath	=项目目录/vendor/topthink/framwork/src/think/library/
$basePath	=项目目录/app/
$appPath	=项目目录/app[/模块名]/
$confPath	=项目目录/config/
$runtimePath=项目目录/runtime[/模块名]/
$extendPath	=项目目录/extend/
$logPath	=项目目录/runtime[/模块名]/log/
```

# ThinkPHP的多应用模式和多模块模式

以下是多应用模式和多模块模式的典型目录结构

```
├─app 应用目录
│  ├─index              主应用
│  │  ├─controller      控制器目录
│  │  │  ├─content      模块1目录
│  │  │  ├─file         模块2目录
│  │  │  └─ ...         更多模块目录
│  │  ├─model           模型目录
│  │  ├─view            视图目录
│  │  ├─config          配置目录
│  │  ├─route           路由目录
│  │  └─ ...            更多类库目录
│  │ 
│  ├─admin              后台应用
│  │  ├─controller      控制器目录
│  │  │  ├─content      模块1目录
│  │  │  ├─file         模块2目录
│  │  │  └─ ...         更多模块目录
│  │  ├─model           模型目录
│  │  ├─view            视图目录
│  │  ├─config          配置目录
│  │  ├─route           路由目录
│  │  └─ ...            更多类库目录
│
├─public                WEB目录（对外访问目录）
│  ├─admin.php          后台入口文件
│  ├─index.php          入口文件
│  ├─router.php         快速测试文件
│  └─.htaccess          用于apache的重写
│
├─config                全局应用配置目录
├─runtime               运行时目录
│  ├─index              index应用运行时目录
│  └─admin              admin应用运行时目录
```



