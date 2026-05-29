# ParFlow-Online-Course

本仓库用于整理 ParFlow 在线课程资料，包括课程讲义和 ParFlow 耦合陆面模式示例。

更多有关 ParFlow 教程请关注我们的公众号：**ParFlow Community**

<img src="./imgs/ParFlowCommunity.jpg" width="300">

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
