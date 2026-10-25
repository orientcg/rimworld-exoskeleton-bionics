# 外骨骼装甲 / Exoskeleton Bionics

![外骨骼装甲](About/Preview.png)

RimWorld **1.6 / 1.7** 的独立外骨骼 Mod，发布版本 **0.14.0**。本仓库只包含游戏运行文件和说明。

- 14种核心与四肢物品；核心永久植入，四肢通过“外骨骼管理”装卸、更换。
- 集齐左右手臂与左右腿后，过载触发20帧机甲变身；能量独立结算，亲自击杀回能。
- 核心与四肢共5件计级：蓝色／工业红色过载×1.5，金色×2.5。
- 吸收100单位金属形成护甲血条，承担75%生命伤害；破甲使核心停机2游戏小时。
- 同页管理金属与四肢；护甲血条位于能量条上方。

## 安装

1. 点击本页 **Code → Download ZIP**，解压。
2. 将包含 `About`、`Common`、`LoadFolders.xml`、`1.6`、`1.7` 的整个目录放入 RimWorld 的 `Mods` 目录。
3. 在游戏的 Mod 列表启用“外骨骼仿生体 / Exoskeleton Bionics”，重启游戏。

只启用一个副本，不要同时加载本地版和同一Mod的工坊版。游戏会自动选择对应的版本目录。Harmony已内置；军用内容沿用皇权DLC条件。

工坊条目：[3826026606](https://steamcommunity.com/sharedfiles/filedetails/?id=3826026606)。本仓库上传不代表已更新Steam创意工坊。

## 兼容与验证

1.7版基于1.7.4985编译，使用.NET 10与Harmony 3；1.6版保留原0.13.3 DLL与Harmony 2.4.3。物品定义、语言、贴图与许可在 `Common` 中共用，版本目录只放对应程序集。

```text
About/               Mod信息、封面和工坊编号
Common/
  Defs/              共用物品与功能定义
  Languages/         共用中英文文本
  Textures/          共用贴图
  Licenses/          Harmony许可
1.6/Assemblies/      1.6专用Mod DLL与Harmony 2
1.7/Assemblies/      1.7专用Mod DLL与Harmony 3
LoadFolders.xml      每个版本加载Common及自身目录
```

此结构通过加载路径共用同一套资源；两个版本的程序集分别保留，不能互换。后续若出现版本专用定义或贴图，可放入对应版本目录，避免复制全部公共内容。

已通过625项1.7隔离引擎检查，覆盖变身／战斗、金属护甲、管理界面、独立能量与旧存档迁移。用户殖民地与第三方Mod组合仍需实际验收。

## 第三方许可

Harmony的MIT许可保留于 `Common/Licenses/Harmony-MIT.txt`。游戏原始参考素材、开发源码、工具、测试、原画和历史备份均不包含在本仓库。
