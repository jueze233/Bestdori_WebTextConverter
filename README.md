# BanG Dream! 剧情文本转换器 - 功能全览

这是一个专为 BanG Dream! (Bestdori) 社区设计的剧情文本转换工具，可以将普通对话文本转换为 Bestdori 平台可用的 JSON 格式。

通过网页来访问这个工具：
[https://bestdori-webtextconverter.zeabur.app/](https://bestdori-webtextconverter.zeabur.app/)

---

## 📝 核心功能

### 1. 文本转换
- 将对话文本自动转换为 Bestdori JSON 格式
- 智能识别角色对话和旁白内容
- 支持多种对话格式 (`角色名：对话` 或 `角色名: “对话”`)
- 自动处理空行作为段落分隔

### 2. 文件支持
- 支持上传 `.txt`、`.docx`、`.md` 三种格式
- 支持拖拽上传文件
- 批量处理多个文件，生成 ZIP 压缩包下载

### 3. 引号处理
- 预设 6 种常用引号格式：
    - 中文引号 `“`...`”`
    - 中文单引号 `‘`...`’`
    - 日文引号 `「`...`」`
    - 日文书名号 `『`...`』`
    - 英文双引号 `"`...`"`
    - 英文单引号 `'`...`'`
- 支持添加自定义引号对
- 自动移除对话首尾的引号

---

## 👥 角色管理

### 1. 角色映射配置
- 内置全部 45 个 BanG Dream! 角色：
    - **Poppin'Party** (5人)
    - **Afterglow** (5人)
    - **Hello, Happy World!** (5人)
    - **Pastel*Palettes** (5人)
    - **Roselia** (5人)
    - **Morfonica** (5人)
    - **RAISE A SUILEN** (5人)
    - **MyGO!!!!!** (5人)
    - **Ave Mujica** (5人)
- 支持添加自定义角色
- 支持角色别名（相同ID不同名称）
- 角色头像显示（40个角色头像）

### 2. 特殊处理
- Ave Mujica 成员特殊ID映射 (`337-341` → `1-5`)
- 自动处理角色ID冲突

---

## 🎭 Live2D 布局系统

### 1. 自动布局
- 为首次出现的角色自动生成 layout action
- 智能管理角色出场顺序

### 2. 服装配置
- 每个角色独立的服装管理
- 支持从预设服装列表选择
- 支持添加自定义服装ID
- 服装列表的增删改功能
- 角色别名独立服装配置

---

## 🖥️ 界面功能

### 1. 双视图模式
- **经典视图**：传统的表单式界面
- **分屏编辑**：左侧编辑，右侧实时预览

### 2. 预览功能
- JSON 格式预览
- 对话模拟预览（模拟 Bestdori 显示效果）
- 自动预览开关
- 可调整分屏大小

### 3. 文本编辑
- 格式化文本功能（自动整理段落间距）
- 实时字数统计
- 语法高亮显示

---

## 💾 数据管理

### 1. 配置导入/导出
- 导出完整配置文件（JSON格式）：
    - 角色映射
    - 自定义引号
    - 服装配置
    - Live2D 设置
- 支持导入配置文件
- 向后兼容旧版本配置

### 2. 本地存储
- 所有配置保存在浏览器本地
- 自动保存用户偏好设置
- 数据持久化存储

### 3. 重置功能
- 角色配置重置（保留服装配置）
- 服装配置重置（保留自定义角色配置）
- 智能重置，不会丢失重要数据

---

## 🚀 高级功能

### 1. 批量处理
- 同时处理多个文件
- 实时显示处理进度
- 详细的处理日志
- 一键下载所有结果（ZIP格式）

### 2. 响应式设计
- 适配桌面和移动设备
- 流畅的动画效果
- 现代化的UI设计

### 3. 错误处理
- 智能的错误提示
- 数据验证机制
- 防止意外数据丢失

---

## 安装要求

### 环境要求
- Python 3
- pip (Python 包管理器)

### 安装步骤
1.  **首先确保您的系统已安装 Python 3**
    ```bash
    # 检查 Python 版本
    python --version
    # 或
    python3 --version
    ```

2.  **克隆仓库**
    ```bash
    # 克隆仓库
    git clone https://github.com/jueze233/Bestdori_WebTextConverter.git

    # 进入项目目录
    cd Bestdori_WebTextConverter
    ```

3.  **安装依赖**
    ```bash
    # 安装项目依赖
    pip install -r requirements.txt
    ```

4.  **启动项目**
    ```bash
    # 运行应用
    python app.py
    # 或
    python3 app.py
    ```

---

## 许可证

本项目采用 MIT 许可证。
