# SchoolAssociation
高校社团管理系统  亮：AI辅助任务分配、协同过滤算法推荐、ECharts数据可视化、活动参与闭环、校园交流与反馈、器材借还管理； 角色：学生、社团管理员、管理员；

所有源码均本人开发，项目是前后端分离的，所有的项目都具备了完整的业务逻辑，不仅仅局限于基础的增删改查（CRUD）操作，系统亮点众多。

本文注重于计算机毕业设计选题指导，列出题目均有源码， 大家可以去【公众号】(毕业终点站)获取或者加我【qq】(2112698948)提意见(别忘记Star哟)。备注：git

声明：仅用于学习使用，请勿用于任何商业行为！

1.系统非商用，非开源，非无偿。

2.由本人开发，如需源码，请联系以下方式，qq:2112698948。

3.项目有很多，并未全部上传，如果未找到想要的，可直接咨询。

# D6037 · 高校社团管理系统

> 本项目仅用于学习交流。文档展示 22 张截图，需要了解更多，请联系我。

## 项目简介

高校社团管理系统是一套面向校园社团日常运营的综合管理平台，采用 **前后端分离 + 多角色** 架构，由学生端、社团管理员端与系统管理员端三部分组成，对应学生、社团负责人与学校管理部门三类使用场景。

平台围绕社团、活动、任务、器材与交流五条主线展开：学生可以浏览社团、报名活动、参与社区论坛、租赁器材、提交留言反馈并查看自己的社团、任务与报名；社团管理员负责入社申请审核、活动与任务维护、任务分配及器材租赁审批；系统管理员统筹社团列表、通知公告与留言反馈处理。

在智能化与数据化方面，系统结合任务标签、成员特长、活跃积分与历史完成情况，由 AI 辅助推荐任务执行成员并给出推荐说明，由社团管理员确认或调整后完成分配；同时基于协同过滤算法，根据学生兴趣、特长及相似同学的入社情况推荐社团并展示推荐理由；并以 ECharts 在控制台及社团、帖子、任务统计页面展示数量概况、分类分布、参与趋势与完成情况，帮助掌握社团运营与成员参与情况。

## 技术架构

| 类别 | 技术选型与说明 |
| :--- | :--- |
| 架构 | B/S、MVC、前后端分离、学生端+社团管理员端+系统管理员端、多角色管理 |
| 系统环境 | Windows |
| 开发环境 | IDEA、JDK17、Maven、MySQL、Node.js |
| 后端技术 | Java、Spring Boot 3.3.1、Spring MVC、MyBatis-Plus、MySQL、JWT、Apache POI、DeepSeek API |
| 网页前端技术 | Vue 3、Vite、Element Plus、Vue Router、Pinia、Axios、ECharts |

## 系统亮点

1. **AI辅助任务分配**：结合任务标签、成员特长、活跃积分与历史完成情况推荐执行成员，展示推荐说明，由社团管理员确认或调整后分配；学生提交成果后进入审核流程，便于跟进任务落实情况。

2. **协同过滤算法推荐**：根据学生兴趣、特长及相似同学的入社情况推荐社团，并展示推荐理由，帮助学生找到适合自己的校园组织。

3. **活动参与完整链路**：覆盖活动发布、学生报名、取消报名、签到及照片上传投票，将参与记录与活动成果集中展示，方便组织者管理活动。

4. **ECharts数据可视化**：通过控制台及社团、帖子、任务统计页面展示数量概况、分类分布、参与趋势和完成情况，辅助了解社团运营与成员参与情况。

5. **校园交流与反馈**：支持帖子点赞、收藏、评论和相关推荐，配合通知公告、私信与留言回复，让社团信息发布、成员交流和意见反馈形成连续流程。

6. **器材借还管理**：串联借用申请、审批、申请归还及归还确认，保留租借记录，方便社团跟踪器材使用与归还情况。


## 系统截图

> 截图存放于仓库 `images/` 目录，不依赖外部图床。

### 平台总览

<img src="images/01-system-overview.png" width="78%" alt="平台总览" />

**图 1 · 平台总览**

### 学生端

<img src="images/02-student-homepage.png" width="78%" alt="首页" />

**图 2 · 首页**

<img src="images/03-student-clubs.png" width="78%" alt="社团" />

**图 3 · 社团**

<img src="images/04-student-club-detail.png" width="78%" alt="社团详情" />

**图 4 · 社团详情**

<img src="images/05-student-club-activities.png" width="78%" alt="社团活动" />

**图 5 · 社团活动**

<img src="images/06-student-activity-detail.png" width="78%" alt="活动详情" />

**图 6 · 活动详情**

<img src="images/07-student-forum.png" width="78%" alt="社区论坛" />

**图 7 · 社区论坛**

<img src="images/08-student-equipment-rental.png" width="78%" alt="器材租赁" />

**图 8 · 器材租赁**

<img src="images/09-student-feedback.png" width="78%" alt="留言反馈" />

**图 9 · 留言反馈**

<img src="images/10-student-my-clubs.png" width="78%" alt="我的社团" />

**图 10 · 我的社团**

<img src="images/11-student-my-tasks.png" width="78%" alt="我的任务" />

**图 11 · 我的任务**

<img src="images/12-student-my-registrations.png" width="78%" alt="我的报名" />

**图 12 · 我的报名**


### 社团管理员端

<img src="images/13-club-admin-join-applications.png" width="78%" alt="入社申请" />

**图 13 · 入社申请**

<img src="images/14-club-admin-activity-list.png" width="78%" alt="活动列表" />

**图 14 · 活动列表**

<img src="images/15-club-admin-activity-stats.png" width="78%" alt="活动统计" />

**图 15 · 活动统计**

<img src="images/16-club-admin-task-list.png" width="78%" alt="任务列表" />

**图 16 · 任务列表**

<img src="images/17-club-admin-task-assignment.png" width="78%" alt="任务分配" />

**图 17 · 任务分配**

<img src="images/18-club-admin-post-list.png" width="78%" alt="帖子列表" />

**图 18 · 帖子列表**

<img src="images/19-club-admin-rental-list.png" width="78%" alt="租赁列表" />

**图 19 · 租赁列表**


### 管理员端

<img src="images/20-admin-club-list.png" width="78%" alt="社团列表" />

**图 20 · 社团列表**

<img src="images/21-admin-announcements.png" width="78%" alt="通知公告" />

**图 21 · 通知公告**

<img src="images/22-admin-feedback.png" width="78%" alt="留言反馈" />

**图 22 · 留言反馈**


---

**说明**：以上截图为系统部分功能演示页面，不同账号角色登录后可见菜单有所差异。

本项目仅用于学习交流，非商用、非开源、非无偿。

文档展示 22 张截图，需要了解更多，请联系我。
