# 如何将项目推送到GitHub

## 方法1: 使用GitHub网页创建仓库

1. 访问 https://github.com/new
2. 填写仓库信息:
   - Repository name: `snake-game`
   - Description: `经典贪吃蛇游戏 - HTML5 Canvas实现`
   - 选择 Public 或 Private
   - **不要**勾选 "Initialize this repository with a README"
3. 点击 "Create repository"
4. 在终端执行以下命令:

```bash
cd ~/Desktop/snake
git remote add origin https://github.com/YOUR_USERNAME/snake-game.git
git branch -M main
git push -u origin main
```

## 方法2: 使用GitHub CLI (需要先安装)

安装GitHub CLI:
```bash
brew install gh
```

然后执行:
```bash
cd ~/Desktop/snake
gh auth login
gh repo create snake-game --public --source=. --remote=origin --push
```

## 当前项目状态

✅ 项目已创建在: ~/Desktop/snake
✅ Git仓库已初始化
✅ 代码已提交到本地仓库
⏳ 等待推送到GitHub远程仓库

## 项目文件

- `index.html` - 完整的贪吃蛇游戏（包含HTML、CSS、JavaScript）
- `README.md` - 项目说明文档
- `.git/` - Git版本控制目录

## 游戏功能

🎮 键盘控制: 方向键或WASD
🖱️ 鼠标控制: 点击屏幕按钮
📊 得分系统: 自动保存最高分
⏸️ 暂停功能: 空格键或点击按钮
🎨 精美UI: 渐变设计和发光效果
