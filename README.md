# OpenGL-ES-3.x
This project`s codes is recorded from the book of OpenGL ES 3.x 游戏开发.

## Projects Catalog
---

### Book A

- Sample3 初识OpenGL ES 3.x
   * Sample3.1: 初识OpenGL ES 3.0应用程序——创建一个旋转三角形
---

- Sample5 必知必会的3D开发知识——投影及各种变换
   * Sample5_1: 正交投影
   * Sample5_2: 透视投影
   * Sample5_3: 平移变换
   * Sample5_4: 旋转变换
   * Sample5_5: 缩放投影
   * Sample5_6: 各种绘制方式概览
   * Sample5_7: 三角形条带与扇面绘制方式
   * Sample5_8: 用三角形条带方式绘制非连续三角形构成的物体
   * Sample5_9: 采用索引法（glDrawElements）进行绘制
   * Sample5_10: 采用索引法（glDrawRangeElements）进行绘制
   * Sample5_11: layout 限定符的使用
   * Sample5_12: 顶点常量属性(glVertexAttribNf)，(glVertexAttribNfv) 基本知识
   * Sample5_13: 设置合理的视角
   * Sample5_14: 设置合理的透视参数
   * Sample5_15: 多边形偏移
   * Sample5_16: 卷绕和背面剪裁
---

- Sample6 光照
   * Sample6_1: 球体构建的基本原理
   * Sample6_2: 环境光
   * Sample6_3: 散射光
   * Sample6_4: 镜面光
   * Sample6_5: 三种光照通道的合成
   * Sample6_6: 定向光
   * Sample6_7: 面法向量的绘制效果
   * Sample6_8: 点法向量的绘制效果
   * Sample6_9: 每片元计算一次光照的案例
   * Sample6_10: 每顶点计算一次光照的案例
---

- Sample7 纹理映射
   * Sample7_1: 纹理映射的简单案例
   * Sample7_2: 纹理色彩通道的灵活组合
   * Sample7_3: 纹理拉伸不同拉伸方式的案例
   * Sample7_4: 不同纹理采样方式的案例
   * Sample7_5: 地月系星空场景(2D纹理映射到球面，多重纹理与过程纹理)
   * Sample7_6: 压缩纹理的使用(ETC1)
   * Sample7_7: 点精灵的简单案例
   * Sample7_8: 3D纹理的简单案例
   * Sample7_9: 2D纹理数组
   * Sample7_10: 采样器配置对象的使用
---

- Sample8 3D基本形状的构建
   * Sample8_1: 圆柱体
   * Sample8_2: 圆锥体
   * Sample8_3: 圆环体
   * Sample8_4: 螺旋管
   * Sample8_5: 几何球
   * Sample8_6: 足球碳分子模型的搭建
   * Sample8_7: 印度古典建筑场景的开发
---

- Sample9 更逼真的游戏场景——3D模型加载
   * Sample9_1: 加载obj模型文件（仅采用条纹着色策略，未加载obj中的法向量）
   * Sample9_2: 根据加载的顶点与及三角形面的数据自动计算法向量并施加光照的案例（使用的法向量为面法向量）
   * Sample9_3: 采用点平均法向量进行光照渲染的案例
   * Sample9_4: 加载纹理坐标信息的案例
   * Sample9_5: 加载带有法向量的obj文件
   * Sample9_6: 双面光照的案例
---

- Sample10 独特的场景渲染技术——混合与雾
   * Sample10_1: 简单混合效果的案例（启用混合模式） GLES30.glBlendFunc(GLES30.GL_SRC_COLOR, GLES30.GL_ONE_MINUS_SRC_COLOR);
   * Sample10_1a: 简单混合效果的案例（启用混合模式） GLES30.glBlendFunc(GLES30.GL_SRC_ALPHA, GLES30.GL_ONE_MINUS_SRC_ALPHA);
   * Sample10_1b: ETC2压缩纹理的使用
   * Sample10_2: 地月系云层效果的实现
   * Sample10_3: 雾的简单实现（采用线性雾计算模型）
   * Sample10_4: 采用非线性雾计算模型的案例
---

- Sample11 常用的3D 开发技巧——标志板、天空盒、镜像绘制等
   * Sample11_1: 标志板的案例
   * Sample11_2: 普通灰度图地形（仅山体）
   * Sample11_3: 过程纹理灰度图地形（对同一物体根据不同情况应用不同纹理着色）
   * Sample11_4: MipMap纹理设置地形
   * Sample11_4a: 在顶点着色器中采样灰度图纹理，计算顶点的海拔高度
   * Sample11_5: 将6个纹理矩形组成天空盒子
   * Sample11_6: 天空穹（采用半球面模拟天空）
   * Sample11_7: 简单镜像效果（镜像和实体的显示效果是一样的）
   * Sample11_8: 镜像效果的升级（镜像相对于实体，显示较为模糊，只需要绘制完镜像体后，采用混合模式绘制一个半透明的反射面即可）
   * Sample11_9: 动态文本输出
   * Sample11_10: 非真实感绘制
   * Sample11_11: 描边效果的实现（沿法线挤出轮廓）
   * Sample11_12: 解决Sample11_11，在两个物体重叠区域，描边没有出现的问题（这是因为描边时关闭了深度缓冲写入，后面绘制的物体将前面的描边挡住了。）
   * Sample11_13: 解决Sample11_11，描边的粗细和物体距离摄像机远近相关（在视空间中挤出）
---

- Sample12 渲染出更加酷炫的3D场景——几种剪裁与测试
   * Sample12_1: 使用裁剪测试设置裁剪窗口
   * Sample12_2: 基于Alpha测试的椭圆窗口案例
   * Sample12_3: 基于模板测试的案例（使用模板测试对案例Sample11_8的升级）
   * Sample12_4: 任意剪裁平面的案例
---

- Sample13 引人入胜的游戏特性——传感器应用开发
   * Sample13_1: 传感器应用开发——基本的开发流程（加速传感器案例）
   * Sample13_2: 磁场传感器案例
   * Sample13_3: 陀螺仪传感器案例
   * Sample13_4: 光传感器案例
   * Sample13_5: 温度传感器案例
   * Sample13_6: 接近传感器案例
   * Sample13_7: 姿势传感器案例
   * Sample13_8: 加速度传感器综合案例
   * Sample13_9: 解决传感器坐标轴问题的案例
---

- Sample14 Android NDK及iOS平台下的OpenGL ES开发
   * Sample14_1: 使用Android NDK开发简单的OpenGL ES 3.0程序——创建一个旋转三角形
   * Sample14_2: 使用Android NDK开发山地地形场景
   * Sample14_3: 基于iOS平台开发OpenGL ES 3.0程序
   * Sample14_4: 基于iOS平台的地月系场景案例
---

- Sample15 Web端3D游戏开发——WebGL3D 应用开发
   * Sample15_1: 简单渲染3D模型的WebGL案例
   * Sample15_2: 加入光照的WebGL案例
   * Sample15_3: 带有纹理贴图的WebGL案例
   * Sample15_4: WebGL版的地月系案例
---

- Sample16 休闲类游戏——3D可爱抓娃娃
   * CatcherFun: 3D可爱抓娃娃（Android应用案例）
---

- Sample17 基于WebGL的3D楼盘展示系统
   * 基于WebGL的3D楼盘展示
---
