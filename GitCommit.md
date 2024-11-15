Write a concise commit message from 'git diff --staged' output in the format `[EMOJI] [TYPE](file/topic): [description in {locale}]`. Use GitMoji emojis (e.g., ✨ → feat), present tense, active voice, max 120 characters per line, no code blocks.A gitmoji commit message consists is composed using the following pieces:
``` 
intention: emoji and keyword, The intention you want to express with the commit, using an emoji from the list. Either in the :shortcode: or unicode format.
scope: An optional string that adds contextual information for the scope of the change.
message: A brief explanation of the change.
<intention> [scope?][:?] <message>
```
---
| Emoji | Code                        | Description           |
| ----- | --------------------------- | --------------------- |
| 🎉     | :tada:                      | 初次提交              |
| 🆕     | :new:                       | 引入新功能            |
| 🔖     | :bookmark:                  | 发行/版本标签         |
| 🐛     | :bug:                       | 修复 bug              |
| 🚑     | :ambulance:                 | 重要补丁              |
| 🌐     | :globe_with_meridians:      | 国际化与本地化        |
| 💄     | :lipstick:                  | 更新 UI 和样式文件    |
| 🎬     | :clapper:                   | 更新演示/示例         |
| 🚨     | :rotating_light:            | 移除 linter 警告      |
| 🔧     | :wrench:                    | 修改配置文件          |
| ➕     | :heavy_plus_sign:           | 增加一个依赖          |
| ➖     | :heavy_minus_sign:          | 减少一个依赖          |
| ⬆️     | :arrow_up:                  | 升级依赖              |
| ⬇️     | :arrow_down:                | 降级依赖              |
| ⚡     | :zap:                       | 提升性能              |
| 🐎     | :racehorse:                 | 提升性能              |
| 📈     | :chart_with_upwards_trend:  | 添加分析或跟踪代码    |
| 🚀     | :rocket:                    | 部署功能              |
| ✅     | :white_check_mark:          | 增加测试              |
| 📝     | :memo:                      | 撰写文档              |
| 📖     | :book:                      | 撰写文档              |
| 🔨     | :hammer:                    | 重大重构              |
| 🎨     | :art:                       | 改进代码结构/代码格式 |
| 🔥     | :fire:                      | 移除代码或文件        |
| ✏️     | :pencil2:                   | 修复 typo             |
| 🚧     | :construction:              | 工作进行中            |
| 🗑️     | :wastebasket:               | 废弃或删除            |
| ♿     | :wheelchair:                | 可访问性              |
| 👷     | :construction_worker:       | 添加 CI 构建系统      |
| 💚     | :green_heart:               | 修复 CI 构建问题      |
| 🔒     | :lock:                      | 修复安全问题          |
| 🐳     | :whale:                     | Docker 相关工作       |
| 🍎     | :apple:                     | 修复 macOS 下的问题   |
| 🐧     | :penguin:                   | 修复 Linux 下的问题   |
| 🏁     | :checkered_flag:            | 修复 Windows 下的问题 |
| 🔀     | :twisted_rightwards_arrows: | 分支合并              |
---
example:
```
 ♻️refactor(WegicSeoSiteService): 提升网站类型处理逻辑

- 移除`webInfo`检查中的`siteType`空校验，替换为自动生成。
- 引入`JsAIService`中的`createWebType`方法以生成网站类型。
```
---
{diff}