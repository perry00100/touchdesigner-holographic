# TouchDesigner 全息投影 / 沉浸式视觉

> 来源：微信视频「钢铁侠投影走进现实 — 华裔女孩刷新视听体验」
> 账号：科技财经派

---

## 🎯 核心工具：TouchDesigner

**官网**：https://derivative.ca/  
**类型**：可视化节点式实时编程平台（类似 UE 蓝图，无需写代码）  
**开发商**：加拿大 Derivative 公司  
**License**：非商业版免费，商业版收费

### 主要功能

| 功能 | 说明 |
|------|------|
| 实时图形渲染 | 2D/3D 图形、粒子系统、着色器编程 |
| 视频处理 | 实时合成、分析、变形、滤镜、映射 |
| 音频可视化 | 实时响应音频输入生成视觉效果 |
| 节点式编程 | 连线即可开发，无需写代码 |
| 多通道输出 | 支持多窗口/多显示器/沉浸式环绕 |
| VR 支持 | HTC Vive、Oculus，支持 75-90Hz 高帧率 |

### 支持的输入/硬件

- Kinect 1/2（体感）
- LeapMotion（手部追踪）
- Oculus / HTC Vive
- MIDI 控制器
- OSC（开放式声音控制）
- 摄像头 / 网络流 / 3D模型
- Python API 扩展

### 应用场景

- 🏛️ 建筑投影映射（楼体秀）
- 🎵 VJ 现场视觉表演
- 🎨 沉浸式艺术装置
- 🎮 交互式展览
- 🎬 音乐视频制作
- 🖥️ 数字标牌 / 信息亭
- 🚗 汽车 HUD / 全息仪表盘
- 🎮 实时游戏引擎交互

---

## 🧩 钢铁侠 HUD 效果制作路径

### 核心技术栈

```
TouchDesigner + LeapMotion + Houdini + LED矩阵/全息幕
```

### 步骤分解

1. **Houdini**：生成地形/3D 模型（如等高面切片）
2. **LeapMotion**：实时捕捉手部动作/手势
3. **TouchDesigner**：接收 LeapMotion 数据，驱动视觉渲染
4. **LED 矩阵 / 全息幕**：输出全息-like 视觉效果

### 关键代码参考

```python
# TouchDesigner 连接 LeapMotion（官方内置节点）
# 无需安装 SDK，装好后直接在 TD 内创建 leapmotion 节点即可

# LeapMotion 可读取的数据（部分）：
# - 手部位置 (x, y, z)
# - 手指关节角度
# - 手势识别（捏合、滑动等）
```

---

## 📚 学习资源

| 资源 | 链接 |
|------|------|
| 官网 | https://derivative.ca/ |
| 官方论坛 | https://forum.derivative.ca/ |
| 中文教程 | https://zhuanlan.zhihu.com/p/492789461 |
| Houdini+TD 钢铁侠效果 | https://www.cnblogs.com/simonxia/p/4298803.html |
| RunwayML + TD 机器学习 | https://blog.csdn.net/gitblog_00181/article/details/146904059 |

---

## 🔗 相关项目收藏

| 项目 | 链接 | 说明 |
|------|------|------|
| MervinPraison/PraisonAI | github.com/MervinPraison/PraisonAI | 多智能体框架 |
| thedotmack/claude-mem | github.com/thedotmack/claude-mem | Claude 记忆管理 |
| MAGI-1 | github.com/AshoraLab/MAGI-1 | 自回归视频生成 |

---

## 💡 商业应用方向

- **展厅/博物馆**：沉浸式数字展览
- **品牌活动**：投影映射 + 交互体验
- **直播/短视频**：AI 生成 + 全息视觉效果
- **智能汽车**：HUD 全息仪表盘
- **元宇宙**：VR/AR 实时内容生成

---

*最后更新：2026-06-27*
