<div align="center">

<img src="https://readme-typing-svg.herokuapp.com/?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&random=false&width=600&lines=Hi+%F0%9F%91%8B%2C+I%27m+%E8%B5%AB%E8%B5%AB;Java+Backend+Developer;%E5%90%8E%E7%AB%AF%E5%BC%80%E5%8F%91+%7C+%E9%AB%98%E5%B9%B6%E5%8F%91%E6%9E%B6%E6%9E%84+%7C+AI+%E5%BA%94%E7%94%A8;%E6%AC%A2%E8%BF%8E%E4%BA%A4%E6%B5%81+%F0%9F%9A%80" alt="Typing SVG" />

[![GitHub followers](https://img.shields.io/github/followers/zhx1233?style=for-the-badge&logo=github&color=6366F1&labelColor=1F2937)](https://github.com/zhx1233)
[![Profile Views](https://komarev.com/ghpvc/?username=zhx1233&style=for-the-badge&color=6366F1&label=PROFILE+VIEWS)](https://github.com/zhx1233)

</div>

<div align="center">

### 🛠️ Tech Stack

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![MyBatis-Plus](https://img.shields.io/badge/MyBatis_Plus-FF0000?style=for-the-badge&logo=mybatis&logoColor=white)
![ShardingSphere](https://img.shields.io/badge/ShardingSphere-FF6B00?style=for-the-badge&logo=apacheshardingsphere&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Nacos](https://img.shields.io/badge/Nacos-3EB9FF?style=for-the-badge&logo=alibabacloud&logoColor=white)
![Sentinel](https://img.shields.io/badge/Sentinel-3EB9FF?style=for-the-badge&logo=alibabacloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

</div>

<br/>

<div align="center">
  <img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />
</div>

<br/>

## 🚀 Featured Projects

<br/>

<div align="center">
<a href="https://github.com/zhx1233/shortlink">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=zhx1233&repo=shortlink&theme=tokyonight&hide_border=true&bg_color=1F2937&title_color=6366F1&icon_color=6366F1&text_color=C9D1D9&description_lines_count=3" />
</a>
</div>

<br/>

### 🔗 链析 — 内容创作者短链流量分析工具

> **JDK17 + SpringBoot3 + SpringCloud 微服务 | 独立开发后端三模块**

面向个人创作者与小微内容团队，提供长链接一键缩链、按分发平台分组管理、链接有效期配置，内置 **PV/UV/UIP 访问量、地域分布、设备/浏览器/OS、访问时段**等全维度数据统计，帮助创作者量化公众号、小红书、朋友圈等多平台分发效果，用数据反哺内容策略。

<img src="https://oss.open8gu.com/image-20231026132606180.png" width="100%" />

<table>
<tr><td>

#### 🎯 核心技术实践

| 模块 | 技术方案 | 解决的问题 |
|------|---------|-----------|
| **多级缓存架构** | Redis → 布隆过滤器 → 空值缓存 → 分布式锁 | 防穿透/击穿，压测缓存命中 **3500+ QPS，< 1ms** |
| **水平分表 + 路由表** | ShardingSphere 16 表 + t_link_goto 路由表 | 应对数据膨胀，跳转时路由表补全分片键，精确路由到单表 |
| **异步统计写入** | Redis Stream 消息队列 + 消费者幂等 | 跳转不阻塞，统计异步处理；两阶段 SETNX 防重复消费 |
| **缓存一致性** | 先更新数据库再删缓存 | 避免并发窗口期写脏数据；缓存过期时间兜底 |
| **并发安全控制** | Redisson 读写锁（short-link 粒度） | 变更分发平台时加写锁，统计消费加读锁，迁移期间数据不丢 |
| **接口保护** | Sentinel QPS 限流 + Gateway Token 鉴权 + 请求头透传 | 防恶意刷量，统一鉴权，下游无需重复依赖 Redis |

</td></tr>
</table>

<br/>

<div align="center">
  <img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />
</div>

<br/>

<div align="center">
<a href="https://github.com/zhx1233/the-medical-project-t1">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=zhx1233&repo=the-medical-project-t1&theme=tokyonight&hide_border=true&bg_color=1F2937&title_color=6366F1&icon_color=6366F1&text_color=C9D1D9&description_lines_count=3" />
</a>
</div>

<br/>

### 🏥 医影智诊 — 医疗影像管理与 AI 辅助诊断平台

> **Spring Boot 3 + MyBatis-Plus + PostgreSQL | 6 人团队，担任后端开发**

面向医生、科研人员和管理员三角色，围绕 **"病例管理 → 影像上传 → AI 诊断 → 结果审核 → 科研反馈"** 构建完整业务闭环。医生上传胸部 X 光发起肺炎 AI 推理，科研人员分析反馈优化模型，管理员维护权限和审计日志。后端全部接口由我开发。

```
Spring Boot 后端 ──HTTP──▶ Python CV 推理服务 (PyTorch + ResNet + Grad-CAM)
       │                        │
       └──HTTP──▶ Python Agent 服务 (FastAPI + LangGraph + RAG)
                        │
                        ▼
                  PostgreSQL (业务 + 科研 + Agent 会话)
```

<table>
<tr><td>

#### 🎯 核心技术实践

| 模块 | 技术方案 | 解决的问题 |
|------|---------|-----------|
| **多角色 RBAC 权限** | 自写 JwtInterceptor + RoleAccessPolicy 路径匹配 | 三角色接口级权限隔离，非 Spring Security 注解，Token 黑名单登出 |
| **异步推理任务管理** | 自定义线程池 + 状态机流转 | AI 推理耗时几十秒，接口立即返回 taskId，后台异步执行 queued→running→completed/failed |
| **外部 AI 服务对接** | WebClient multipart 文件传输 | 调 Python CV 服务推理，处理超时、异常容错、标注图下载 |
| **操作审计日志** | OperationLogInterceptor 拦截 + 管理端查询 | 关键操作全量留痕，支持按时间/类型追溯，满足合规要求 |
| **Docker Compose 编排** | 前端 + 后端 + CV + Agent + PostgreSQL 一键启动 | 全栈 5 服务统一编排，首次启动自动初始化 schema 和种子数据 |

</td></tr>
</table>

<br/>

<div align="center">
  <img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />
</div>

<br/>

<div align="center">

### 📊 GitHub Stats

<a href="https://github.com/zhx1233">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=zhx1233&show_icons=true&theme=tokyonight&hide_border=true&bg_color=1F2937&title_color=6366F1&icon_color=6366F1&text_color=C9D1D9&count_private=true&include_all_commits=true" />
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zhx1233&layout=compact&theme=tokyonight&hide_border=true&bg_color=1F2937&title_color=6366F1&icon_color=6366F1&text_color=C9D1D9&langs_count=8" />
</a>

<br/>

<a href="https://github.com/zhx1233">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=zhx1233&theme=tokyonight&hide_border=true&background=1F2937&stroke=6366F1&ring=6366F1&fire=6366F1&currStreakNum=C9D1D9&sideNums=C9D1D9&currStreakLabel=C9D1D9&sideLabels=C9D1D9" />
</a>

<br/>

<a href="https://github.com/zhx1233">
  <img src="https://github-profile-trophy.vercel.app/?username=zhx1233&theme=tokyonight&no-frame=true&margin-w=8&column=7&title=Stars,Followers,Commit,Repositories,Issues,PullRequest,Reviews" />
</a>

</div>

<br/>

<div align="center">
  <img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />
</div>

<br/>

<div align="center">

### 🐍 Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zhx1233/zhx1233/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zhx1233/zhx1233/output/github-contribution-grid-snake.svg" />
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/zhx1233/zhx1233/output/github-contribution-grid-snake.svg" />
</picture>

</div>

<br/>

<div align="center">
  <img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />
</div>

<br/>

<div align="center">

### 🤝 Let's Connect

[![GitHub](https://img.shields.io/badge/GitHub-zhx1233-6366F1?style=for-the-badge&logo=github&logoColor=white&labelColor=1F2937)](https://github.com/zhx1233)

</div>

<br/>

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com/?font=Fira+Code&weight=400&size=16&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&random=false&width=440&lines=Thanks+for+visiting!+%E2%9C%A8;Star+%E2%AD%90+the+projects+you+like;Happy+Coding!+%F0%9F%92%BB" alt="Footer" />
</div>
