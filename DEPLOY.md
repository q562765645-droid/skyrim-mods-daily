Nexus Mods Skyrim SE 每日热门 Mod 推送
=====================================

## 部署到 GitHub Pages

### 步骤：

1. 创建 GitHub 仓库
   - 登录 GitHub，新建仓库（例如 `skyrim-mods-daily`）
   - 设为 Public

2. 上传文件
   - 把 `index.html` 上传到仓库根目录
   - 提交并推送

3. 启用 GitHub Pages
   - 进入仓库 Settings → Pages
   - Source 选择 "Deploy from a branch"
   - Branch 选择 "main" / "(root)"
   - 点击 Save

4. 等待 1-2 分钟，访问：
   `https://你的用户名.github.io/skyrim-mods-daily/`

### 更新内容：
每次推送新 mod 时，更新 `index.html` 中的 `MOD_DATA` 数组即可。

### 本地预览：
```bash
python3 -m http.server 8888
# 然后访问 http://localhost:8888
```
