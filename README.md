# STM32+K210+0.96寸OLED代码资源说明

## 项目简介

本项目展示了如何结合STM32微控制器、亚博K210人工智能芯片以及0.96英寸OLED显示屏来实现手写数字识别的功能。通过利用K210的强大AI处理能力进行手写数字的识别，然后通过串口通信技术将识别结果传递至STM32。STM32接收数据后，控制OLED显示屏显示出被识别的数字，实现了人机交互的一个有趣应用。

## 功能特点
- **手写数字识别**：K210芯片负责捕捉并分析用户在特定区域的手写数字，利用其内置的神经网络加速器高效完成识别任务。
- **STM32-K210通讯**：建立基于串口的通信机制，使得K210能实时地将识别到的数据发送给STM32。
- **OLED显示**：通过STM32控制0.96英寸OLED屏幕，展示K210识别出的数字，提供直观反馈。

## 硬件连接
- **STM32与OLED连接**：
  - B8 引脚连接 OLED 的 SCL（I2C时钟）。
    - B9 引脚连接 OLED 的 SDA（I2C数据）。

      - **STM32与K210连接**：
        - A2 引脚作为TX，连接到K210的Rx，用于STM32向K210发送指令或数据。
          - A3 引脚作为RX，连接到K210的Tx，接收K210处理后的数据。

          ## 使用说明
          1. **环境搭建**：确保开发环境中已配置好STM32和K210的相关编译工具及驱动库。
          2. **代码编译**：导入提供的源码到您的IDE中，针对目标硬件平台进行编译。
          3. **烧录程序**：分别将STM32和K210的程序烧录至对应的芯片。
          4. **连接调试**：按照上述硬件连接方式进行设备连接，通过串口助手或OLED屏直接观察识别效果。

          ## 注意事项
          - 在开始项目前，请确认你的硬件版本和固件兼容性。
          - 调试过程中，可能需要调整串口通信的波特率等参数以确保稳定通讯。
          - 由于涉及AI模型的运行，请确保K210的固件支持神经网络推理。

          此资源适合对嵌入式开发、人工智能感兴趣的工程师和爱好者实践学习，希望能激发大家的创新灵感，探索更多的智能应用场景。

          ## 下载链接
          [STM32K2100.96寸OLED代码资源说明](https://pan.quark.cn/s/3a7da5d10212) 

          (备用: [备用下载](https://pan.baidu.com/s/1pkhSWn2JaYGIzdKddIRdkw?pwd=1234))

          ## 说明

          该仓库仅用于学习交流，请勿用于商业用途。
