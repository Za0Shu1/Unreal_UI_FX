# Unreal_UI_FX

用于存放 Unreal Engine 的 UMG 界面特效。当前资产使用 **Unreal Engine 5.8** 制作，请使用 UE 5.8 项目导入。

## 拷贝到其他项目

1. 下载或克隆仓库。
2. 将仓库的 `Content` 目录合并到目标项目根目录，保留 `Content/Materials/UMG_FX` 层级。
3. 用 UE 5.8 打开目标项目，在内容浏览器中进入 `Content/Materials/UMG_FX`。打开 `WBP_Preview` 查看示例，或将 `WBP_RectBorderTrail` 放进自己的 UMG 界面。

资产间通过 `/Game/Materials/UMG_FX` 下的包路径互相引用，建议整目录复制。

## 矩形跑线

亮线沿矩形边框循环移动，尾部逐渐淡出。可以直接使用控件蓝图，也可以把材质实例赋给 UMG `Image` 的 `Brush → Image`。

| 资产 | 用途 |
| --- | --- |
| `M_UI_RectBorderTrail` | 矩形跑线母材质 |
| `M_UI_RectBorderTrail_Inst` | 可调整速度、拖尾、线宽、光晕和颜色的材质实例 |
| `WBP_RectBorderTrail` | 矩形跑线控件 |
| `WBP_Preview` | 预览示例 |
