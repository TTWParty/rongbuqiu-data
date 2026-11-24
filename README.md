# rongbuqiu-data

**绒布球生图（[TTWParty/rongbuqiu](https://github.com/TTWParty/rongbuqiu)）独立云端数据包仓库。**

将大规模双语词库与 V5 视觉配方库与插件本体解耦，插件内可一键检查、下载与热更新（自动通过 jsDelivr CDN / GitHub Raw 多线路回退，本地缓存于浏览器 IndexedDB，无需升级插件即可持续扩充最新角色、画师、Tag 与视觉配方）。

## 数据包目录

| 文件 | 说明 | 格式 |
| --- | --- | --- |
| `manifest.json` | 索引清单（版本号、条数、体积、SHA-256 校验值） | JSON |
| `packs/tags-100k.tsv.gz` | 100,020 条 Danbooru + NovelAI V5 全量中英双语词库（含 3.5 万角色、2.4 万画师、8.4 千作品、3 万常规 Tag 与完整中文别名） | Gzip 列式 TSV |
| `packs/recipes-v5.json.gz` | 2,980 套零发色污染 V5 视觉动作、场景、穿搭与构图配方库（含 261 套精编核心与世界书全量蒸馏扩展动作/服饰/速查表） | Gzip JSON |

## 数据来源与许可

- 本仓库采用 **MIT License** 开源。
- `packs/tags-100k.tsv.gz` 中的 Danbooru 中文译名、别名与热度数据基于 MIT 开源项目 [amenorira/danbooru-tags-data-zh](https://github.com/amenorira/danbooru-tags-data-zh) 编译整理，特此致谢。
