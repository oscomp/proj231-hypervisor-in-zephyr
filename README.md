# proj-hypervisor-in-zephyr
## 题目
基于Zephyr RTOS开发Hypervisor启动Linux内核和Zephyr内核。

## 项目描述：
ZVM（Zephyr-based Virtual Machine）是基于Zephyr RTOS开发的轻量级虚拟机管理器，其面向嵌入式和实时系统环境，提供基础的虚拟化能力。ZVM的目标是支持多种硬件架构，满足混合关键性系统的隔离需求，并兼顾实时性和高性能。

本项目旨在围绕ZVM进行功能增强和特性扩展，吸引同学们学习操作系统、虚拟化相关知识，并通过实际动手开发，提升系统软件开发能力。本次挑战赛设置四个方向，每个方向作为独立子赛题，参赛队伍可选择其一或多个方向进行研究。

## 参考资料：
##### (1) ZVM项目Gitee地址：https://gitee.com/openeuler/zvm
##### (2) 云计算内存管理技术: Survey of memory management techniques for hpc and cloud computing
##### (3) 实时操作系统内存管理算法: An analysis and review on memory management algorithms for real time operating system
##### (4) 实时多核 VCPU 调度框架: Maracas: A real-time multicore vcpu scheduling framework
##### (5) ACRN hypervisor(x86): https://github.com/projectacrn/acrn-hypervisor
##### (6) bao-hypervisor(RISC-V,Armv8-R): https://github.com/bao-project/bao-hypervisor

## 所属赛道
2025全国大学生操作系统比赛的“OS功能挑战”赛道

## 题目要求
本题目设置四个方向，每个方向作为独立子赛题，参赛队伍可选择其一或多个方向进行研究。

### 子赛题1：支持ARMv8 Cortex-R系列
目前ZVM主要面向Cortex-A系列设计，而Cortex-R系列作为高实时需求场合（如汽车电子、工业控制等）的重要处理器架构，其虚拟化支持对ZVM未来的应用场景具有重要意义。选手需：
- 分析Cortex-R系列虚拟化特性与差异；
- 能在QEMU或硬件上运行一个Zephyr或Linux Guest；

### 子赛题2：ZVM内存管理优化
当前ZVM的内存管理机制较为基础，内存动态管理能力较为基础。选手需：
- 优化ZVM的动态内存管理机制；
- 优化ZVM的内存分配与回收算法，提高内存利用率与实时响应需求；

### 子赛题3：ZVM vCPU调度优化
现有ZVM的vCPU调度策略较为简单，未充分考虑实时性与优先级。选手需：
- 分析ZVM当前vCPU调度逻辑，设计并实现更优的vCPU调度算法；
- 支持虚拟机的实时优先级调度，探索Host OS与Guest OS调度协同机制；

### 子赛题4：跨架构支持扩展
ZVM当前主要支持ARM架构，选手可选择一种新架构（x86或RISC-V）支持核心功能：
- 分析目标架构的虚拟化特性；
- 适配ZVM核心框架至目标架构；

## 项目导师
谢国琪 xgqman@hnu.edu.cn

## 难度
中等 ~ 高 等

## 特征：
1. 使用C/C++语言开发；
2. 支持QEMU模拟器运行或实机运行；

## 预期目标
#### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标
### 子赛题1预期目标：
- 在QEMU或开发板上成功运行支持Cortex-R的ZVM；
- 能在QEMU或硬件上运行Zephyr或Linux虚拟机

### 子赛题2预期目标：
- 实现ZVM动态内存分配与释放；
- 测试冬天内存分配下的内存利用率；

### 子赛题3预期目标：
- 实现ZVM中至少一种vCPU调度实时调度算法；
- 测试调度性能与实时性指标；

### 子赛题4预期目标：
- 完成至少一种新架构（x86或RISC-V）的ZVM移植；
- 能在QEMU或硬件上运行Zephyr或Linux虚拟机


