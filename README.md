# test-data
openai 专用格式
* 《临高启明》中采样 30K [https://github.com/zsc/test-data/blob/main/training_data_prepared%20(1).jsonl](https://raw.githubusercontent.com/zsc/test-data/main/training_data_prepared%20(1).jsonl)
* 欧神水库论坛 中采样 20K [https://github.com/zsc/test-data/blob/main/training_data_prepared%20(2).jsonl](https://github.com/zsc/test-data/blob/main/training_data_prepared%20(2).jsonl)

# 使用 OpenAI fine-tune
```
openai tools fine_tunes.prepare_data -f training_data.jsonl
openai api fine_tunes.create -t training_data_prepared\ \(3\).jsonl -m davinci
openai wandb sync # 建好 wandb 帐号后
```
