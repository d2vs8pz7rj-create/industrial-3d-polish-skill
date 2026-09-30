# Industrial 3D Polish Skill

从设备照片到可信的 Blender 写实模型的通用 agent skill。适用于工业设备、机柜、工作站和其他硬表面产品：先校准图片与比例，再修正制造和装配结构，最后选择材质、棚拍灯光、镜头与渲染方案。每一轮修改都用同机位和相邻视角验证。

## 安装到另一台电脑

克隆或下载此仓库，把 industrial-3d-polish 文件夹放到用户技能目录：

- Windows：%USERPROFILE%\.agents\skills\
- macOS / Linux：~/.agents/skills/

如果只希望某个项目使用，可放到该项目的 .agents/skills/ 目录。也可以让 Codex 的 skill-installer 从本 GitHub 仓库安装。安装后在 Codex 中确认 industrial-3d-polish 可被发现；若刚安装后未显示，重启 Codex。

使用时提供获授权的参考照片、已知尺寸、现有模型和目标输出，然后要求 agent 使用 industrial-3d-polish。可从照片开始，也可从需要精修的粗模开始。

## 工作内容

- SKILL.md：全流程、决策顺序和参考文件入口
- photo-to-model.md：照片盘点、透视校准、多视角约束与灰模
- photo-to-geometry-playbook.md：部件地图、相机匹配循环、尺寸关系骨架、Blender 构造路线与表面资料提取
- geometry-and-assembly.md：钣金、孔、接缝、支撑、传动与紧固件等结构细化
- materials-and-surfaces.md：工艺识别、材质小样、微纹理、屏幕和玻璃
- lighting-and-rendering.md：棚景、反射、镜头、Cycles 渲染与成本控制
- failure-modes.md：常见“不真实”症状的排查顺序和修复路径
- quality-checks.md：阶段验收、版本保护、跨视角检查和交付记录
- execution-and-portability.md：agent 在 Blender 中的阶段产物与跨电脑重开、重渲染检查
- realtime-transfer.md：仅在需要交互展示时使用的材质与几何迁移检查

仓库不含任何项目设备模型、照片、商标、具体尺寸或账号信息。照片无法唯一确定被遮挡结构；视觉拟合不等于制造级 CAD。
