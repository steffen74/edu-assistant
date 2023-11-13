# Educational Helpfulness Assistant

## Repository Link

[https://github.com/steffen74/edu-assistant]

## Description

The Zephyr-7B-α model (Hugging Face, 2023) is fine-tuned via training data generated according to the Constitutional AI approach. Hereby, the model is requested to critique its generated answers and generate improved answers. The new data is then used for further fine-tuning. A set of 1000 questions on physics and history with difficulty levels ranging from Kindergarten to 12th grade is generated using GPT-4 (OpenAI, 2023b). On each of these, fifteen different critique and revision prompt pairs like the following are applied:

#### Critique

> Point out instances where the assistant's last response directly provided the answer or did not guide the student through a learning process in a Socratic manner.

#### Revision

> Please rewrite the assistant's response to follow a Socratic style of questioning, aimed at guiding the student to think for themselves.

For a baseline comparison answers of OpenAI’s GPT-3.5 and GPT-4 default models are used with custom prompts soliciting an educational helpful, Socratic style answer as proposed by OpenAI (OpenAI, 2023a, 2023b).
To evaluate the answer quality, GPT-4 is prompted to rank the answers of the different models for a given question according to the rules defined by the prompt to generate the training data. Additionally, a qualitative review is conducted by educational experts to provide further insights.

### Task Type

Fine-Tuning a Chatbot

### Results Summary

- **Best Model:** [Name of the best-performing model]
- **Evaluation Metric:** [e.g., Accuracy, F1-Score, MSE]
- **Result:** [e.g., 95% accuracy, F1-score of 0.8]

## Documentation

1. **[Literature Review](0_LiteratureReview/README.md)**
2. **[Dataset Characteristics](1_DatasetCharacteristics/exploratory_data_analysis.ipynb)**
3. **[Baseline Model](2_BaselineModel/baseline_model.ipynb)**
4. **[Model Definition and Evaluation](3_Model/model_definition_evaluation)**
5. **[Presentation](4_Presentation/README.md)**

## Cover Image

![Project Cover Image](CoverImage/cover_image.png)
