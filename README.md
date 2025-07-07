# GPT-Instruction-Finetuning
Fine-tuned GPT-2 model on a structured instruction dataset to enhance response quality.

This project provides a complete, from-scratch implementation of a GPT-2 style transformer model in PyTorch. It demonstrates the entire lifecycle of a modern LLM project:
Building the Model: All core components, including Multi-Head Attention, Feed-Forward Networks, and Layer Normalization, are implemented from scratch.
Loading Pre-trained Weights: The script loads the official 124M parameter weights from OpenAI into the custom model architecture.
Base Model Generation: It showcases the text generation capabilities of the pre-trained base model.
Instruction Finetuning: The model is then fine-tuned on an Alpaca-style instruction dataset to teach it how to follow commands.
Evaluation & Inference: Finally, it evaluates the performance of the fine-tuned model, demonstrating its improved ability to follow instructions.
