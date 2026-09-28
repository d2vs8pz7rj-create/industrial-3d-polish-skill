# Industrial 3D Polish Skill

一个可迁移的 Codex skill：从多视角设备图片和可信尺寸开始，在 Blender 里完成比例校准、初模、制造结构、装配细化、材质选择、棚拍布光、渲染和逐轮回验。

## 安装

克隆或下载仓库，把 industrial-3d-polish 文件夹放入 Codex 的 skills 目录：

- Windows：%USERPROFILE%\.codex\skills\
- macOS / Linux：~/.codex/skills/

在任务中提供获授权的设备照片、尺寸和目标输出，然后说：

> 使用 industrial-3d-polish 技能，从这些图片建立可编辑设备模型。先校准多视角比例和结构，再逐步细化装配、材质、灯光和渲染；每阶段给我同机位检查图和推定项。

## 内容

- industrial-3d-polish/SKILL.md：完整执行顺序与阶段检查点
- industrial-3d-polish/references/photo-to-model.md：多视角图片校准与从 2D 建 3D
- industrial-3d-polish/references/blender-finish.md：结构收尾、材质、灯光、镜头和渲染
- industrial-3d-polish/references/quality-checks.md：检查证据、迭代记录和停止条件

仓库只包含通用方法，不包含任何设备模型、客户照片、品牌素材、私有路径、服务器地址或凭据。照片无法唯一确定被遮挡结构或制造尺寸；具体项目需要另行提供参考并标明推定范围。
