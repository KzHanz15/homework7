# three-d · 课堂作业七（Three.js 与 A-Frame 浏览器三维开发）

姓名：彭建仁    学号：20253060001    课程：软件开发综合实践（2026 秋）

## 目录结构

| 文件/目录 | 说明 | 类型 |
|-----------|------|------|
| `showcase.html` + `showcase.js` | Three.js 旋转展示台（案例复现） | 必做·案例复现 |
| `campus.html` | A-Frame 校园角标小场景（案例复现） | 必做·案例复现 |
| `my-scene-three/` | 自主实践 · Three.js 版《星球宇宙》 | 必做·自主实践 |
| `my-scene-aframe/` | 自主实践 · A-Frame 版《星球宇宙》 | 必做·自主实践 |

## 运行方式

依赖均在线的 CDN，无需本地库文件，直接双击 HTML 用浏览器打开即可：

- Three.js 核心：`https://cdn.jsdelivr.net/npm/three@0.128.0/build/three.min.js`
- Three.js 轨道控制器：`https://cdn.jsdelivr.net/npm/three@0.128.0/examples/js/controls/OrbitControls.js`
- A-Frame：`https://aframe.io/releases/1.4.2/aframe.min.js`

> 需联网加载库。若离线环境，请将对应库文件下载为 `libs/` 本地文件并替换 `<script>` 中的 `src`。

## 自主实践说明

主题：**星球宇宙**。用纯几何体（球、环面、方盒、Points 粒子）搭建太阳系简化模型，无外部模型/贴图，版权安全。

- **Three.js 版**（`my-scene-three`）：太阳（自发光）、地球公转+自转+轴倾斜、月球绕地球、带光环行星、小行星带、星空粒子；环境光+点光源；动画循环；OrbitControls 鼠标拖拽旋转/滚轮缩放；窗口 resize 适配。
- **A-Frame 版**（`my-scene-aframe`）：深空天空+地面、太阳点光源、地球/月球/带环行星绕转动画、小行星点缀、相机初始位。

选型理由：Three.js 做精细控制（轨道、自转、粒子、精确光源），A-Frame 用标签快速搭出可走动的沉浸场景；原理相通（A-Frame 底层就是 Three.js）。