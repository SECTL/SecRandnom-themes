# SecRandom Themes Index

## 提交主题

请在 `index/themes/` 目录下创建一个新的 YAML 文件，文件名格式建议为 `作者名.主题名.yml`（例如 `lzy98276.testrollcalltheme.yml`）。

文件内容格式如下：

```yaml
id: lzy98276.testrollcalltheme  # 主题唯一 ID
name: TestRollcallTheme         # 主题名称
description: 点名界面主题(测试)   # 主题描述
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
