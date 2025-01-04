---
license: other
library_name: peft
tags:
- llama-factory
- lora
- generated_from_trainer
base_model: /mnt/workspace/lixiangyu/Meta-Llama-3-8B-Instruct
model-index:
- name: sft-citation
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft-citation

This model is a fine-tuned version of [/mnt/workspace/lixiangyu/Meta-Llama-3-8B-Instruct](https://huggingface.co//mnt/workspace/lixiangyu/Meta-Llama-3-8B-Instruct) on the citation_train dataset.
It achieves the following results on the evaluation set:
- Loss: 1.7767

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 1
- eval_batch_size: 1
- seed: 42
- gradient_accumulation_steps: 8
- total_train_batch_size: 8
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: cosine
- lr_scheduler_warmup_steps: 0.1
- num_epochs: 3.0
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step  | Validation Loss |
|:-------------:|:-----:|:-----:|:---------------:|
| 1.9597        | 0.05  | 500   | 1.9664          |
| 1.9169        | 0.1   | 1000  | 1.9242          |
| 1.8869        | 0.16  | 1500  | 1.9028          |
| 1.8874        | 0.21  | 2000  | 1.8911          |
| 1.8707        | 0.26  | 2500  | 1.8791          |
| 1.9158        | 0.31  | 3000  | 1.8716          |
| 1.8741        | 0.36  | 3500  | 1.8642          |
| 1.8468        | 0.42  | 4000  | 1.8575          |
| 1.8279        | 0.47  | 4500  | 1.8510          |
| 1.8166        | 0.52  | 5000  | 1.8452          |
| 1.8289        | 0.57  | 5500  | 1.8421          |
| 1.8639        | 0.62  | 6000  | 1.8374          |
| 1.8275        | 0.67  | 6500  | 1.8332          |
| 1.8866        | 0.73  | 7000  | 1.8290          |
| 1.8176        | 0.78  | 7500  | 1.8262          |
| 1.8061        | 0.83  | 8000  | 1.8218          |
| 1.8166        | 0.88  | 8500  | 1.8180          |
| 1.8146        | 0.93  | 9000  | 1.8154          |
| 1.8108        | 0.99  | 9500  | 1.8119          |
| 1.8093        | 1.04  | 10000 | 1.8106          |
| 1.7701        | 1.09  | 10500 | 1.8080          |
| 1.7164        | 1.14  | 11000 | 1.8050          |
| 1.7304        | 1.19  | 11500 | 1.8035          |
| 1.7474        | 1.25  | 12000 | 1.8031          |
| 1.7805        | 1.3   | 12500 | 1.8005          |
| 1.7144        | 1.35  | 13000 | 1.7994          |
| 1.7408        | 1.4   | 13500 | 1.7974          |
| 1.7235        | 1.45  | 14000 | 1.7950          |
| 1.7264        | 1.5   | 14500 | 1.7932          |
| 1.7325        | 1.56  | 15000 | 1.7903          |
| 1.7315        | 1.61  | 15500 | 1.7896          |
| 1.7194        | 1.66  | 16000 | 1.7899          |
| 1.7633        | 1.71  | 16500 | 1.7862          |
| 1.7488        | 1.76  | 17000 | 1.7833          |
| 1.7526        | 1.82  | 17500 | 1.7829          |
| 1.6691        | 1.87  | 18000 | 1.7820          |
| 1.7509        | 1.92  | 18500 | 1.7795          |
| 1.7142        | 1.97  | 19000 | 1.7795          |
| 1.6712        | 2.02  | 19500 | 1.7813          |
| 1.6786        | 2.08  | 20000 | 1.7807          |
| 1.6966        | 2.13  | 20500 | 1.7805          |
| 1.6424        | 2.18  | 21000 | 1.7807          |
| 1.6469        | 2.23  | 21500 | 1.7805          |
| 1.666         | 2.28  | 22000 | 1.7800          |
| 1.6542        | 2.34  | 22500 | 1.7792          |
| 1.6505        | 2.39  | 23000 | 1.7784          |
| 1.6994        | 2.44  | 23500 | 1.7780          |
| 1.7104        | 2.49  | 24000 | 1.7782          |
| 1.7291        | 2.54  | 24500 | 1.7779          |
| 1.6194        | 2.59  | 25000 | 1.7776          |
| 1.619         | 2.65  | 25500 | 1.7777          |
| 1.6469        | 2.7   | 26000 | 1.7770          |
| 1.6965        | 2.75  | 26500 | 1.7769          |
| 1.696         | 2.8   | 27000 | 1.7768          |
| 1.6625        | 2.85  | 27500 | 1.7767          |
| 1.6547        | 2.91  | 28000 | 1.7767          |
| 1.6197        | 2.96  | 28500 | 1.7767          |


### Framework versions

- PEFT 0.10.0
- Transformers 4.38.2
- Pytorch 2.1.2+cu121
- Datasets 2.16.1
- Tokenizers 0.15.1