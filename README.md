![Alt text](images/banner.jpeg "HintQA")

<span align="center">
    <a href="https://huggingface.co/datasets/JamshidJDMY/HintQA/tree/main"><img alt="Huggingface" src="https://img.shields.io/static/v1?label=Datasets&message=HintQA&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAIGNIUk0AAHomAACAhAAA+gAAAIDoAAB1MAAA6mAAADqYAAAXcJy6UTwAAAIoUExURQAAAP/////57v/67xUVFf/clv+KAP/uzf/sxv8AAP9TAP/ltP///v/ouP/////////////////////////////8+v/pvP/biP/Vbf/Vbv/cif/qv//9+//////////03v/Yev/Zfv/14//25v/Uav/Vbv/46//////dkf/gmP/////04P/25//pvP/sxf/////lr//ouP/qwP/tyf/msv/ntf/+/P/36f/LUf/36P/w0v/w0//w0//w0//78//gm//QZv/RZv/gm//78v/////14v/nt//gnP/hn//w0f/////w0f/hn//gnP/nt//14v/////////////////LLv/MGv/PGf/LL//LG//THP/THv/SHv/UHv/LGv/LH/7SHuK8JOzDIuW+I+jAI//LHv/PTP/NF/PBG3BkOpyGMvrOH4R0NoV0NvzJGv/MF//QT//MLv/LGPu/FNayJu7FIdq2Jf7DFP/JF//ML//LJurCIsCiKujCIubAI7+hK/DHIf/LJ//HK//NGf/SHeS9IlxSP25QQmtOQmVZPu3DIf/RHf/HLP++Kf/AD/++EP3EFNCfLNhpQthrQdinKv/FFP/AEP+/K/++Dv/BEv+/Ef/CE//MIf/NIP/MGf++D//KTP/FOP/DE//PG//PHP/JGP/EFP/EM//BDf/TH//GFP/CEP/DEP/EEv/BDv/MS//IJ//JHf/JHP/JP//IQf/IHP/IJv/LSf///7SHOh0AAABUdFJOUwAAAAAAAAAAAAAAAAAABiZCQykIAUGn3/Hy4q5KAwRy7vJ/Yfb7cR/X4ipkdpepAqi5mavM2z5v/pGTtZS2QtP4999bIGyry8yUR4fJzbJ2BRIRE9ZoIHEAAAABYktHRAH/Ai3eAAAAB3RJTUUH6AIGEyohVAr+rAAAARZJREFUGNNjYGBgZGTi4xcQFBJmZmRkYQDxRUTFxCUkpaRlZBkZQXw5eYWQ0LCw0HBFJWGgCCOrskpEZFR0dExkrKoaG1BAXSMuPiExOjopOSpFU4uRgV07NS09IzMqKzsnNy9fh4OBU7egsKi4JCo6ubSsvEJPlkHfoDIqqqq6prauPiqqwVCYgcuosam5pbWtvaOzq6nbWJZBy6Snt69/wsRJk6f0TZ1masZgbjF9xsxZhbPnzJ01c8a8+ZYMVgt6F5aHLly0eGHokqVTl1kz2CxYXhi1YuWq1WuiouauXWbLYGe/bv2GjZscHDdv2bh1m5MzA7eLq5u7h6eXoLePr5+/ENDpjBwBgYH6PIyMQcF8vIyMAKnZUpQQgaV4AAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDI0LTAyLTA2VDE5OjQyOjI1KzAwOjAwybP6HAAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyNC0wMi0wNlQxOTo0MjoyNSswMDowMLjuQqAAAAAodEVYdGRhdGU6dGltZXN0YW1wADIwMjQtMDItMDZUMTk6NDI6MzMrMDA6MDBAgVbbAAAAAElFTkSuQmCC&color=20BEFF"/></a>
</span>
<a href="https://doi.org/10.18653/v1/2024.findings-emnlp.546"><img src="https://img.shields.io/static/v1?label=Paper&message=ACL Anthology&color=green&logo=arxiv"></a>
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

To replicate the results of **HintQA**, we encourage you to explore the **[RAG Pipeline](https://hinteval.readthedocs.io/en/latest/howtos/applications/rag_pipeline.html)** section in the **HintEval** documentation. This guide provides step-by-step instructions on implementing the methodology outlined in the HintQA paper.  

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
