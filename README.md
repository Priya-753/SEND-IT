# README

#This project evaluates PEFT approaches, BitFit and Lora, used for large language models (LLMs) with an emphasis on small scale models and ultra-low resource fine-tuning.

To start, please create a HuggingFace token to access the OPT-125m model from transformers and the Sentiment140 dataset from datasets

Next, run the baseline model in the ipynb notebook "OPT125M_Baseline_PEFT.ipynb" where you will evaluate the base OPT125m model on binary sentiment (tweet) analysis as well as with the addition of two PEFT techniques (BitFit and LoRA)

Next, to produce visualizations as included in the report, run the ipynb within the visualizations folder -- as a guide a pre-printed pdf version is provided in this folder.

Next, run the distilled model in the ipynb notebooke "OPT125M_distilled.ipynb" where you will perform distillation of the OPT350m model (which takes the form of the teacher) to the student OPT125m model. Expected is that the distilled OPT125m, which has learned from a more powerful 350m model, will perform better on the binary sentiment analysis task.

For documentation, contributions and publication, see the doc folder.