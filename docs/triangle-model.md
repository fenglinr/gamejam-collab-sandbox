# 第一个 Blender 模型：三角形

通过 Blender MCP 在 Blender 5.2.3 LTS 中制作。

![三角形预览](previews/triangle.png)

| 文件 | 用途 |
| --- | --- |
| [triangle.blend](../art-source/props/triangle/triangle.blend) | 在 Blender 中继续编辑的源文件 |
| [triangle.glb](../game/assets/props/triangle/triangle.glb) | 交给 Godot 使用的模型 |
| [triangle.png](previews/triangle.png) | 512 × 512 透明背景预览图 |

模型是边长 2 个 Blender 单位的平面等边三角形，3 个顶点、3 条边、1 个面，没有厚度，使用绿色双面材质。Blender 中位于 XY 平面，法线朝 +Z；GLB 导出按 glTF 的 Y 向上坐标约定转换。

源文件带有预览用的相机和灯光，GLB 只导出 `JamTriangle`，不包含相机或灯光。预览输出位置使用相对路径，其他电脑克隆后可重新渲染。

## 在 GitHub Desktop 中拿到这项任务

点“获取更新 / Fetch origin”，在“当前分支 / Current branch”里选择 `task/blender-triangle`。Git LFS 会取回源文件与导出资产。源文件在 `art-source/props/triangle/`，双击即可用 Blender 打开。

这项任务在独立分支中交付；检查后再把分支合入 `main`。以后继续编辑 `.blend` 前按仓库约定取得文件锁。

## 本次检查

- 用新的 Blender 后台进程重新打开源文件，核对顶点、边、面和三个等长边。
- 检查 GLB 文件：只有一个模型节点，3 个顶点、1 个三角面，双面材质，无相机或灯光。
- 查看 Blender 实际渲染的透明背景预览图。

尚未在正式 Godot 游戏中接入；这个练习仓库目前没有可运行的 Godot 项目。
