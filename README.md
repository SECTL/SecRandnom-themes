# SecRandom Themes Index

## 提交主题

请在 `index/themes/` 目录下创建一个新的 YAML 文件，文件名格式建议为 `作者名.主题名.yml`（例如 `lzy98276.testrollcalltheme.yml`）。

文件内容格式如下：

```yaml
id: lzy98276.testrollcalltheme  # 主题唯一 ID
name: 点名界面主题(测试)           # 主题主题
description: 仅限测试使用！       # 主题描述
url: https://github.com/lzy98276/TestRollcallTheme # 主题项目主页 URL
author: lzy98276                # 作者名称
version: 1.0.0                  # 主题版本
apiVersion: 2.3.0-beta.1        # 支持的最低软件 API 版本
repoOwner: lzy98276             # GitHub 仓库所有者
repoName: TestRollcallTheme     # GitHub 仓库名称
assetsRoot: master/TestRollcallTheme # 资源文件在仓库中的根目录
artifactName: TestRollcallTheme.zip  # 资源文件名
banner: banner.png              # 横幅图片路径（可选）
```

提交 Pull Request 后，系统会自动进行格式检查并自动合并。

## 主题规范

### 文件类型限制
主题仅支持包含以下类型的文件：
- Python (`.py`)
- HTML (`.html`)

### 目录结构要求
根据主题功能类型，请将文件存放在对应文件夹中，且入口文件名称为main：
- **点名页面**：存放在主题ID文件夹下的 `Roll_call_page` 目录
- **抽奖页面**：存放在主题ID文件夹下的 `Lottery_page` 目录

主题ID文件夹下还需放置一个包含版本号和主题ID的JSON文件，文件名为 `manifest.json`：

```json
{
  "id": "lzy98276.testrollcalltheme",
  "version": "1.0.0",
  "url": "https://github.com/lzy98276/TestRollcallTheme"
}
```

### 源代码参照
主要源代码页面请参照以下链接：
- **点名页面**：https://github.com/SECTL/SecRandom/blob/master/app/view/main/roll_call.py
- **抽奖页面**：https://github.com/SECTL/SecRandom/blob/master/app/view/main/lottery.py

**注意：如果使用HTML将无法接入SecRandom的通用函数。**
