# Testing

![AI101 Mini-Project](https://img.shields.io/badge/AI101%20Mini--Project-green)
![Team 28](https://img.shields.io/badge/Team-28-green)
![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-green?logo=python&logoColor=white)
lol
## Team and roles

| Member | Entry no | Role |
|---|---|---|
| Member 1 (placeholder) | 2026AIB0001 | Documentation lead |
| Member 2 (placeholder) | 2026AIB0002 | Execution lead |
| Member 3 (placeholder) | 2026AIB0003 | PPT lead | 
| Member 4 (placeholder) | 2026AIB0004 | Video lead |

All four members write code and commit from their own accounts (see commit history).
## Project structure

```
ai101-team-XX-ai-layoff-risk-predictor/
├── AI_Layoff_Risk_LogReg.ipynb              # all code, with output cells
├── ai-impact-jobs-layoff-risk-dataset.csv   # dataset (keep it next to the notebook)
├── training_curve_gd.png                    # training curve, saved by the notebook
├── outputs/                                 # plots and metrics.json saved by the notebook
├── docs/Team_XX_slides.pdf                  # 5 slides
├── requirements.txt
└── README.md
```

## Setup

Python 3.12 or newer. The notebook was last run on Python 3.14.6, and its code was re-checked on Python 3.12 with the versions in `requirements.txt` (same final metrics).

```bash
git clone https://github.com/Shreyas-IITRPR/AI-Layoff-Risk-Predictor.git
cd AI-Layoff-Risk-Predictor
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
