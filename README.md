# AdminLog_PreWork
- **Our Team**: **The Bug Killers**
- **成绩构成: 三次小作业 30% + MOOC考勤 10% + 大作业 60%**
- **评测标准：结果交付40%(代码规范10%+功能实现20%+前端风格10%) + 答辩演示40% + 文档20%**
# 选题: 综10——用户行为日志管理
- 技术栈: **vue** + **python** + **日志存储**
- 需求: 为FloK系统设计一套用户行为日志管理系统，存储用户的行为数据(*访问、浏览、搜索、点击、查询*)
- 关于**文档要求**以及**结果交付**：详见作业要求文档 & 开发文档
## 基本要求
- 使用**Vue框架**为日志系统设计一个前端页面，并集成到FloK系统中
- 调研现有系统日志工具，包括**日志管理和存储**等方面
- 对FloK系统**用户**行为进行**建模**，设计日志存储方式
- 实现*写入*日志、***查询***日志、***筛选***日志等功能
## 进阶要求
- 丰富用户行为信息，如**页面停留时长**、**浏览器和IP**等
- 针对不同类型的行为数据选择**不同可视化方式**展现统计信息
## 开发流程
### 代码工程准备
- [x] 每位同学准备github账号 
- [ ] 组长提供github账号给负责助教
- [ ] 组长fork工程至个人仓库
- [ ] 对各自的工程给组员赋予权限
- [ ] 各组员建立各自分支
- [ ] 各组员克隆代码至本地，准备后续开发工作

### 开发环境准备
#### 后端调试环境准备
- [x] 需要一个Ubantu 16.04 + Python 3.7的环境作为服务器，可以是虚拟机或者云服务器等
- [ ] 将本地代码上传至服务器（也可以使用git管理）
- [ ] 在服务器端
  cd 项目工程目录/FloK
  pip install -r requirements.txt
  cd flok
  sh run.sh

#### 前端开发环境准备
- 在本地机器上，需支持npm
  cd 项目工程目录/flok/vue-frontend/
  npm install
  安装无误后
  修改vue-frontend目录下的vue.config.js配置的后端工程ip
  npm run serve（启动工程）

#### 数据库准备
- 准备一个数据库连接工具（如Navicat/DataGrip/PyCharm插件..)
  连接数据库，创建数据库副本
  服务器端修改flok.cfg
  sh run.sh 重启后端


### 设计
- 根据选题内容，组内进行讨论设计，如有需调研，则需先调研行程调研文档，**完成设计文档**，交由助教审阅
  在审阅通过后方可进入后续开发阶段，设计也会随开发过程不断迭代完善，**积极与负责人沟通设计方向**

### 开发及调试
#### 前端开发及调试
- 有前端修改后，在npm run serve启动状态下，可以访问前端服务器地址即可查看修改


#### 后端开发及调试
- 在本地开发修改后，将修改上传至服务器，只要保证后端启用中，修改自动刷新

#### 数据库内容更改
- 仅能在自己组创建的副本上更改，不可修改或删除其他database
  将修改的sql语句记录下来，随测试报告提交

#### 在各自完成一个完整功能点并调试无误后
- 在本地git工程上git commit修改
  git push到远端
  向主分支提pr合并，由组长进行审核及合并

### 测试及交付
#### 开发同学
- 自行开发功能并**完成相关文档**
  开发完成的代码**合并至**项目任务组长分支
  **提供测试报告（包括测试示例）**

#### 项目组长
- **合并代码**/code review/**功能验证**/**文档验收**
  对合并的代码进行review，确认合并的代码**符合**开发**规范**，**没有冲突**，使用正确技术栈，数据库改动正确，没有硬编码等
  对合并的功能进行review，确认合并的功能符合设计，功能使用无问题等
  对合并的功能文档进行验收整合，**形成完整文档提交**
  对已验证完的分支可以对**项目任务负责人**提出**pr申请**

### 答辩

- 技术讲解
- 单元测试结果
- 项目演示

