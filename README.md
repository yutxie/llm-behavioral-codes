# Using Large Language Models to Categorize Strategic Situations and Decipher Motivations Behind Human Behaviors

Thanks for your interest! This repository contains the code and data for the paper ["Using Large Language Models to Categorize Strategic Situations and Decipher Motivations Behind Human Behaviors"](https://arxiv.org/pdf/2503.15752).


## File Description

| File/Folder | Description | Reproducing the Results |
|-------------|-------------|-------------------------|
| `Behavioral Codes.csv` | Summarizes all behavioral codes learned and analyzed in this study for quick reference. | --- |
| `data/`     | Contains human data from MobLab and the meta-study of the Dictator Game.  | --- |
| `records/`  | Contains the learned behavioral codes and intermediate results.  | --- |
| `clusters/` | Contains the clustering results of the behavioral codes. | --- |
| `data-preprocess.ipynb` | Preprocesses the human data. | --- |
| `learn-codes.ipynb` | Learns the behavioral codes for each game (Algorithm S1). | Fig. 2; Table S1 |
| `weight.ipynb` | Learns the weights for behavioral codes (Algorithm S2). | Fig. S14 |
| `prompt-analysis.ipynb` | Analyzes the learned behavioral codes. | Fig. 3-4,S4-S11; Table S4-S6   | 
| `visualization.ipynb` | Visualizes the learned behavioral codes. | Fig. 5-7,S12-S13 |
| `consistency.ipynb` | Analyzes the consistency of behaviors that can be elicited from behavioral codes. | Fig. S1 | 
| `generalizability.ipynb` | Analyzes the generalizability of behavioral codes across different LLMs. | Fig. S2 |
| `evaluate.ipynb` | Evaluates behavioral code mixtures compared with human data. | Fig. S3; Table S2-S3 |

## Behavioral Codes

`Behavioral Codes.csv` summarizes all behavioral codes learned and analyzed in the study for quick reference. Each row is a unique code, and the columns are:
* `Behavioral Code`: The content in the code -- a natural language description that articulates  the motivation that might influence behavior. 
* `Elicited Behaviors`: The behaviors that can be elicited from an LLM (`gpt-4o-2024-05-13`) using the code as the system prompt. 
* `Game`: The economic game that the code is learned from.

## Dependencies

Required packages are listed in `environment.yml`. Some commented-out code in the notebooks may require instailling some additional packages (e.g., `spacy`, `umap`) and resolving the dependency conflicts manually. The exported conda environment is only for reproducing the results with the preprocessed intermediate data in `/records`.

## Citation and Contact

```
@article{xie2025using,
  title={Using Large Language Models to Categorize Strategic Situations and Decipher Motivations Behind Human Behaviors},
  author={Xie, Yutong and Mei, Qiaozhu and Yuan, Walter and Jackson, Matthew O},
  journal={arXiv preprint arXiv:2503.15752},
  year={2025}
}
```

Please contact Yutong Xie (yutxie AT umich DOT edu) if you find any problem in the code or data. 