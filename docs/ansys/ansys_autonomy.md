# Ansys 自动驾驶技术 Ansys Autonomy

## Ansys 自动驾驶解决方案目的

为短期内上市的自动驾驶公司提供数十英里的仿真测试环境，使得其算法可以短时间内满足必要的机器测试步骤且符合安全标准。

## Ansys 自动驾驶解决方案

Aysns 自动驾驶解决方案是将高保真物理学与真实驾驶和操纵场景的闭环仿真相结合，以验证功能的安全性。

## Ansys Autonomy Safety & Cybersecurity Ansys自动驾驶安全和网络安全

* 自动驾驶安全

    * 传感器 Sensors：传感器仿真与验证

        仿真激光雷达、摄像头、雷达等各种类型的传感器，准确预测安装在车辆上的性能。

    * 软件 Software：推动自动化和控制软件开发。

        通过仿真并自动生成经过ISO 26262标准认证的代码，加快通过认证的时间（2倍），并将嵌入式软件开发成本降低50%。

    * Scenarios 场景：场景验证。 

        快速测试数百万种驾驶场景下的车辆，包括复杂的现实环境交通、行人、天气和光照条件等。

    * 系统 System：系统集成。 

        从芯片级到系统级仿真控制算法、人机交互（HMI）、车辆动力学等，确保车辆的可靠性与安全性。


* 网络安全：功能安全、SOTIF和网络安全分析。 

    在功能安全分析方面，开展危险与可操作性（HAZOP）分析、故障树分析（FTA）、故障模式与影响分析（FMEA）、故障模式、影响和诊断分析（FMEDA）；在网络安全分析方面，开展评估目标（TOE）建模、威胁评估和修复分析（TARA）以及攻击树分析。

## Ansys自动驾驶的闭环仿真

* Functional Safety & SOTIF Analysis 功能安全 & SOTIF 分析
    
    * 分析原则

        * FUSA ISO 26262
        * SOTIF Standard ISO 21448

    * Causes Analysis 原因分析

        * Limitaions & Disturbances：利用车辆行为和触发条件构建Fault Trees，用于分析造成限制和干扰的原因。
        * Triggering Conditions：仿真测试中产生的信的问题，根据SOTIF原则创建信的触发条件

* Control Software Development 控制软件发展

    分为 Autonomous Mode（develped by Embotech）和 Manual Mode

    * Geofencing Controls：Autopilot 只允许在已知的地理区域内运行，可以设置路径决策，道路条件，速度，传感器条件等
    * 控制软件通过 ANSYS SCADE 进行判别和验证
    * Code 生成通过 ASICD 评估

* Closed-Loop Simulation 闭环仿真

    仿真器由SCANER提供支持

    * 车辆动力学仿真添加到loop中
    * 基于安全功能分析的场景可以由 AI mode 产生也可在 Scenario Library 中选择
    * 场景变化量
        
        场景仿真目标：通过在真实世界模型， 仿真世界场景，传感器模型中对 perception，planning， control 算法进行测试，使其满足需求

    * 传感器仿真

        * Semantic Sensor Models 语义传感器模型：验证控制算法
        * High Fidelity Physic-based sensor Models 高保真物理传感器模型：验证感知算法在不同环境，不同条件中的表现
        * Validate the full system

* Simulating everything in unison

    * 系统，软件，动画演示，传感器都用于测试自动驾驶车辆
    * 通过获取测试驾驶员的行为和接管的情况得到反馈，车辆可以通过数字，视觉，听觉的方式对驾驶员发出警告
    * 在loop中引入人机交互，可以优化系统，使其使用更加快速，容易
    * Monitor Situationed Awareness：紧急情况管理和用户接管情况
    * Anticipate situaions：路口link之间对拓扑关系，使得自动驾驶车辆可以在loop中持续的跑