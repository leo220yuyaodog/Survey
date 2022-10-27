## 后端运行
1. 创建数据库star-vey并导入数据脚本sty_2021xxxx.sql
2. 修改数据库连接，编辑resources目录下的application-druid.yml
```
数据源配置
spring:
  druid:
主库数据源
    master:
      url: 数据库地址
        username: 数据库账号
        password: 数据库密码
```
3. 打开项目运行com.ruoyi.RuoYiApplication.java，出现如下图表示启动成功。

## 前端
```
# 进入项目目录
cd web

# 安装依赖
npm install

# 强烈建议不要用直接使用 cnpm 安装，会有各种诡异的 bug，可以通过重新指定 registry 来解决 npm 安装速度慢的问题。
npm install --registry=https://registry.npmmirror.com

# 本地开发 启动项目
npm run dev
```
## 项目结构
```text
com.ruoyi     
├── common            // 工具类
│       └── annotation                    // 自定义注解
│       └── config                        // 全局配置
│       └── constant                      // 通用常量
│       └── core                          // 核心控制
│       └── enums                         // 通用枚举
│       └── exception                     // 通用异常
│       └── filter                        // 过滤器处理
│       └── utils                         // 通用类处理
├── framework         // 框架核心
│       └── aspectj                       // 注解实现
│       └── config                        // 系统配置
│       └── datasource                    // 数据权限
│       └── interceptor                   // 拦截器
│       └── manager                       // 异步处理
│       └── security                      // 权限控制
│       └── web                           // 前端控制
├── system      // 系统代码
├── admin       // 后台服务
├── xxxxxx      // 其他模块 (问卷模块）
```

## 详细介绍 见

[RuoYi](http://doc.ruoyi.vip/ruoyi-vue/document/xmjs.html#%E5%90%8E%E7%AB%AF%E6%8A%80%E6%9C%AF)
