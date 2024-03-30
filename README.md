# llama-7b-ft
Llama 2 (7B) finetuned on 50k instruction-tuning data produced with GPT4. The data is from [here](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM). llama-finetune.ipynb has code finetuning 8/32 layers of Llama 2 7B, the rest are frozen. The model stats were logged with Weights and Biases, and a report for the same can be found [here](https://wandb.ai/kevinv3796/alpaca-ft/reports/Finetuning-Llama2-7B-on-Alpaca-GPT4--Vmlldzo3MzQ4MTMw) This took ~1hr on an A100 on runpod with 80GB VRAM.

The model can be found on [Huggingface](https://huggingface.co/MadMarx37/llama2-alpaca-gpt4).

The GPT4-based eval can be seen [here](https://wandb.ai/kevinv3796/alpaca-ft/reports/GPT4-eval-of-fine-tuned-Llama2--Vmlldzo3MzUwMjY0)

### WIP
- [x] GPT4-based eval
- [ ] Documentation
- [ ] Parameter-efficient finetuning using QLoRA

### References
I followed more than a few tutorials and references for this, starting from Maxime Labonne's [LLM Course](https://github.com/mlabonne/llm-course)
Most of the code here can be found in different repos - some of it on this Weights and Biases [tutorial](https://wandb.ai/capecape/alpaca_ft/reports/How-to-Fine-Tune-an-LLM-Part-1-Preparing-a-Dataset-for-Instruction-Tuning--Vmlldzo1NTcxNzE2), some on Maxime Labonne's [blog](https://mlabonne.github.io/blog/posts/Fine_Tune_Your_Own_Llama_2_Model_in_a_Colab_Notebook.html), some of it [here](https://github.com/tcapelle/llm_recipes/tree/main)
