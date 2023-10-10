<div align="center">
  <p>
    <a href="https://github.com/CVHub520/X-AnyLabeling/" target="_blank">
      <img width="100%" src="https://user-images.githubusercontent.com/72010077/273420485-bdf4a930-8eca-4544-ae4b-0e15f3ebf095.png"></a>
  </p>

[简体中文](README.zh-CN.md) | [English](README.md)

</div>

<p align="center">
    <a href="./LICENSE"><img src="https://img.shields.io/badge/License-LGPL%20v3-blue.svg"></a>
    <a href=""><img src="https://img.shields.io/github/v/release/CVHub520/X-AnyLabeling?color=ffa"></a>
    <a href=""><img src="https://img.shields.io/badge/python-3.7+-aff.svg"></a>
    <a href=""><img src="https://img.shields.io/badge/os-linux%2C%20win%2C%20mac-pink.svg"></a>
    <a href="https://github.com/CVHub520/X-AnyLabeling/stargazers"><img src="https://img.shields.io/github/stars/CVHub520/X-AnyLabeling?color=ccf"></a>
</p>

![](https://user-images.githubusercontent.com/18329471/234640541-a6a65fbc-d7a5-4ec3-9b65-55305b01a7aa.png)

<div style="text-align: center;">
  <a href="https://www.bilibili.com/video/BV1AV4y1U7h3/?spm_id_from=333.999.0.0">
    <img style="width: fit; margin-left: auto; margin-right: auto; display: block;" alt="AnyLabeling-SegmentAnything" src="https://user-images.githubusercontent.com/72010077/273759618-31a716ed-3366-4fad-b564-20d99f7ab2e4.gif"/>
  </a>
  <p style="text-align: center; margin-top: 10px;">
    <span style="background-image: linear-gradient(to right, #ff0000, #ff6600, #ffcc00, #00ccff, #6600ff);
 transparent;">X-AnyLabeling</span>: 
    <span style="color: yellow;">更好</span>, 
    <span style="color: orange;">更快</span>, 
    <span style="color: lightblue;">更强</span>
  </p>
</div>


## 📄 目录

- [🥳 新功能](#🥳-新功能-⏏️)
- [👋 简介](#👋-简介-⏏️)
- [🔥 亮点](#🔥-亮点-⏏️)
  - [🗝️关键功能](#🗝️关键功能-)
  - [⛏️模型库](#⛏️模型库-)
- [📖 教程](#📖-教程-⏏️)
  - [🔜快速开始](#🔜快速开始)
  - [👨🏼‍💻从源码构建](#👨🏼‍💻从源码构建)
  - [📦编译](#📦编译)
- [📋 用法](#📋-用法-⏏️)
  - [📌基础用法](#📌基础用法)
  - [🚀高级用法](#🚀高级用法)
  - [📜文档](#📜文档)
  - [🧷快捷键](#🧷快捷键)
- [📧 联系](#📧-联系-⏏️)
- [✅ 许可](#✅-许可-⏏️)
- [🏷️ 引用](#🏷️-引用-⏏️)

## 🥳 新功能 [⏏️](#📄-目录)

- Oct. 2023:
  - Release version [0.3.0]((https://github.com/CVHub520/X-AnyLabeling/releases/tag/v0.3.0)).
  - Release [Gold-YOLO](https://github.com/huawei-noah/Efficient-Computing/tree/master/Detection/Gold-YOLO) and [DAMO-YOLO](https://github.com/tinyvision/DAMO-YOLO) models.
  - Release MOT algorithms: [OC_Sort](https://github.com/noahcao/OC_SORT) (**CVPR'23**).
  - Add a new feature for small object detection using [SAHI](https://github.com/obss/sahi).
- Sep. 2023:
  - Release version [0.2.4](https://github.com/CVHub520/X-AnyLabeling/releases/tag/v0.2.4).
  - Release [EfficientViT-SAM](https://github.com/CVHub520/efficientvit/tree/main) (**ICCV'23**), [SAM-Med2D](https://github.com/OpenGVLab/SAM-Med2D), [MedSAM](https://arxiv.org/abs/2304.12306) and YOLOv5-SAM.
  - Support [ByteTrack](https://github.com/ifzhang/ByteTrack) (**ECCV'22**) for MOT task.
  - Support [PP-OCRv4](https://github.com/PaddlePaddle/PaddleOCR) model.
  - Add `video` annotation feature.
  - Add `yolo`/`voc`/`mot` export functionality.
  - Add the ability to process all images at once.
- Aug. 2023:
  - Release version [0.2.0]((https://github.com/CVHub520/X-AnyLabeling/releases/tag/v0.2.0)).
  - Release [LVMSAM](https://arxiv.org/abs/2306.11925) and it's variants [BUID](https://github.com/CVHub520/X-AnyLabeling/tree/main/assets/examples/buid), [ISIC](https://github.com/CVHub520/X-AnyLabeling/tree/main/assets/examples/isic), [Kvasir](https://github.com/CVHub520/X-AnyLabeling/tree/main/assets/examples/kvasir).
  - Support lane detection algorithm: [CLRNet](https://github.com/Turoad/CLRNet) (**CVPR'22**).
  - Support 2D human whole-body pose estimation: [DWPose](https://github.com/IDEA-Research/DWPose/tree/main) (**ICCV'23 Workshop**).
- Jul. 2023:
  - Add [label_converter.py](./tools/label_converter.py) script.
  - Release [RT-DETR](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/configs/rtdetr/README.md) model.
- Jun. 2023:
  - Release [YOLO-NAS](https://github.com/Deci-AI/super-gradients/tree/master) model.
  - Support instance segmentation: [YOLOv8-seg](https://github.com/ultralytics/ultralytics).
  - Add [README_zh-CN.md](README_zh-CN.md) of X-AnyLabeling.
- May. 2023:
  - Release version [0.1.0](https://github.com/CVHub520/X-AnyLabeling/releases/tag/v0.1.0).
  - Release [YOLOv6-Face](https://github.com/meituan/YOLOv6/tree/yolov6-face) for face detection and facial landmark detection.
  - Release [SAM](https://arxiv.org/abs/2304.02643) and it's faster version [MobileSAM](https://arxiv.org/abs/2306.14289).
  - Release [YOLOv5](https://github.com/ultralytics/yolov5)-v7.0, [YOLOv6](https://github.com/meituan/YOLOv6), [YOLOv7](https://github.com/WongKinYiu/yolov7), [YOLOv8](https://github.com/ultralytics/ultralytics), [YOLOX](https://github.com/Megvii-BaseDetection/YOLOX), 


## 👋 简介 [⏏️](#📄-目录)

`X-AnyLabeling` 是一款基于 [LabelImg](https://github.com/HumanSignal/labelImg)、[Labelme](https://github.com/wkentaro/labelme) 和 [Anylabeling](https://github.com/vietanhdev/anylabeling) 构建的出色的标注工具。它的独特之处在于，它不仅提供了各种领先的SOTA模型，还优先考虑了实际应用，旨在创建一个工业级、功能丰富的工具，以帮助开发人员简化标注工作流程，轻松实现各种复杂任务的自动标注和数据处理。</br>

## 🔥 亮点 [⏏️](#📄-目录)

### 🗝️关键功能

- 支持导入 `图像` 和 `视频`。
- 支持 `CPU` 和 `GPU` 推理，可按需选择。
- 兼容多种领先的深度学习算法。
- 单帧预测和一键处理所有图像。
- 导出选项，支持格式如 `COCO-JSON`、`VOC-XML`、`YOLOv5-TXT` 和 `MOT-CSV`。
- 与流行框架集成，包括 [PaddlePaddle](https://www.paddlepaddle.org.cn/)、[OpenMMLab](https://openmmlab.com/)、[timm](https://github.com/huggingface/pytorch-image-models) 等。
- 提供全面的 `帮助文档`，并提供积极的 `开发者社区支持`。
- 支持各种视觉任务，如 `目标检测`、`图像分割`、`人脸识别` 等。
- 模块化设计，赋予用户根据其具体需求自行编译系统的能力，同时支持自定义和二次开发。
- 图像标注功能，包括 `多边形`、`矩形`、`圆形`、`线条`、`点`，以及 `文本检测`、`识别` 和 `KIE` 标注。

### ⛏️模型库

<div align="center">

| **目标检测** | **小目标检测-[SAHI](https://github.com/obss/sahi)** | **人脸关键点检测** | **人体关键点检测** |
| :--------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------: |
| 
<img src='https://user-images.githubusercontent.com/72010077/273488633-fc31da5c-dfdd-434e-b5d0-874892807d95.png' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/61035602/206095892-934be83a-f869-4a31-8e52-1074184149d1.jpg' height="126px" width="180px"> |  <img src='https://user-images.githubusercontent.com/61035602/206095684-72f42233-c9c7-4bd8-9195-e34859bd08bf.jpg' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/61035602/206100220-ab01d347-9ff9-4f17-9718-290ec14d4205.gif' height="126px" width="180px"> |
|  **车道线检测** | **光学字符识别** | **多目标跟踪** | **实例分割** |
| 
<img src='https://user-images.githubusercontent.com/72010077/273764641-65f456ed-27ce-4077-8fce-b30db093b988.jpg' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/72010077/273421210-30d20e08-3b72-4f4d-8976-05b564e13d87.png' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/61035602/206111753-836e7827-968e-4c80-92ef-7a78766892fc.gif' height="126px" width="180px"  > | <img src='https://user-images.githubusercontent.com/61035602/206095831-cc439557-1a23-4a99-b6b0-b6f2e97e8c57.jpg' height="126px" width="180px"> |
|  **[分割一切](https://segment-anything.com/)** | **乳腺癌分割** | **皮肤病灶分割** | **息肉分割** |
| 
<img src='https://user-images.githubusercontent.com/72010077/273421331-2c0858b5-0b92-405b-aae6-d061bc25aa3c.png' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/72010077/273764259-718dce97-d04d-4629-b6d2-95f17670ce2a.png' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/72010077/273764288-e26767d1-3c44-45cb-a72e-124efb4e8263.png' height="126px" width="180px"> | <img src='https://user-images.githubusercontent.com/72010077/273764318-e8b6a197-e733-478e-a210-e4386bafa1e4.png' height="126px" width="180px"> |

更多详情，敬请参考[模型列表](./docs/models_list.md)。

</div>

## 📖 教程 [⏏️](#📄-目录)

### 🔜快速开始

直接从 [Release](https://github.com/CVHub520/X-AnyLabeling/releases/tag/v0.3.0) 或 [百度网盘](https://pan.baidu.com/s/1jcxQxhocLanKJFZBIIMfjA?pwd=xl7x) 下载并运行 `GUI` 版本。

注意事项：
- 对于 MacOS：
  - 安装完成后，前往 Applications 文件夹。
  - 右键单击应用程序并选择打开。
  - 从第二次开始，您可以使用 Launchpad 正常打开应用程序。

- 由于当前工具缺乏必要的硬件支持，所以仅提供 `Windows` 和 `Linux` 可执行版本。如果您需要其他操作系统的可执行程序，例如 `MacOS`，请参考以下步骤进行自行编译。

### 👨🏼‍💻从源码构建

- 安装所需的库：

```bash
pip install -r requirements.txt
```

> 如果您需要使用 GPU 推理，请安装相应的 requirements-gpu.txt 文件，并根据您本地的 CUDA 和 CuDNN 版本下载相应版本的 onnxruntime-gpu。更多详细信息，请参阅[帮助文档](./docs/Q&A.md).

- 生成资源 [可选]:

```
pyrcc5 -o anylabeling/resources/resources.py anylabeling/resources/resources.qrc
```

- 运行应用程序：

```
python anylabeling/app.py
```

### 📦编译

```bash
#Windows-CPU
bash scripts/build_executable.sh win-cpu

#Windows-GPU
bash scripts/build_executable.sh win-gpu

#Linux-CPU
bash scripts/build_executable.sh linux-cpu

#Linux-GPU
bash scripts/build_executable.sh linux-gpu
```

<details open>

<summary>注意：</summary>

1. 在编译之前，请根据适当的 GPU/CPU 版本，在 "anylabeling/app_info.py" 文件中修改 `__preferred_device__` 参数。
2. 如果您需要编译 GPU 版本，请使用 "pip install -r requirements-gpu-dev.txt" 安装相应的环境。具体来说，要编译 Windows-GPU 版本，请手动修改 "anylabeling-win-gpu.spec" 文件中的 "datas" 列表参数，以包括您本地 onnxruntime-gpu 的相关动态库 (*.dll)。另外，在下载 onnxruntime-gpu 包时，请确保与您的 CUDA 版本兼容。您可以参考官方文档以获取特定的兼容性表格。
3. 对于 macOS 版本，您可以参考 "anylabeling-win-*.spec" 脚本进行修改。

</details>

## 📋 用法 [⏏️](#📄-目录)

### 📌基础用法

1. 按照上述说明进行构建和启动。
2. 在 `菜单/文件` 中点击 `更改输出目录` 以指定输出目录；否则，它将默认保存在当前图像路径下。
3. 点击 `打开`/`打开目录`/`打开视频` 以选择特定的文件、文件夹或视频。
4. 在左侧工具栏上点击 `开始绘制 xxx` 按钮或 `自动标注` 控制以启动标注。
5. 单击并释放鼠标左键以选择要注释的矩形区域。或者，您可以按 "运行 (i)" 键进行一键处理。

> 注意：标注将保存到您指定的文件夹中，并且您可以参考下面的热键以加快您的工作流程。

### 🚀高级用法

- 选择左侧的 **AutoLalbeing 按钮** 或按下快捷键 "Ctrl + A" 以启动自动标注。
- 从下拉菜单 "Model" 中选择一个 `Segment Anything-liked Models`，其中 "Quant" 表示模型的量化程度。
- 使用 `自动分割标记工具` 标记对象。
    - +Point：添加属于对象的点。
    - -Point：删除您希望从对象中排除的点。
    - +Rect：绘制包含对象的矩形。Segment Anything 将自动分割对象。
    - 清除：清除所有自动分割标记。
    - 完成对象 (f)：完成当前标记。完成对象后，您可以输入标签名称并保存对象。

### 📜文档

- [帮助文档](./docs/Q&A.md)
- [模型库](./docs/models_list.md)
- [加载自定义模型](./docs/custom_model.md)

### 🧷快捷键

<details open>

<summary>点击展开/关闭</summary>

| 快捷键   | 功能                 |
| ---------| -------------------- |
| d        | 打开下一个文件         |
| a        | 打开上一个文件         |
| p        | 创建多边形             |
| r        | 创建矩形               |
| +        | SAM 模式下的 `+point`  |
| -        | SAM 模式下的 `-point`  |
| g        | 组合选定的形状         |
| u        | 取消组合选定的形状     |
| Ctrl + q | 退出应用程序           |
| Ctrl + i | 打开图像文件           |
| Ctrl + o | 打开视频文件           |
| Ctrl + u | 从目录加载所有图像     |
| Ctrl + e | 编辑标签             |
| Ctrl + j | 编辑多边形           |
| Ctrl + d | 复制多边形           |
| Ctrl + p | 切换保留上一模式     |
| Ctrl + y | 切换自动使用上一标签 |
| Ctrl + m | 批量处理任务         |
| Ctrl + a | 启用自动注释功能     |
| Ctrl + s | 保存当前信息         |
| Ctrl + Shift + s | 更改输出目录   |
| Ctrl + - | 缩小                   |
| Ctrl + 0 | 缩放至原始大小         |
| [Ctrl++, Ctrl+=] | 放大             |
| Ctrl + f | 适合窗口             |
| Ctrl + Shift + f | 适合宽度       |
| Ctrl + z | 撤销上一操作         |
| Delete   | 删除多边形             |
| Ctrl + Delete | 删除文件       |
| Backspace | 移除选定点           |
| ↑→↓←     | 使用键盘箭头移动选定对象 |

</details>

## 📧 联系 [⏏️](#📄-目录)

<p align="center">
🤗 亲，给个 Star 支持一下吧！ 🤗
</p>

如果您觉得这个项目有用或有趣，请考虑给它点赞以表示支持。如果您在使用这个项目时遇到任何问题或有任何疑问，请随时使用以下方式寻求帮助：


- [创建问题](https://github.com/CVHub520/X-AnyLabeling/issues)
- 邮箱: cv_hub@163.com
- 微信: `ww10874` （请在您的消息中包含`X-Anylabeing+问题的简要描述`）

## ✅ 许可 [⏏️](#📄-目录)

本项目采用 [GPL-3.0 开源许可证](./LICENSE)。

## 🏷️ 引用 [⏏️](#📄-目录)

### BibTeX

如果您在研究中使用了这个软件，请按照以下方式引用它：

```
@misc{X-AnyLabeling,
  year = {2023},
  author = {CVHub},
  publisher = {Github},
  journal = {Github repository},
  title = {Advanced Auto Labeling Solution with Added Features},
  howpublished = {\url{https://github.com/CVHub520/X-AnyLabeling}}
}
```