# Ash Engine

Ash Engine 是一个跨平台的 3D 引擎，基于 Qt、OpenGL 和 Assimp，仅用于学习用途。

## 截图

![](screenshots/screenshot0.jpg)

## 先决条件

* 需要 macOS 10.12+ 或 Windows x64 操作系统。
* 需要一张支持 OpenGL 3.3 或以上版本的图形卡，并安装好最新的驱动程序。

## 特点

* 友好、简洁、方便的用户界面，易于扩展。
* 支持读取 40 多种格式的 3D 模型文件，包括 FBX, DXF, Collada, Obj, X, PLY, 3DS 等。
* 支持读取和保存整个场景工程（使用本引擎定义的文件类型 `*.aeproj`）
* 使用树结构来描述场景，支持对模型（Model）和网格（Mesh）进行基本变换（平移、旋转、缩放）。
* 支持漫反射贴图、镜面反射贴图和法线贴图。
* 支持环境光、方向光、点光、聚光。每种光源类型支持最多 8 个，可对光源的颜色、位置、衰减等进行调整。

## 用法

### 打开场景

在菜单中选择 `File` --> `Open Scene`。

### 保存场景

在菜单中选择 `File` --> `Save Scene` 或 `Save Scene As`。

### 导入模型

在菜单中选择 `File` --> `Import Model`，或者直接将模型文件拖放到窗口。

### 导出模型

选中一个网格（Mesh）或模型（Model），在菜单中选择 `File` --> `Export Model`。

### 移动

* 使用 `W` 和 `S` 键来前进和后退
* 使用 `A` 和 `D` 键来左移或右移
* 使用 `E` 和 `Q` 键来上升或下降
* 使用 `Shift` 键来加速移动（5 倍速度）
* 按下鼠标左键并移动鼠标来调整视角

### 创建

在 `Create` 菜单中可以创建网格线、光源和基本体。

### 网格(Mesh)操作

在 `Mesh` 菜单中，支持给选中的网格赋予新材质、反转法线等。

### 三维小控件(Gizmo)

三维小控件可以帮助用户沿三维轴或平面移动、旋转或缩放一组对象，本程序支持的三维小控件包括：

* 三维移动小控件：沿轴或平面重新定位选定的对象
* 三维旋转小控件：绕指定轴旋转选定的对象
* 三维缩放小控件：沿指定平面或轴或沿全部三条轴统一缩放选定的对象

## 文档

文档将在 Wiki 中不定期更新。
