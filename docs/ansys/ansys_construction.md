# Ansys 自动驾驶仿真平台

Ansys自动驾驶仿真解决方案可以提供自定义道路环境、自定义交通场景、构建车辆动力学模型、基于物理真实的三维场景建模、基于物理真实的多传感器模型融合和系统级仿真、基于物理的智能头灯照明仿真系统等一系列功能

## 自定义道路环境

* 具备直道、弯道、曲线等设计能力，支持道路宽度、长度、半径、方向、车道数量、车道方向、车道限速、车道类型等的编辑。
* 支持高架等不同高度道路以及不同坡度倾角、道路交叉口、匝道、并道等的定义
* 还支持车道线的自定义化建模，包括单线、双线、实线、虚线、车道线纹理、颜色等一系列车道线类型
* 具有环境模型库，如树木、建筑物、交通标识、路灯、电线杆、绿化带、动物，施工路段障碍物和设施、交通行人等对象模型
* 除自定义场景外，支持导入OpenStreetMap等3D高精地图，自动生成与地图匹配的道路模型。

## 自定义交通场景

* 提供基于语义的道路交通流设计，包括车道行驶规则、车辆及行人行为、交通指示牌行为，以及某一时刻各交通对象交通行为的数据输出。
* 自定义交通对象行为，如车辆驾驶行为、突然变道、突然加速、行人乱闯红灯和人行道等一系列场景的仿真，
* 支持设定软件内部车辆和行人之间可自定义交互与否，即可仿真自动避让行人和忽视行人发生碰撞等行为

## 构建车辆动力学模型

* Ansys 仿真平台提供了基于总成特性的车辆动力学模型，并提供了以下性能参数的配置：
        
    * 底盘参数，如长宽高、轴间距、重量等；
    * 性能参数，如最大时速、引擎转速等；
    * 转向参数
    * 轮毂参数

* 此外仿真平台还提供了各类特性参数的预定义实验数据，方便用户对所定义车辆的特性进行快速的测试验证。相关的实验数据有：
        
    * 加速特性实验数据
    * 刹车特性实验数据
    * 转弯特性实验数据
    * 方向盘特性实验数据
    * 侧风实验数据
    * 障碍物和转弯实验数据
    
* Ansys 仿真平台车辆动力学模型的导入和集成，如CarSim车辆动力学模型，以及用户自研的车辆动力学模型。

## 基于物理真实的三维场景建模

Ansys提供基于物理真实的三维场景建模和ray-tracing的图形算法。Ansys需设定相关环境光源参数以及场景中道路，建筑，车身等物体材料表面光学属性使得仿真场景的构建与物理真实达到一个高匹配度。环境光源参数设置如下：

* 环境光源

    * 天空的照度值
    * 基于经纬度的太阳光的照度和位置定义
    * 环境场景中各种点光源以及面光源的定义（光谱+IES+XMP）
    * 车辆照明系统的光源定义（光谱+IES+XMP）；
    
* 材料表面光学属性
        
    结合Ansys提供等材料库，通过Ansys开发的一套OMS材料物理光学属性BRDF测量仪硬件设备，对用户所需仿真的场景材料库进行探测，并将探测所得材料表面光学属性BSDF函数附在前述场景建模的所属材质表面，从而在ray-tracing的图形算法下仿真得到一整套完整的考虑环境光以及物体表面光学属性的物理真实的三维场景建模。

## 基于物理真实的多传感器模型融合和系统级仿真

* 基于物理的摄像头系统级仿真

    通过定义摄像头的如下物理参数得到RAW图像用以对摄像头供应商进行验证或者硬件在环系统的仿真验证。摄像头系统级仿真参数模型参照EMVA1288标准建模，主要包含：

    * 镜头模型

        * 镜头材料
        * 焦距
        * 孔径光阑
        * 镜片透过率函数
        * 畸变

    * 成像仪模型
        
        * 分辨率
        * 尺寸
        * 曝光时间
        * 噪声系数
        * 量子效率
        * 增益等

    * 处理器模型
    * 摄像头位置
    * 风挡参数
        * 入射角
        * 折射率
        * 厚度
        * 透过率函数

* 基于物理的激光雷达系统级仿真

    激光雷达的系统级仿真通过准确定义的激光雷达参数，通过发射和接收生成的点云图对用户构建的场景和交通流进行感知探测并验证相关感知算法。支持多种激光雷达模式（扫描式，旋转式）。激光雷达的建模参数包括：
    
    * 扫描式
        * 最大和小探测距离；
        * 横向视场角；
        * 纵向视场角；
        * 分辨率等；

    * 旋转式
        * 最大和最小探测距离；
        * 旋转速率；
        * 最大线数等；

* 基于物理的毫米波雷达系统级仿真

    毫米波雷达的系统级别仿真通过ROM降阶技术，以HFSS软件为模拟工具，可以通过内嵌接口工具与ANSYS自动驾驶仿真平台结合实现毫米波雷达与摄像头和激光雷达的同步实时仿真，得到雷达回波的成像结果并进行分析。

## 基于物理的智能头灯照明仿真系统

* ANSYS自动驾驶仿真平台Headlamp模块通过ANSYS特有的物理级仿真引擎，为客户提供真实的车辆头灯路面光型分布测试和动态驾驶与智能头灯仿真测试。
* 为了保证接近真实的物理仿真光型，Headlamp模块同样对光源进行仿真模拟，包括车灯光源，自然光光源，路灯光源等。
* 支持静态，动态光源分布验证

## 参考资料

* [Ansys 仿真平台代理商](https://b2b.baidu.com/land?id=5d461b79514d295016a3af1c110522e310)
* [Ansys仿真技术为自动驾驶汽车保驾护航](https://www.sohu.com/a/428156729_251620)