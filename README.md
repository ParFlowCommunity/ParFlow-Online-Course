# ParFlow-Online-Course

本仓库用于整理 ParFlow 在线课程资料，包括课程讲义和 ParFlow 耦合陆面模式示例。

更多有关 ParFlow 教程请关注我们的公众号：**ParFlow Community**

<img src="./imgs/ParFlowCommunity.jpg" width="200">

---  

## 课程讲义/lectures
本目录用于存放 ParFlow 在线课程讲义。 我们会根据学员们的反馈不定期更新讲义。 
### 第1讲 Docker环境下运行ParFlow-CLM/CoLM示例  
主讲人：唐泽宇 中山大学大气科学学院 
### 第2讲 基于Python的pftools的主要功能函数  
主讲人：杨晨 中山大学大气科学学院  
### 第5讲 地下含水介质的配置  
主讲人：杨晨 中山大学大气科学学院  
### 第6讲 ParFlow中solid file的构建方法  
主讲人：杨晨 中山大学大气科学学院  
### 第7讲 基础数据缺乏地区的地形处理与评估    
主讲人：杨晨、徐文杰 中山大学大气科学学院  
### 第8讲 ParFlow水均衡计算    
主讲人：杨晨、唐泽宇 中山大学大气科学学院  
### 第12讲 谈一谈ParFlow建模中的spin-up    
主讲人：杨晨 中山大学大气科学学院  
### 第13讲 ParFlow主要数值方法    
主讲人：杨晨 中山大学大气科学学院  
### 第14讲 ParFlow中陆面模式的使用及原理简介    
主讲人：杨晨 中山大学大气科学学院  

---  

## 目录结构

```text
.
├── examples/
│   ├── parflow-clm/          # ParFlow-CLM 示例
│   │   ├── model_run.py      # 模型运行脚本
│   │   ├── forcing/          # 气象驱动数据
│   │   └── inputs/           # 模型输入文件
│   └── parflow-colm/         # ParFlow-CoLM 示例
│       ├── model_run.py      # 模型运行脚本
│       ├── forcing/          # 气象驱动数据
│       └── inputs/           # 模型输入文件
└── lectures/                 # 课程讲义
```

---

## 示例运行

若还未安装 ParFlow，请参考 [ParFlow Docker 环境中文配置指南](https://github.com/ParFlowCommunity/ParFlow-Docker-CN)。

启动 Docker：

```bash
docker run -d --rm -v ./:/workspace -p 8888:8888 parflowcommunity/parflow-docker-cn:v1.0
```

进入 Docker 环境后，打开终端并进入对应示例目录：

```bash
cd examples/parflow-clm
python3 model_run.py
```
