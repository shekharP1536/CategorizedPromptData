# Dataset Name: **Categorized Prompt Data**

## Overview
This dataset is designed to classify and categorize various types of prompts. It contains prompts that can be divided into categories such as **Generation**, **Task**, **Information**, etc. The prompts within each category are further classified by type, such as **Text**, **Image**, and **Code**. The dataset is ideal for training models that can identify the category and type of a given prompt and is useful for prompt-based classification tasks.

## Dataset Structure
The dataset is structured as a list of JSON objects, where each object represents a single entry. Each entry contains the following fields:
- **Category**: The primary category of the prompt (e.g., **Generation**, **Task**, **Information**).
- **Type**: The type of the prompt (e.g., **Text**, **Image**, **Code**).
- **Prompt**: The actual text of the prompt.

### Example Entry:
```json
{
  "Category": "Generation",
  "Type": "Text",
  "Prompt": "Write a short story about a character who discovers a hidden world within their reflection."
}


### Full Example Dataset:
```json
[
  {
    "Category": "Generation",
    "Type": "Text",
    "Prompt": "Write a short story about a character who discovers a hidden world within their reflection."
  },
  {
    "Category": "Task",
    "Type": "Question",
    "Prompt": "What is the capital of France?"
  },
  {
    "Category": "Information",
    "Type": "Code",
    "Prompt": "Write a Python function to reverse a string."
  },
  ...
]
```

## Categories & Types
The dataset is organized into the following **categories** and **types**:
1. **Generation**: Prompts that require content generation (e.g., stories, poems, etc.).
    - Type: Text, Image, Code
2. **Task**: Prompts that represent a task or question.
    - Type: Question, Instruction, Request
3. **Information**: Prompts that provide or request information.
    - Type: Text, Code
4. **Miscellaneous**: Miscellaneous prompts that do not fit into the above categories.
    - Type: Various (depending on the nature of the prompt)

## Usage
This dataset can be used for training or fine-tuning models to classify and categorize different types of prompts. You can use this dataset to:
- Train a model to classify prompts based on their **Category** and **Type**.
- Perform prompt-based categorization tasks such as sorting, filtering, or organizing prompts.

### Example Python Code to Load the Dataset:
You can load this dataset in Python as follows:
```python
import json

# Load the dataset
with open('dataset.json', 'r') as f:
    dataset = json.load(f)

# Print the first entry
print(dataset[0])
```

## Dataset Splits
Currently, this dataset is available as a single unified JSON file containing all entries. You may choose to split it into training, validation, and test sets according to your requirements.

## Licensing
This dataset is shared under a custom license. Please refer to the LICENSE file for more details. Non-commercial use only. If you wish to use this dataset for commercial purposes, you must obtain permission and agree to the terms outlined in the LICENSE file. Redistribution or modification of the dataset is not allowed for commercial training purposes.

## Citation
If you use this dataset in your personal work, please cite it as follows:
```
@misc{prompt_classification,
  author = {shekharP1536},
  title = {Prompt Classification Dataset},
  year = {2024},
  url = {https://github.com/shekharP1536/CategorizedPromptData}
}

```
## Contact
For any questions or issues related to the dataset, feel free to reach out via the GitHub issues page or by emailing [mailto:mywork1536@gmail.com].


### Key Sections:
- **Overview**: Describes the dataset and its purpose.
- **Dataset Structure**: Explains how the data is structured (categories, types, and prompts).
- **Categories & Types**: Lists the categories and types of prompts in the dataset.
- **Usage**: Provides an example of how to use the dataset in code.
- **Licensing**: Please read the LICENSE file for more information on usage and restrictions.
- **Citation**: Information on how to cite your dataset.