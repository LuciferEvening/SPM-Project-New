# 06 团队协作指南

## 面向组员：rookiedude

### 一、准备工作

#### 1. 安装 Trae
- 在你的电脑上下载并安装 Trae IDE
- 打开 Trae，进入任意项目目录

#### 2. 配置 Git 用户信息
打开终端，执行以下命令：
```bash
git config --global user.name "rookiedude"
git config --global user.email "你的邮箱地址"
```

> ⚠️ 注意：用户名必须前后一致，用于识别你的贡献

### 二、获取项目代码

#### 1. 克隆仓库
```bash
git clone https://github.com/LuciferEvening/SPM-Project-New.git
cd SPM-Project-New
```

#### 2. 创建你的工作分支
```bash
git checkout -b feature-rookiedude
```

### 三、开始工作

#### 1. 查看当前状态
```bash
git status
```

#### 2. 修改文档
你负责的任务：
- 完善 WBS 文档（docs/02-wbs.md）
- 完善进度计划（docs/03-schedule.md）
- 参与总结报告编写（docs/05-summary-report.md）

#### 3. 提交修改
```bash
# 添加修改的文件
git add docs/02-wbs.md docs/03-schedule.md

# 提交（写清楚做了什么）
git commit -m "feat: 完善WBS三级分解"

# 推送到远程仓库
git push origin feature-rookiedude
```

### 四、协作流程

```
创建分支 → 修改文档 → 提交 → 推送 → 通知项目经理合并
```

### 五、提交信息规范

| 类型 | 说明 | 示例 |
|---|---|---|
| feat | 新功能/完善内容 | feat: 添加活动管理WBS条目 |
| fix | 修复问题 | fix: 修正进度计划日期 |
| docs | 文档更新 | docs: 更新总结报告 |
| merge | 分支合并 | merge: 合并到dev分支 |

### 六、保持同步

每次开始工作前，先同步最新代码：
```bash
git checkout dev
git pull origin dev
git checkout feature-rookiedude
git merge dev
```

### 七、遇到问题？

1. **冲突问题**：
   ```bash
   # 查看冲突文件
   git status
   # 手动编辑冲突文件，然后提交
   git add .
   git commit -m "fix: 解决冲突"
   ```

2. **忘记配置用户名**：
   ```bash
   git config user.name "rookiedude"
   ```

### 八、任务清单

| 任务 | 状态 |
|---|---|
| [ ] 完善 WBS 文档（三级分解） |
| [ ] 完善进度计划（活动列表、工期、责任人） |
| [ ] 参与冲突解决（修改 conflict.md） |
| [ ] 参与总结报告编写 |

---

**项目经理：王其潇（wangqixiao）**
**协作成员：rookiedude**

完成任务后通知项目经理合并到 dev 分支！
