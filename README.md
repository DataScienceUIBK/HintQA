![Alt text](banner.jpeg "HintQA")

<span align="center">
    <a href="https://huggingface.co/datasets/JamshidJDMY/HintQA/tree/main"><img alt="Huggingface" src="https://img.shields.io/static/v1?label=Datasets&message=HintQA&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAIGNIUk0AAHomAACAhAAA+gAAAIDoAAB1MAAA6mAAADqYAAAXcJy6UTwAAAIoUExURQAAAP/////57v/67xUVFf/clv+KAP/uzf/sxv8AAP9TAP/ltP///v/ouP/////////////////////////////8+v/pvP/biP/Vbf/Vbv/cif/qv//9+//////////03v/Yev/Zfv/14//25v/Uav/Vbv/46//////dkf/gmP/////04P/25//pvP/sxf/////lr//ouP/qwP/tyf/msv/ntf/+/P/36f/LUf/36P/w0v/w0//w0//w0//78//gm//QZv/RZv/gm//78v/////14v/nt//gnP/hn//w0f/////w0f/hn//gnP/nt//14v/////////////////LLv/MGv/PGf/LL//LG//THP/THv/SHv/UHv/LGv/LH/7SHuK8JOzDIuW+I+jAI//LHv/PTP/NF/PBG3BkOpyGMvrOH4R0NoV0NvzJGv/MF//QT//MLv/LGPu/FNayJu7FIdq2Jf7DFP/JF//ML//LJurCIsCiKujCIubAI7+hK/DHIf/LJ//HK//NGf/SHeS9IlxSP25QQmtOQmVZPu3DIf/RHf/HLP++Kf/AD/++EP3EFNCfLNhpQthrQdinKv/FFP/AEP+/K/++Dv/BEv+/Ef/CE//MIf/NIP/MGf++D//KTP/FOP/DE//PG//PHP/JGP/EFP/EM//BDf/TH//GFP/CEP/DEP/EEv/BDv/MS//IJ//JHf/JHP/JP//IQf/IHP/IJv/LSf///7SHOh0AAABUdFJOUwAAAAAAAAAAAAAAAAAABiZCQykIAUGn3/Hy4q5KAwRy7vJ/Yfb7cR/X4ipkdpepAqi5mavM2z5v/pGTtZS2QtP4999bIGyry8yUR4fJzbJ2BRIRE9ZoIHEAAAABYktHRAH/Ai3eAAAAB3RJTUUH6AIGEyohVAr+rAAAARZJREFUGNNjYGBgZGTi4xcQFBJmZmRkYQDxRUTFxCUkpaRlZBkZQXw5eYWQ0LCw0HBFJWGgCCOrskpEZFR0dExkrKoaG1BAXSMuPiExOjopOSpFU4uRgV07NS09IzMqKzsnNy9fh4OBU7egsKi4JCo6ubSsvEJPlkHfoDIqqqq6prauPiqqwVCYgcuosam5pbWtvaOzq6nbWJZBy6Snt69/wsRJk6f0TZ1masZgbjF9xsxZhbPnzJ01c8a8+ZYMVgt6F5aHLly0eGHokqVTl1kz2CxYXhi1YuWq1WuiouauXWbLYGe/bv2GjZscHDdv2bh1m5MzA7eLq5u7h6eXoLePr5+/ENDpjBwBgYH6PIyMQcF8vIyMAKnZUpQQgaV4AAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDI0LTAyLTA2VDE5OjQyOjI1KzAwOjAwybP6HAAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyNC0wMi0wNlQxOTo0MjoyNSswMDowMLjuQqAAAAAodEVYdGRhdGU6dGltZXN0YW1wADIwMjQtMDItMDZUMTk6NDI6MzMrMDA6MDBAgVbbAAAAAElFTkSuQmCC&color=20BEFF"/></a>
</span>
<a href="https://opensource.org/license/mit"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=red"></a>

# HintQA: Exploring Hint Generation Approaches in Open-Domain Question Answering
*HintQA* revolutionizes the field of automatic question answering by introducing a novel context preparation method that utilizes Automatic Hint Generation. Unlike traditional QA systems that rely on either retrieval-based methods (sourcing documents from databases like Wikipedia) or generation-based approaches (using large language models to generate context), HintQA prompts large language models to produce hints that guide the answering process.

## Datasets
In this study, we have generated up to 10 hints for each question of popular datasets [⬇️TriviaHG](https://huggingface.co/datasets/JamshidJDMY/TriviaHG/resolve/main/training.json?download=true), [⬇️NaturalQuestions](https://huggingface.co/datasets/JamshidJDMY/TriviaHG/resolve/main/training.json?download=true), and [⬇️WebQ](https://huggingface.co/datasets/JamshidJDMY/TriviaHG/resolve/main/training.json?download=true) using Automatic Hint Generation systems. You can access and download each subset by clicking on its respective link.

The datasets are structured as JSON files, including Vanilla.json, FineTuned.json, and test.json for training, validation, and test phases, respectively:

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

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Citation
If you find this work useful, please cite our paper:

## Acknowledgments
Thanks to our contributors and the University of Innsbruck for supporting this project.
