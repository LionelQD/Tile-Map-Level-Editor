# Tile Map Level Editor
# 瓦片地图关卡编辑器

A lightweight, standalone 2D tile map editor built for game developers. Import your tilesets, paint levels across multiple layers, and export to JSON or CSV for any game engine.
一款为游戏开发者打造的轻量、免安装 2D 瓦片地图编辑器。支持导入瓦片集、多图层绘制关卡，并可导出为 JSON 或 CSV 格式，适配任意游戏引擎。
<img width="2040" height="1366" alt="1772519709158_d" src="https://github.com/user-attachments/assets/7bd2caf7-338c-4542-8288-94e51832779c" />

---

## What is it?
## 产品简介

Tile Map Level Editor is a free, portable desktop tool for designing 2D tile-based game levels. No installation required -- just download, run, and start building. It supports multi-layer editing, multiple tilesets, and exports to standard formats that integrate with any game engine or custom pipeline.
瓦片地图关卡编辑器是一款免费、便携的桌面工具，专为设计 2D 瓦片式游戏关卡而生。无需安装——下载即运行，开箱即可创作。支持多图层编辑、多瓦片集管理，导出格式通用，可无缝对接任意游戏引擎或自定义工作流。

Built with simplicity in mind: no bloated features, no steep learning curve. Open the app, import a spritesheet, and start placing tiles.
设计理念极简：无冗余功能，无陡峭学习成本。打开软件、导入精灵图集，就能开始放置瓦片。

---

## Key Features
## 核心功能

**Multi-Layer Editing**
**多图层编辑**
Create and manage multiple layers with independent visibility and lock controls. Organize your terrain, decorations, collision, and foreground elements on separate layers. Reorder, rename, show/hide, or lock layers as needed.
创建并管理多个图层，支持独立控制显示/隐藏、锁定。可将地形、装饰、碰撞、前景元素分图层整理，按需调整图层顺序、重命名、显示/隐藏或锁定。

**Flexible Tileset Management**
**灵活的瓦片集管理**
Import any number of tilesets from PNG, JPG, BMP, or GIF images. The editor auto-detects tile size from common formats (8, 16, 32, 48, 64px) or lets you set custom dimensions. Each tileset displays in a zoomable, scrollable palette panel with collapse/expand support.
支持从 PNG、JPG、BMP、GIF 图片导入任意数量瓦片集。编辑器可自动识别常见瓦片尺寸（8、16、32、48、64px），也支持自定义尺寸。所有瓦片集在可缩放、可滚动的面板中展示，支持折叠/展开。

**Drawing Tools**
**绘制工具**
- **Brush (B)** -- Click or drag to paint tiles. Hold Shift while dragging to constrain to straight lines (horizontal/vertical).
  **画笔（B）** —— 点击或拖拽绘制瓦片；拖拽时按住 Shift 可强制水平/垂直直线绘制。
- **Eraser (E)** -- Click or drag to remove tiles. Right-click anywhere for quick erase.
  **橡皮擦（E）** —— 点击或拖拽擦除瓦片；任意位置右键可快速擦除。
- **Fill (F)** -- Click for flood fill or drag to fill a rectangular area.
  **填充（F）** —— 点击进行泛洪填充，或拖拽填充矩形区域。

**Canvas Navigation**
**画布操作**
- Hold **Space + drag** or **Middle mouse drag** to pan the canvas freely.
  按住 **空格+拖拽** 或 **鼠标中键拖拽** 自由平移画布。
- **Ctrl + Mouse Wheel** to zoom in/out.
  **Ctrl+鼠标滚轮** 缩放画布。
- **Home** to reset and center the view.
  **Home** 重置并居中视图。
- Hover highlight shows exactly which cell you're targeting.
  悬停高亮，精准显示当前选中单元格。

**Anchor-Based Map Resize**
**基于锚点的地图尺寸调整**
Change your map dimensions at any time. Choose from 7 anchor points (corners, edges, center) to control how existing tiles shift during resize. Never lose your work when adjusting canvas size.
可随时修改地图尺寸。提供 7 个锚点（四角、四边、中心），缩放时控制瓦片偏移方式，调整画布尺寸时不会丢失任何内容。

**Canvas Background Color**
**画布背景色**
Pick from preset colors or choose any custom color for the canvas background. Useful for previewing levels against different game backgrounds.
支持选用预设色或自定义任意背景色，方便在不同游戏背景下预览关卡。

**Dark / Light Theme**
**深色/浅色主题**
Switch between a dark theme (easy on the eyes during long sessions) and a light theme with a single click.
一键切换护眼深色主题与浅色主题。

**Bilingual Interface**
**双语界面**
Full English and Simplified Chinese language support. Toggle between EN and CN at any time -- all menus, dialogs, labels, and messages switch instantly.
完整支持英文/简体中文，可随时切换，所有菜单、弹窗、标签、提示文字即时生效。

**Undo / Redo**
**撤销/重做**
Full undo/redo support for all operations: painting, erasing, filling, layer changes, map resize, and more. Every brush stroke is batched into a single undo step for efficient history management.
全操作支持撤销/重做：绘制、擦除、填充、图层修改、地图尺寸调整等。每笔绘制会合并为一个撤销步骤，历史记录管理更高效。

---

## Export Formats
## 导出格式

