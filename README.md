# 草地 Q 弹小人

把表情包小人摆到那片经典草坡上，点一下全体 Q 弹的网页小玩具。

纯静态页面，双击 `index.html` 就能玩，不需要装任何东西、也不需要联网。

## 玩法

| 操作 | 效果 |
| --- | --- |
| 右上角「开始Q弹」 | 所有角色一起上下弹（带挤压/拉伸），空格也能开关 |
| 弹跳幅度 | 0.50× – 2.00×，只放大上下位移 |
| 弹跳速度 | 0.50× – 2.00×，1.00× 时一轮 0.4 秒 |
| 隐藏操作台 | 面板 + 鼠标一起藏起来，点鼠标或按右 Shift 召回 |
| 左上角红点 | 别按 |

## 编辑模式

点「✎ 调整位置 / 大小 / 翻转 / 图层」进入：

- **拖动角色** → 换位置
- **拖右下角小圆点** → 改大小（30% – 260%）
- **⇄ 左右翻转这只** → 单独镜像这一个角色
- **图层** → 上移一层 / 下移一层 / 置顶 / 置底
- **复位** → 还原这只 / 全部还原

所有改动自动存进浏览器 localStorage，下次打开还是你摆的样子。

## 部署到 GitHub Pages

1. 在 GitHub 新建一个**空仓库**（不要勾选 README / .gitignore）
2. 本地跑：

   ```bash
   git remote add origin https://github.com/<你的用户名>/<仓库名>.git
   git push -u origin main
   ```

   提示输入密码时，用 **Personal Access Token**（GitHub → Settings → Developer settings → Personal access tokens），不要用账号密码。

3. 仓库 → Settings → Pages → Source 选 `Deploy from a branch`，分支 `main`，目录 `/ (root)`，保存
4. 等一分钟，访问 `https://<你的用户名>.github.io/<仓库名>/`

## 目录结构

```
index.html              页面本体（HTML + CSS + JS 都在里面）
assets/
  grass.jpg             草坡背景（已左右镜像）
  01_昔涟.png … 14_万敌.png   角色贴图
```

## 说明

角色贴图来自游戏《崩坏：星穹铁道》，版权归米哈游所有；这里只作同人 / 个人演示用途，请勿商用。
