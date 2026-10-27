# 运营补丁 OPS-20261026（主人授权：A1–A4 + B1–B5；B6 搁置）

不改 Goal/合同/已签 hash。覆盖 RB 技能与例行的增量约定；与 00/01 冲突时以本补丁 + 更新后的 skills 为准。

- A1 噪音：ACK/停等/预告/无变化不进主会话
- A2/B4 attempt：派工带 attempt；席位只认最新
- A3 Mac 离线降级：预签可、合闸等上线；只提醒一次
- A4 残余授权清单一次勾
- B1 门审两段：预签≠合闸；承重链已签收仅合闸
- B2 纯门审/复测不占 RUNNING
- B3 承重链 box 镜像 `/workspace/load-bearing-mirror/`
- B5 晨报/巡检含预签未合闸栏
