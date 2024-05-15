Attempt at reproducing results from paper [Math-Shepherd: Verify and Reinforce LLMs Step-by-step without Human Annotations](https://arxiv.org/abs/2312.08935). The evaluation scripts have been modified from [MetaMath](https://github.com/meta-math/MetaMath/tree/main) repository.

## GSM8k

To run tests on GSM8K, run the following command:
```
python eval_gsm8k.py --model peiyi9979/mistral-7b-sft --data_file data/GSM8K_test.jsonl
```

__Results__:

|| [__peiyi9979/mistral-7b-sft__](https://huggingface.co/peiyi9979/mistral-7b-sft)    | [__peiyi9979/math-shepherd-mistral-7b-rl__](https://huggingface.co/peiyi9979/math-shepherd-mistral-7b-rl) |
|--------| -------- | ------- |
|Reported| 77.9  | 84.1    |
|Reproduced| 77.9 | 83.6     |

## MATH500

Data source: https://github.com/openai/prm800k/blob/main/prm800k/math_splits/test.jsonl modified for processing.

To run tests on GSM8K, run the following command:
```
python eval_gsm8k.py --model peiyi9979/mistral-7b-sft --data_file data/GSM8K_test.jsonl
```

|| [__peiyi9979/mistral-7b-sft__](https://huggingface.co/peiyi9979/mistral-7b-sft)    | [__peiyi9979/math-shepherd-mistral-7b-rl__](https://huggingface.co/peiyi9979/math-shepherd-mistral-7b-rl) |
|--------| -------- | ------- |
|Reported| 28.6  |  33.0  |
|Reproduced| 26.6 |  29.6  |