# Integrating Negative Examples when Fine-tuning Large Language Models as Agents

## Models

Our models are trained with negative-aware training method based on Llama-2-chat. Each model is trained with both positive and negative samples. All model links can be found in **Table 1**.


**Table 1**: Models and datasets.

## Interactive

You can try our model using the interactive script:

```bash
python -m utils.interactive \
  --model_name_or_path  \
  --task math
```


## Evaluation

Run the following command or `scripts/evaluate.sh` to evaluate a model.

```bash
python -m data.generate --model llama-2-7b --template zero-shot-target-aware --temperature 0.2 --task_name gsm8k --task_split test
```


