# Fine-Tune LLAVA Repository

This repository demonstrates the process of fine-tuning LLAVA for various tasks, including data parsing and extracting JSON information from images. 

---

## Repository Structure

### Notebooks
- **`data_exploration/`**  
  Contains notebooks for exploring the [Cord-V2](https://huggingface.co/datasets/naver-clova-ix/cord-v2) and [DocVQA](https://huggingface.co/datasets/nielsr/docvqa_1200_examples) datasets.

- **`fine-tuning/`**  
  Includes:
  - A notebook for fine-tuning LLAVA 1.6 7B
  - A notebook for testing the fine-tuned model

- **`test_model/`**  
  Contains multiple notebooks for testing:
  - LLAVA 1.5 7B and 13B
  - LLAVA 1.6 7B, 13B, and 34B

### Source Code
- **`src/`**  
  Contains a Streamlit app to showcase the performance of the fine-tuned model. 

  To run the dashboard:
  1. In Terminal 1:
     ```bash
     python src/serve_model.py
     ```
  2. In Terminal 2:
     ```bash
     streamlit run src/app.py
     ```
  Open the dashboard at [http://localhost:8501/](http://localhost:8501/) and upload sample images from the `data` folder to view the results. You can find 20 sample images in the `data` folder.

---

## Installation

1. Install dependencies from `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

2. Install additional requirements:
   ```bash
   pip install git+https://github.com/huggingface/transformers.git
   ```
---

