# Qwen中医药命名实体识别

本项目基于 **Qwen2.5-7B-Instruct** 模型，使用 **QLoRA** 技术进行微调，旨在实现中医药领域的命名实体识别。

该模型能够从非结构化的医疗文本中提取结构化信息，支持以下 10 类实体：

- **诊断信息**：中医诊断、中医证候、西医诊断
- **治疗方案**：中医治则、中医治疗、西医治疗、其他治疗
- **药物/方剂**：中药、方剂
- **症状**：临床表现

## 技术栈

- **Base Model**: Qwen/Qwen2.5-7B-Instruct
- **Fine-tuning**: QLoRA (BitsAndBytes + PEFT)
- **Training**: HuggingFace Transformers
- **Monitoring**: SwanLab

## 目录结构

```text
.
├── data/                   # 存放训练和测试数据
├── output/                 # 训练输出权重
├── Qwen_NER_Finetune.ipynb # 核心代码
├── requirements.txt        # 环境依赖
└── README.md               # 项目说明
```
