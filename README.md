# ParFlow-CLM/CoLM实例

本仓库提供两个 ParFlow 耦合陆面模式的实例，分别提供 ParFlow-CLM 和 ParFlow-CoLM 的输入文件和运行脚本。

更多有关 ParFlow 教程请关注我们的公众号： **ParFlow Community**

![ParFlow Community](ParFlowCommunity.jpg)

---

## 目录结构

```
.
├── parflow-clm/          # ParFlow-CLM 实例
│   ├── model_run.py      # 模型运行脚本
│   ├── forcing/          # 气象驱动数据
│   └── inputs/           # 模型输入文件
│
└── parflow-colm/         # ParFlow-CoLM 实例
    ├── model_run.py      # 模型运行脚本
    ├── forcing/          # 气象驱动数据
    └── inputs/           # 模型输入文件
```

---


### 运行
若还未安装ParFlow，请参考[ParFlow Docker环境中文配置指南](https://github.com/ParFlowCommunity/ParFlow-Docker-CN)

在该实例目录下，启动DocKer
```bash
docker run -d --rm -v ./:/workspace -p 8888:8888 parflowcommunity/parflow-docker-cn:v1.0
```
进入Docker环境后，打开终端

```bash
python3 model_run.py
```

---
