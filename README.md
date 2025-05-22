# Houdni-Digital-Assets
This is a repository for houdini nodes
---

## 🔧 HDA 工具列表

### 1. `Rozen_CellForcell_blackbox.hda`

**用途：**  
产出粒子拉丝效果

**参数说明：**

| 参数名           | 描述 |
|------------------|------|
| `CellSize`       | 最小细胞尺寸；决定了拉丝精细程度，和呈现的细胞图案或拉丝密集度 |
| `ScaleForce`     | 作用强度；决定多长时间汇聚成型 |
| `Density`        | 最大密度；能检测汇聚成团状粒子数量，决定支持的最大梯度范围 |
| `ForceFalloff`   | 距离衰减指数；距离越远，作用力越弱 |
| `MinMaxDivide`   | 最大距离/最小距离；原读作“最小细胞尺寸”，实际决定了衰减范围 |
| `dissolveSpeed`  | 加速死亡速度；粒子密度过大的地方会加速死亡 |
| `CoverageScale`  | 覆盖范围缩放；调整整体粒子分布覆盖区域 |
| `particleScale`  | 粒子半径缩放；值越大粒子越粗，但可能相互影响遮挡，影响形状识别 |
| `UseCurvature`   | 应用曲率；若开启，则使用曲率结果形成腺脉、成细胞，适合更精细的拉丝结构 |
| `switchPointVDB` | 废弃；旧方法，直接用粒子数量代替 `density` 体积计算，效率极低，但生成的结构更细 |
| `pscaleVEX`      | 半径表达式；可在此处写 VEX 表达式控制粒子半径变化，比如使用倍乘关系 |
| `forceVEX`       | 力场表达式；可在此处写 VEX 表达式控制作用力，比如乘以 `amp` 参数作为系数 |



**演示视频：**  
[📹 使用演示]([videos/CurveScatter_Demo.mp4](https://www.bilibili.com/video/BV1pa4y1K7HR/?spm_id_from=333.1391.0.0&vd_source=9edcf7b007daf6ce85a2a97aaff93230))


### 2. `energ`

**说明：**  
螺旋拉丝吸引粒子项目

---
