# Integrating Negative Examples when Fine-tuning Large Language Models as Agents

## Models

Our model is Llama-2-chat. 

https://huggingface.co/meta-llama/Llama-2-7b-chat-hf

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


