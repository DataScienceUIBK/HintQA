![Alt text](images/banner.jpeg "HintQA")

<span align="center">
    <a href="https://huggingface.co/datasets/JamshidJDMY/HintQA/tree/main"><img alt="Huggingface" src="https://img.shields.io/static/v1?label=Datasets&message=HintQA&logo=huggingface&color=20BEFF"/></a>
</span>
<a href="https://doi.org/10.18653/v1/2024.findings-emnlp.546"><img src="https://img.shields.io/static/v1?label=Paper&message=ACL Anthology&color=green&logo=arxiv"></a>
<a href="https://colab.research.google.com/github/DataScienceUIBK/HintQA/blob/main/Code/demo.ipynb"><img src="https://img.shields.io/static/v1?label=Colab&message=Demo&logo=Google%20Colab&color=f9ab00"></a>
<a href="https://opensource.org/license/mit"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=red"></a>


# HintQA: Exploring Hint Generation Approaches in Open-Domain Question Answering
*HintQA* revolutionizes the field of automatic question answering by introducing a novel context preparation method that utilizes Automatic Hint Generation. Unlike traditional QA systems that rely on either retrieval-based methods (sourcing documents from databases like Wikipedia) or generation-based approaches (using large language models to generate context), HintQA prompts large language models to produce hints that guide the answering process.

## <img src="https://github.com/DataScienceUIBK/HintQA/blob/main/images/gif-dan.gif" width="32" height="32"/> Attention<img src="https://github.com/DataScienceUIBK/HintQA/blob/main/images/gif-dan.gif" width="32" height="32"/>

As of **February 2025**, we strongly recommend using **HintEval**, the dedicated framework for **hint generation and evaluation**. HintEval now incorporates the **HintQA datasets**, including the rich datasets of TriviaQA, NQ, and WebQ. Each dataset is enhanced to provide up to 10 hints per question, facilitating an unparalleled ease in handling hints.

🔗 Explore HintEval's resources:
- 📖 **[HintEval Documentation](http://hinteval.readthedocs.io/)**
- 📦 **[HintEval PyPI Installation](https://pypi.org/project/hinteval/)**
- 💻 **[HintEval GitHub Repository](https://github.com/DataScienceUIBK/HintEval)**
- 📜 **[HintEval Paper (arXiv)](https://doi.org/10.48550/arXiv.2502.00857)**  

For a **seamless integration** of hint generation and evaluation in your projects, transitioning to **HintEval** is highly recommended!

## 🗃️Datasets
In this study, we generated up to 10 hints for each question from popular datasets: [⬇️TriviaQA](https://huggingface.co/datasets/JamshidJDMY/HintQA/tree/main/TriviaQA), [⬇️NaturalQuestions](https://huggingface.co/datasets/JamshidJDMY/HintQA/tree/main/NQ), and [⬇️WebQ](https://huggingface.co/datasets/JamshidJDMY/HintQA/tree/main/WebQ) using the [Automatic Hint Generation systems](https://github.com/DataScienceUIBK/TriviaHG). You can access and download each dataset by following the corresponding links. The statistics of the datasets are below: 
|  Dataset          |  Scenario | Num. of Questions | Num. of Hints |
| ----------------- | --------- | ----------------- | ------------- |
| TriviaQA          | Finetuned | 11,313            | 105,709       |
| TriviaQA          | Vanilla   | 11,313            | 103,018       |
| NaturalQuestions  | Finetuned | 3,610             | 33,131        |
| NaturalQuestions  | Vanilla   | 3,610             | 30,976        |
| WebQ              | Finetuned | 2,032             | 16,978        |
| WebQ              | Vanilla   | 2,032             | 15,812        |

These datasets are available as JSON files, containing both **Vanilla.json** and **Finetuned.json** versions. The Finetuned.json was generated using the LLaMA 70b model, which was fine-tuned on [💡TriviaHG](https://github.com/DataScienceUIBK/TriviaHG), while Vanilla.json was created using the base, untrained model.
```json
[
    {
        "Q_ID": "",
        "Question": "",
        "Hints": [ ],
        "ExactAnswer": "",
        "Answers": [  ],
        "MajorType": "",
        "MinorType": "",
        "Candidates_Answers": [  ],
        "Scores": [  ],
        "Convergence": [  ],
        "Familiarity": [  ],
        "Convergence_Ranked": [  ],
        "T5_Ranked": [  ],
    }
]

```

## ♻️ Reproducibility

To replicate the results of **HintQA**, you can run the **[Demo](https://colab.research.google.com/github/DataScienceUIBK/HintQA/blob/main/Code/demo.ipynb)** on Google Colab, which provides an end-to-end implementation of the **RAG Pipeline** using **HintEval** library. The demo walks you through the entire process, including:

- 🏗️ **Generating a dataset:** Create a custom dataset with questions and their corresponding answers.  
- 💡 **Generating hints:** Use a model to generate hints that will later be utilized in the RAG process.  
- 🔄 **RAG Pipeline:** Use hints in the RAG process to guide the LLM in generating more accurate answers.  
- 📊 **Displaying results:** Compare the predicted answers with the actual (ground truth) answers for evaluation.  

For a more detailed explanation, refer to the **[HintEval Documentation](https://hinteval.readthedocs.io)**. 

## ⚗️ Experiments
The paper presents extensive experiments on these datasets, employing zero-shot and few-shot strategies with varying numbers of hints and reranking methods to explore different scenarios and evaluate the performance of the HintQA approach. For more details on the experiments, baselines, and scenarios, please refer to the paper. The results of our experiments are provided in the `Experiments` directory.

## 🪪License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ✨Citation
If you find this work useful, please cite [📜our paper](https://doi.org/10.18653/v1/2024.findings-emnlp.546):
### Plain
Jamshid Mozafari, Abdelrahman Abdallah, Bhawna Piryani, and Adam Jatowt. 2024. Exploring Hint Generation Approaches for Open-Domain Question Answering. In Findings of the Association for Computational Linguistics: EMNLP 2024, pages 9327–9352, Miami, Florida, USA. Association for Computational Linguistics.
### Bibtex
```bibtex
@inproceedings{mozafari-etal-2024-exploring,
    title = "Exploring Hint Generation Approaches for Open-Domain Question Answering",
    author = "Mozafari, Jamshid  and
      Abdallah, Abdelrahman  and
      Piryani, Bhawna  and
      Jatowt, Adam",
    editor = "Al-Onaizan, Yaser  and
      Bansal, Mohit  and
      Chen, Yun-Nung",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2024",
    month = nov,
    year = "2024",
    address = "Miami, Florida, USA",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.findings-emnlp.546",
    doi = "10.18653/v1/2024.findings-emnlp.546",
    pages = "9327--9352"
}
```

## 🙏Acknowledgments
Thanks to our contributors and the University of Innsbruck for supporting this project.
