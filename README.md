# Easy云盘项目架构

## 系统架构

```mermaid
graph TD
    subgraph 前端
        A[用户界面] --> B[Vue 3组件]
        B --> C[API调用]
        C --> D[axios请求]
        B --> E[状态管理]
        E --> F[本地存储]
    end

    subgraph 后端
        G[Spring Boot应用] --> H[控制器层]
        H --> I[服务层]
        I --> J[数据访问层]
        J --> K[MySQL数据库]
        H --> L[拦截器]
        L --> M[权限验证]
    end

    D <--> G
```

## 前端架构

```mermaid
graph TD
    subgraph 页面组件
        A[Login.vue] --> B[AdminLogin.vue]
        B --> C[AdminDashboard.vue]
        C --> D[用户管理]
        C --> E[文件管理]
        C --> F[系统设置]
    end

    subgraph 工具模块
        G[request.ts] --> H[axios配置]
        H --> I[拦截器]
        I --> J[token管理]
    end

    subgraph API模块
        K[user.ts] --> L[用户相关API]
        M[admin.ts] --> N[管理员相关API]
    end

    D --> L
    E --> N
    F --> N
```

## 后端架构

```mermaid
graph TD
    subgraph 控制器层
        A[AccountController] --> B[用户相关接口]
        C[AdminController] --> D[管理员相关接口]
        E[FileInfoController] --> F[文件相关接口]
        G[FileShareController] --> H[文件分享接口]
    end

    subgraph 服务层
        I[UserInfoService] --> J[用户业务逻辑]
        K[FileInfoService] --> L[文件业务逻辑]
        M[FileShareService] --> N[文件分享业务逻辑]
    end

    subgraph 数据访问层
        O[UserInfoMapper] --> P[用户数据操作]
        Q[FileInfoMapper] --> R[文件数据操作]
        S[FileShareMapper] --> T[文件分享数据操作]
    end

    B --> J
    D --> J
    D --> L
    F --> L
    H --> N
    J --> P
    L --> R
    N --> T
```

## 功能模块

```mermaid
graph TD
    subgraph 核心功能
        A[用户认证] --> B[登录/注册]
        B --> C[密码重置]
        C --> D[邮箱验证]
    end

    subgraph 文件管理
        E[文件上传] --> F[文件下载]
        F --> G[文件分享]
        G --> H[文件管理]
    end

    subgraph 系统管理
        I[用户管理] --> J[账号启用/禁用]
        J --> K[存储空间管理]
        K --> L[VIP管理]
    end
```

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
