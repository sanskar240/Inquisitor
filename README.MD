# Inquisitor: A Prompt Generation Model

**Inquisitor** is an innovative prompt generation model designed to produce meaningful prompts from any given corpus of text. By leveraging an LSTM-based architecture, Inquisitor aims to facilitate deeper understanding and engagement with content by generating relevant prompts that encourage critical thinking and exploration.

## Vision

Inquisitor envisions a future where learning and comprehension are enhanced through the use of intelligently generated prompts. By transforming static text into dynamic interactions, this model seeks to:
- Foster inquiry-based learning by encouraging users to ask questions.
- Aid educators in creating engaging materials that stimulate curiosity.
- Enhance automated tutoring systems that adapt to users’ comprehension levels.

## Applications

Inquisitor can be applied in various domains, including but not limited to:
- **Education**: Generate questions for quizzes and study materials, promoting active learning.
- **Content Creation**: Assist writers and bloggers in developing prompts for articles, discussions, or brainstorming sessions.
- **Tutoring Systems**: Provide personalized prompts in adaptive learning environments to facilitate deeper understanding of subjects.
- **Research**: Aid researchers in exploring new angles by generating prompts based on existing literature.

## Model Architecture

Inquisitor is built using a custom LSTM (Long Short-Term Memory) architecture, designed to capture the sequential dependencies in text. Key components of the architecture include:

1. **Embedding Layer**: Converts input tokens into dense vector representations, allowing the model to learn semantic meanings.
2. **LSTM Layer**: Processes the embedded sequences and captures temporal dependencies, enabling the model to understand context and generate coherent prompts.
3. **Fully Connected Layer**: Maps the LSTM output to the vocabulary size, allowing the model to predict the next token in a prompt based on the context.

The architecture's ability to learn from sequential data makes it suitable for generating prompts that maintain contextual relevance.

### Training Process

Inquisitor was trained on the SQuAD dataset, where it learned to generate prompts based on context-question pairs. The training involved:
- **Epochs**: 5
- **Batch Size**: 16
- **Learning Rate**: 0.001
- **Loss Function**: Cross-Entropy Loss with padding tokens ignored.

## Current Issues

While Inquisitor shows promise, there are several challenges that need to be addressed to improve its performance:

- **Overfitting**: The model may generate repetitive or nonsensical prompts, as observed in some cases where the output consists of repeated tokens (e.g., "the the the..."). This suggests that the model is not effectively generalizing from the training data.
- **Context Understanding**: The model may struggle with complex contexts or nuanced text, leading to irrelevant or vague prompts.
- **Prompt Diversity**: The generated prompts may lack variety, often producing similar outputs for different inputs, limiting its usefulness in diverse applications.

### Future Directions
To enhance Inquisitor's capabilities, future work will focus on:
- Implementing attention mechanisms to improve context handling and focus on relevant parts of the input text.
- Experimenting with larger and more diverse training datasets to broaden the model's understanding.
- Fine-tuning hyperparameters and model architecture for better performance and prompt quality.

## Installation

To install Inquisitor, clone this repository and install the required dependencies.

```bash
git clone https://github.com/sanskar240/Inquisitor.git
cd Inquisitor
pip install -r requirements.txt
