# 编译期依赖 jar（不入库）

本目录存放构建所需的游戏本体与加载器 / 基础库 jar，供顶层 `pom.xml` 以 `system` scope 引用。
`*.jar` 由顶层 `.gitignore` 统一忽略，**不要提交**。

| 文件 | 来源 | 版本 |
| :--- | :--- | :--- |
| `desktop-1.0.jar` | 游戏本体（Steam app 646570，游戏根目录） | 补丁 `12-18-2022` |
| `ModTheSpire.jar` | Steam 创意工坊 `646570/1605060445` | 3.30.3 |
| `BaseMod.jar` | Steam 创意工坊 `646570/1605833019` | 5.56.0 |
| `StSLib.jar` | Steam 创意工坊 `646570/1609158507` | 2.12.0 |

也可手动放入游戏目录 `mods/`（两种安装方式等价，见 `specs/001-anthonys-wrath/quickstart.md` §1）。
版本号以顶层 `pom.xml` 的 `<properties>` 为唯一事实来源（宪法引言）。
