# GPT-Instruction-Finetuning
Fine-tuned GPT-2 model on a structured instruction dataset to enhance response quality.

This project provides a complete, from-scratch implementation of a GPT-2 style transformer model in PyTorch. It demonstrates the entire lifecycle of a modern LLM project:
Building the Model: All core components, including Multi-Head Attention, Feed-Forward Networks, and Layer Normalization, are implemented from scratch.
Loading Pre-trained Weights: The script loads the official 124M parameter weights from OpenAI into the custom model architecture.
Base Model Generation: It showcases the text generation capabilities of the pre-trained base model.
Instruction Finetuning: The model is then fine-tuned on an Alpaca-style instruction dataset to teach it how to follow commands.
Evaluation & Inference: Finally, it evaluates the performance of the fine-tuned model, demonstrating its improved ability to follow instructions.

Project Pipeline : The project follows these main steps -
1. Model Architecture Definition: The complete GPT-2 transformer architecture is defined from scratch using PyTorch.
2. Loading Pre-trained Weights: Official OpenAI GPT-2 124M weights are loaded into the custom architecture to create a functional base model.
3. Baseline Performance Assessment: The base model is tested on instruction prompts to establish a performance baseline before finetuning.
4. Data Acquisition and Preparation: An instruction dataset is downloaded, converted into the Alpaca prompt format, and split into training, validation, and test sets.
5. Dataset Structuring and Batching: A custom DataLoader is created to pad batches and mask the loss function, ensuring the model only trains on the response portion of the text.
6. Instruction Finetuning: The model is trained on the prepared instruction data using an AdamW optimizer while monitoring training and validation losses.
7. Evaluation and Inference: The finetuned model's performance is evaluated by generating responses for the unseen test set and comparing them to the ground-truth answers.
8. Saving the Final Model: The final weights of the instruction-tuned model are saved to a file for future inference.
