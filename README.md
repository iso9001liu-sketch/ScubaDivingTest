# 蓝洞边缘 · ScubaDivingTest

一款单文件、无需安装的 2D 水肺潜水观察模拟。打开 `dist/index.html` 即可游玩。

## 操作
- 方向键 / WASD：水平游动、上升与下潜
- 触屏方向按钮：按住连续游动
- “观察视野”：只记录当前深度且实际出现在画面中的鱼；无目标时显示未发现
- 选择 OW（18m）或 AOW（30m）训练模式

## 生态与场景
礁鱼按代表性活动水层生成，各物种有独立体型、颜色/花纹和活动深度；随着深度与礁壁位置变化，鱼群进入或离开观察画面。礁壁、平台、沙地和开阔水域构成连续可游区域，无左边界墙。

物种分布是热带珊瑚礁的代表性教学近似，不对应单一真实潜点。浅水礁鱼受深度与珊瑚生长光照带影响；鹦嘴鱼、蝴蝶鱼等可见于较宽水深，部分蝴蝶鱼与礁鱼在更深礁坡仍有记录。可参阅 [NOAA 珊瑚礁栖息地说明](https://www.fisheries.noaa.gov/national/habitat-conservation/shallow-coral-reef-habitat)、[Florida Museum 蝴蝶鱼资料](https://www.floridamuseum.ufl.edu/discover-fish/species-profiles/reef-butterflyfish/) 和 [Stoplight Parrotfish 资料](https://www.floridamuseum.ufl.edu/discover-fish/species-profiles/stoplight-parrotfish/)。

## 参考项目与许可
程序化鱼群分布、连续游动和分层水下视觉的设计思路参考公开项目 [Yohans' Reef](https://github.com/chintagunta/aquarium-relax)。未复制其代码或素材；该项目页面未明确显示许可证，因此本游戏保持独立实现。游戏内鱼类形态由 Canvas 程序绘制。

## 模型说明
压力约每 10m 增加 1 ATA；水面耗气率按 20 L/min 并随压力倍增；氮负荷为简化提示。仅用于教学演示，不可用于真实潜水计划。请遵循持证教练、潜伴和潜水电脑指导。

GitHub Pages 由 GitHub Actions 自动部署。