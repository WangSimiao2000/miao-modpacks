# 米奇喵整合包源 (Miao Modpacks Source)

> 状态：**Phase 1 实施期 fixture 仓库** — 待 MMCL Phase 1 (modpack source ecosystem) 完成后转为正式发布渠道。

这是 [MiaoMinecraftLauncher (MMCL)](https://github.com/WangSimiao2000/MiaoMinecraftLauncher) "整合包源生态"功能内置的默认源仓库。MMCL 启动器订阅本仓库，自动发现、解算、安装这里发布的整合包。

## 仓库结构

```
manifest.json                          源根 manifest（列出所有整合包）
packs/
  miao-1.21-base-test/
    pack.json                          整合包定义
    config/                            配置 overlay（按 MC 版本分支）
```

格式与字段定义见 [MMCL Phase 1 spec §2](https://github.com/WangSimiao2000/MiaoMinecraftLauncher/blob/main/docs/modpack-source-phase1-spec.md)。

## 当前整合包

| Pack ID | 显示名 | MC 版本 | Loader | 状态 |
|---|---|---|---|---|
| `miao-1.21-base-test` | 米奇喵 1.21 基础测试整合包 | 1.21.4, 1.21.5 | Fabric | active (fixture) |

## 内容信任

所有 mod 内容均托管在 Modrinth / CurseForge 平台，本仓库**仅声明 mod ID**，不直接分发任何 mod jar 文件。MMCL 启动器在玩家本地解算并下载。

## 作者

**mickeymiao (鄙人米奇喵)** — [Bilibili](https://space.bilibili.com/36913332)

## License

整合包元数据 (manifest.json / pack.json) 以 CC0 / Public Domain 发布，社区可自由参考、复制本仓库结构作为自己整合包源的模板。

每个 mod 各自的 license 由其原作者决定，本仓库仅声明 mod ID，不重新分发。