| Format | Description |
|--------|-------------|
| **.tlemap** | Native project format. Saves complete editor state: map dimensions, all tilesets, all layers, every tile placement, layer order and settings. Reopen and continue editing at any time. |
| **.tlemap** | 原生项目格式，保存完整编辑状态：地图尺寸、瓦片集、图层、瓦片摆放、图层顺序及设置，可随时打开继续编辑。 |
| **JSON** | Single-file export containing map dimensions, cell sizes, tileset metadata, and all layer tile data. Ready for parsing in any game engine. |
| **JSON** | 单文件导出，包含地图尺寸、单元格大小、瓦片集元数据和所有图层瓦片数据，可直接在游戏引擎中解析。 |
| **CSV** | One CSV file per layer. Grid format with tile references (`tileset_id:tile_x:tile_y`). Easy to process with scripts or import into spreadsheet tools. |
| **CSV** | 每层生成一个 CSV 文件，以网格格式存储瓦片引用（`tileset_id:tile_x:tile_y`），便于脚本处理或导入表格工具。 |

---

## Keyboard Shortcuts
## 键盘快捷键

| Shortcut | Action |
|----------|--------|
| B | Brush tool 画笔 |
| E | Eraser tool 橡皮擦 |
| F | Fill tool 填充 |
| G | Toggle grid 显示/隐藏网格 |
| Space + Drag | Pan canvas 平移画布 |
| Shift + Drag | Straight line constraint 直线绘制约束 |
| Right-Click | Quick erase 快速擦除 |
| Ctrl + Z | Undo 撤销 |
| Ctrl + Y | Redo 重做 |
| Ctrl + = | Zoom in 放大 |
| Ctrl + - | Zoom out 缩小 |
| Ctrl + Wheel | Zoom in/out 缩放画布 |
| Home | Center view 居中视图 |
| Ctrl + N | New project 新建项目 |
| Ctrl + O | Open project 打开项目 |
| Ctrl + S | Save project 保存项目 |

---

## Tileset Palette
## 瓦片集面板

- **Zoomable** -- Use Ctrl + Mouse Wheel over a tileset to smoothly zoom from 25% to 500%. Or use the +/- buttons for step adjustments.
  **可缩放** —— 在瓦片集上使用 Ctrl+鼠标滚轮，可在 25%~500% 之间平滑缩放；也可通过 +/- 按钮逐级调整。
- **Scrollable** -- Horizontal and vertical scrollbars appear automatically when zoomed content exceeds the panel.
  **可滚动** —— 当缩放后的内容超出面板范围时，会自动显示水平/垂直滚动条。
- **Collapsible** -- Click the arrow to collapse/expand individual tilesets to save space.
  **可折叠** —— 点击箭头可折叠/展开单个瓦片集，节省界面空间。
- **Live Preview** -- Selected tile shown in a preview panel with tileset name and coordinates.
  **实时预览** —— 选中的瓦片会在预览面板中显示，并标注瓦片集名称与坐标。

---

## Who is this for?
## 适用人群

- **Indie game developers** building 2D games who need a simple, fast level editor
  **独立游戏开发者** —— 开发2D游戏、需要简洁高效关卡编辑器
- **Level designers** prototyping tile-based layouts before importing into a game engine
  **关卡设计师** —— 导入引擎前快速制作瓦片布局原型
- **Game jam participants** who need a quick, zero-setup tool for creating maps
  **游戏创作节参与者** —— 需要零配置、快速制图工具
- **Hobbyists and students** learning about 2D game design and tile mapping
  **爱好者与学生** —— 学习2D游戏设计与瓦片地图

---

## Technical Details
## 技术信息

- **Platform:** Windows (standalone .exe, no installation required)
  **平台:** Windows（独立 .exe 文件，免安装）
- **Size:** ~17 MB
  **体积:** 约 17 MB
- **Runtime:** Self-contained (Python + Tkinter bundled via PyInstaller)
  **运行环境:** 自包含运行包（Python + Tkinter 由 PyInstaller 打包）
- **Dependencies:** None -- just download and run
  **依赖:** 无额外依赖——下载即运行
- **Tileset formats:** PNG, JPG, BMP, GIF
  **瓦片集格式:** PNG, JPG, BMP, GIF
- **Project format:** .tlemap (JSON-based, human-readable)
  **项目格式:** .tlemap（基于 JSON，可读可编辑）

---

## How to Use
## 使用方法

1. Download `TileMapEditor.exe`
   下载 `TileMapEditor.exe`
2. Double-click to run (no installation needed)
   双击运行（无需安装）
3. Click **+ Import Tileset** to load your spritesheet image
   点击 **+ 导入瓦片集** 加载精灵图集
4. Set tile dimensions (auto-detected or manual) and confirm
   设置瓦片尺寸（自动识别或手动填写）并确认
5. Select a tile from the palette, choose a tool, and start painting
   从面板中选择瓦片，选用工具，开始绘制
6. Add layers, adjust map size, toggle grid as needed
   按需添加图层、调整地图尺寸、开关网格
7. Save your project as `.tlemap` or export to JSON/CSV
   将项目保存为 `.tlemap`，或导出为 JSON/CSV 格式

---

## Screenshots
## 截图
<img width="2040" height="1366" alt="1772519842384_d" src="https://github.com/user-attachments/assets/b8f18687-9913-4138-81ec-35fa029c2886" />
<img width="2040" height="1366" alt="image" src="https://github.com/user-attachments/assets/7e1841c0-5ac8-44e0-b47c-30b8472deadf" />
<img width="2040" height="1366" alt="1772519826802_d" src="https://github.com/user-attachments/assets/e6045a7d-7cf5-4161-ab40-d11e4287f29e" />

---

**Author:** Lionel
**作者:** Lionel

Free to use. Built for the game development .
免费使用，为游戏开发打造。
