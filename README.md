# Easy云盘项目架构
## 技术栈

| 分类 | 技术 | 版本 |
|------|------|------|
| 前端 | Vue 3 | 3.x |
| 前端 | TypeScript | 4.x+ |
| 前端 | Element Plus | 2.x |
| 前端 | Axios | 1.x |
| 后端 | Spring Boot | 3.x |
| 后端 | MyBatis-Plus | 3.x |
| 后端 | MySQL | 8.x |
| 后端 | Redis | 7.x |

## 项目运行截图
登录界面
<img width="1268" height="682" alt="图片1" src="https://github.com/user-attachments/assets/1ab94860-0ba2-4295-9afb-bd279fff1868" />
成功登录
<img width="1920" height="1022" alt="图片2" src="https://github.com/user-attachments/assets/75e792bf-4b58-4b8d-a307-090facafb5a2" />
进入首页
<img width="1920" height="1036" alt="图片3" src="https://github.com/user-attachments/assets/a94572ed-2cc9-4334-8a11-b400f7b03e1b" />
文件类型进具体分类-部分显示
<img width="1920" height="988" alt="图片4" src="https://github.com/user-attachments/assets/94415cdb-036b-44c7-a0b2-6bbfa4b4c9cc" />
文件分享-创建分享
<img width="1906" height="995" alt="图片5" src="https://github.com/user-attachments/assets/2c519e93-4324-4857-a1b9-e5b1251c1d96" />
文件分享-复制分享链接(可进行直接下载或保存至网盘)
<img width="1919" height="1034" alt="图片6" src="https://github.com/user-attachments/assets/477a770d-0c31-426b-aa09-581e22cbbac2" />
文件删除后移至回收站-可进行恢复或彻底粉碎
<img width="1920" height="1030" alt="图片7" src="https://github.com/user-attachments/assets/da8b2b31-5d49-47f2-a88d-a477b2c4470a" />
会员中心-设有三个套餐(可进行按需购买-充值通过支付宝沙箱支付实现)充值成功显示vip会员标识
<img width="1920" height="1035" alt="图片8" src="https://github.com/user-attachments/assets/20e87f0d-667f-48f3-b4c0-3a12216c1df9" />
登录页-分享中心
<img width="1920" height="995" alt="图片9" src="https://github.com/user-attachments/assets/e6293430-3711-4391-b421-65d26b298983" />
登录页-管理员账号登录
<img width="1267" height="653" alt="图片10" src="https://github.com/user-attachments/assets/d9caf42c-817e-4462-926d-6f8601270622" />
管理员后台页面-仪表盘
<img width="1267" height="653" alt="图片10" src="https://github.com/user-attachments/assets/4ec0328e-7be6-4e4f-800a-2ae1b95d9011" />
管理员后台页面-用户管理-显示具体用户信息(可进行账号的启用和禁用/修改账号网盘空间)
<img width="1910" height="1004" alt="图片12" src="https://github.com/user-attachments/assets/f17d0e7f-fb85-4851-b6ba-864a71a197d7" />
管理员后台页面-文件管理-可查看所有账号网盘内的文件
<img width="1920" height="959" alt="图片13" src="https://github.com/user-attachments/assets/6019655f-c589-45ae-8a70-4be8c969727d" />
管理员后台页面-系统设置-可修改所有用户基础网盘空间
<img width="1909" height="985" alt="图片14" src="https://github.com/user-attachments/assets/8102c726-50d3-459a-a3f6-b43b6d4db22d" />

## 项目启动流程

### 前端启动
1. **进入前端目录**：
   ```bash
   cd easypan-frontend
   ```
2. **安装依赖**（首次运行）：
   ```bash
   npm install
   ```
3. **启动开发服务器**：
   ```bash
   npm run dev
   ```
4. **访问前端**：
   - 打开浏览器，访问终端输出的本地地址（通常是 `http://localhost:5173`）

### 后端启动
#### 方法1：使用IDEA启动
1. 打开 `easypan-backend` 目录
2. 找到 `EasyPanApplication.java` 启动类
3. 右键点击并选择 "Run EasyPanApplication"

#### 方法2：使用Maven启动
1. **进入后端目录**：
   ```bash
   cd easypan-backend
   ```
2. **启动应用**：
   ```bash
   mvn spring-boot:run
   ```
3. **访问后端API**：
   - 后端服务默认运行在 `http://localhost:8080`

## 环境要求
- **前端**：Node.js 16.x+
- **后端**：JDK 17+, Maven 3.8+
- **数据库**：MySQL 8.x
- **缓存**：Redis 7.x














