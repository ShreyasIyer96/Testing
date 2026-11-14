# Testing

![AI101 Mini-Project](https://img.shields.io/badge/AI101%20Mini--Project-green)
![Team 28](https://img.shields.io/badge/Team-28-green)
![Python 3.10+](https://img.shields.io/badge/Python-3.12%2B-green?logo=python&logoColor=white)
lol
## Team and roles
| Member | Entry no. | Role | GitHub Handle|
|---|---|---|---|
| Shreyas Iyer | 2026EEB1412 | Documentation lead | [@Shreyas-IITRPR](https://github.com/Shreyas-IITRPR) |
| Hisham Muhammad K | 2026MCB1530 | Execution lead | [@Hisham-iitrpr](https://github.com/Hisham-iitrpr) |
| Saniya Jain | 2026DAB1306 | PPT lead | [@Saniya-Jn](https://github.com/Saniya-Jn) |
| Bhakti Bagade | 2026AIB1027 | Video lead | [@Bhakti-iitrpr](https://github.com/Bhakti-iitrpr) |

All four members write code and commit from their own accounts (see commit history).
## Project structure

```
AI-Layoff-Risk-Predictor/
├── ai101_team28.ipynb              # all code, with output cells
├── ai-impact-jobs-layoff-risk-dataset.csv   # dataset (keep it next to the notebook)
├── training_curve_gd.png                    # training curve, saved by the notebook
├── outputs/                                 # plots and metrics.json saved by the notebook
├── docs/Team28_slides.pdf                  # 5 slides
├── requirements.txt
└── README.md
```

## Setup

Python 3.12 or newer. The notebook was last run on Python 3.14.6, and its code was re-checked on Python 3.12 with the versions in `requirements.txt` (same final metrics).

```bash
git clone https://github.com/Shreyas-IITRPR/AI-Layoff-Risk-Predictor.git
```
```bash
cd AI-Layoff-Risk-Predictor
```
```bash
python -m venv venv
```
- Linux / macOS
```bash
source venv/bin/activate 
```
- Windows:
```bash
venv\Scripts\activate
```
```bash
pip install -r requirements.txt
```
## How to run

1. From the repo folder, run `jupyter notebook`.
2. Open `ai101_team28.ipynb`.
3. Choose **Kernel → Restart & Run All**. It finishes in well under a minute and saves the plots and `metrics.json` in `outputs/` (and `training_curve_gd.png` in the repo folder).

The data path is relative (`ai-impact-jobs-layoff-risk-dataset.csv`), so the notebook and the CSV must stay in the same folder.

## Expected output

| | Train | Test |
|---|---|---|
| Accuracy | 0.941000 | 0.937750 |
| Precision (macro) | 0.940924 | 0.937548 |
| Recall (macro) | 0.940860 | 0.937530 |
| F1 (macro) | 0.940888 | 0.937535 |
| ROC AUC (macro, one-vs-rest) | 0.994580 | 0.993885 |

<img width="890" height="340" alt="training_curve_gd" src="https://github.com/user-attachments/assets/3e12f13a-47a8-4d8a-95d2-d0336c27c970" />
<img width="851" height="390" alt="Confusion_Matrix" src="https://github.com/user-attachments/assets/23a5a4eb-f01b-46c4-888e-0bdb04db653f" />
<img width="890" height="390" alt="ROC_curve" src="https://github.com/user-attachments/assets/5773a3f1-bd2b-46d9-a25a-77b82dec8189" />

## Links
- Slides:[Team28_slides](https://drive.google.com/file/d/1vXiiMBQ3SsCNKfQXjiQKUsnSEoDO3oOH/view?usp=drivesdk)
- Video: [Project Video](https://drive.google.com/file/d/1pzjD4EJI8dMH936MUILzIbMN4KOArENa/view?usp=sharing)
## Note

One early commit, with commit message <made output folder with the metrices.json file> in this repository was made by @ShreyasIyer96, a personal account belonging to @Shreyas-IITRPR (Shreyas Iyer), by mistake while logged in to the wrong account. Kindly ignore this commit. All other commits by this member are from @Shreyas-IITRPR.

## AI-use disclosure


- Claude: First draft of README, assisted with code for plotting curves & debugged an error in SGDCclassifier code
- No AI was used to generate the dataset. All reported metrics come from running the notebook.

