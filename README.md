# Efficient Large Language Model training with LoRA and Hugging Face

This hands-on labs modifies the Hugging Face [PEFT](https://github.com/huggingface/peft) fine-tuning and model deployment example on Amazon SageMaker. For training and debugging purposes, start with `1_train-debug.ipynb`.

### Issues
When in LoRA+Int8 training mode, multi-gpu training (Data Parallel) does not work when training with the HF `Trainer` class.
- https://github.com/artidoro/qlora/issues/137

## References
- https://github.com/huggingface/notebooks/tree/main/sagemaker/24_train_bloom_peft_lora
