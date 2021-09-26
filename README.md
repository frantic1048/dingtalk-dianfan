# dingtalk-dianfan

工作日每天定时发送点饭提醒。

## Fork

本项目源自 [whtsky/dingtalk-dianfan](https://github.com/whtsky/dingtalk-dianfan)，主要调整有：

- frantic1048/dingtalk-dianfan#1 将剩余点饭次数从按月调整到了按季度计算（适应政策变化）

## 快速开始

```sh
poetry install
env DINGTALK_ACCESS_TOKEN=<钉钉机器人 token> poetry run python dianfan.py
```

## 开发

### 安装依赖

先安装 [poetry](https://python-poetry.org/)，然后用 poetry 安装项目依赖：

```sh
poetry install
```

### 代码检查与测试

```sh
poetry run black .
poetry run pytest
```

## 部署

参考 [./github/workflows/cron.yaml]()