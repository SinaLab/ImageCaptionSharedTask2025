# 🖼️ [Arabic Image Captioning Shared Task 2025](https://sina.birzeit.edu/image_eval2025/index.html)

This repository contains official baselines for the **Arabic Image Captioning Shared Task 2025**, which aims to advance the development of culturally aware Arabic image captioning models. The task provides an Arabic-language dataset and invites participants to generate natural captions for images using zero-shot or fine-tuned approaches. This repository includes two baseline systems using Qwen2.5-VL 7B, along with an evaluation script.

** Fine-tuned Model**: [Sinalab/Qwen2.5-VL-7B-Instruct-Image-Captioning](https://huggingface.co/SinaLab/Qwen-2.5-VL-7B-Instruct-Image-Captioning)

## 📂 Contents

- A zero-shot baseline for generating captions using Qwen2.5-VL 7B without fine-tuning.
- A fine-tuned baseline using Qwen2.5-VL 7B trained on the provided Arabic-captioned training set.
- An evaluation script to compare predictions with ground truth using the official metrics (BLEU, ROUGE, Cosine Similarity, and LLM as a Judge).

## 📊 Dataset

The dataset comprises images with Arabic captions. It is divided into:

- **Training Set**
- **Development Set**
- **Test Set**

To participate in the shared task, please register in ([the official registration form](https://forms.gle/qn4NDr6PYW49bLns7)).

The training and development datasets are available in the [SinaLab/ImageEval2025Task2TrainDataset](https://huggingface.co/datasets/SinaLab/ImageEval2025Task2TrainDataset) dataset.

 The test dataset will be shared only during the test phase in the shared task ([see the deadlines](https://sina.birzeit.edu/image_eval2025/index.html))
 
 *Note: The dataset can be accessed on request.*


## 🗂️ Project Structure

This repository is organized into three main components:

### [`ImageValZeroShot/`](./ImageValZeroShot/)
Contains the zero-shot baseline implementation for generating Arabic captions without any fine-tuning. See the [Zero-Shot README](./ImageValZeroShot/README.md) for detailed setup and usage instructions.

### [`ImageValFinetune/`](./ImageValFinetune/)  
Contains the fine-tuning pipeline for training Qwen2.5-VL on Arabic image captions using LoRA. See the [Fine-tuning README](./ImageValFinetune/README.md) for comprehensive training and evaluation guidance.

### [`Evaluation/`](./Evaluation/)
Contains the evaluation framework for measuring caption quality using multiple metrics including BLEU, ROUGE, Cosine Similarity, and LLM-based evaluation. See the [Evaluation README](./Evaluation/README.md) for metric details and usage.


## 🚀 Quick Start

1. **Choose your approach**: 
   - For zero-shot inference: Navigate to [`ImageValZeroShot/`](./ImageValZeroShot/)
   - For fine-tuning: Navigate to [`ImageValFinetune/`](./ImageValFinetune/)

2. **Follow the respective README**: Each directory contains detailed instructions for setup, dependencies, and execution.

3. **Evaluate results**: Use the evaluation framework in [`Evaluation/`](./Evaluation/) to measure your model's performance.

## 📬 Contact

For any questions or support:

- Email: abashiti@birzeit.edu, aaljabari@birzeit.edu, hhamoud@dohainstitute.edu.qa

---

*This repository provides the foundational tools and baselines for participating in the Arabic Image Captioning Shared Task 2025. Each component is designed to be modular and extensible for research and development purposes.*

## 📖 Citation

If you use this repository in your research, please cite:

```bibtex
@inproceedings{bashiti2025imageeval,
  title     = {{ImageEval 2025: The First Arabic Image Captioning Shared Task}},
  author    = {Bashiti, Ahlam and Aljabari, Alaa and Hamoud, Hadi and Biswas, Md. Rafiul and Shalash, Bilal and Jarrar, Mustafa and Zaraket, Fadi and Mikros, George and Asgari, Ehsaneddin and Zaghouani, Wajdi},
  booktitle = {Proceedings of the Third Arabic Natural Language Processing Conference (ArabicNLP 2025)},
  year      = {2025},
  location  = {Suzhou, China},
  note      = {Co-located with EMNLP 2025, November 5--9}
}

