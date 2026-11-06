# Machine Learning & Data Science Portfolio

A collection of hands-on data analysis, machine learning, and deep learning projects
by **Kinnshuk Bhaduri**. Each project lives in its own folder with its notebook and,
where relevant, a `requirements.txt`, saved model artifacts, and a small app.

> **Note on scope:** These are learning and demonstration projects. Any metrics shown
> come from the notebook outputs themselves — this README does not claim accuracy,
> F1, R², or business-impact numbers that haven't been reproduced. Treat results as
> illustrative until re-run in a clean environment.

---

## 📂 Projects

### Data analysis & regression
| # | Project | Notebook | Core tools |
|---|---|---|---|
| 1 | Exploratory Data Analysis | [EDA Proj 1](<EDA Proj 1/EDA Proj 1.ipynb>) | pandas, numpy, matplotlib, seaborn |
| 3 | Linear Regression | [Linear Regression Proj 3](<Linear Regression on my own Proj 3/Linear Regression Proj 3.ipynb>) | pandas, numpy, matplotlib, scikit-learn |
| 5 | Housing Price Prediction | [Housing price pred Proj 5](<Housing Price prediction Proj 5/Housing price pred Proj 5.ipynb>) | pandas, numpy, seaborn, scikit-learn, xgboost |

### Classification (classic ML)
| # | Project | Notebook | Core tools |
|---|---|---|---|
| 2 | Iris Flower Classification | [Iris Classification Proj 2](<IRIS CLASSIFCIATION Proj 2/Iris flower Classification Project 2.ipynb>) | pandas, numpy, scikit-learn |
| 4 | Titanic Survival Prediction | [Titanic Proj 4](<Titanic Survival Prediction Proj 4/Titanic Survival Pred Proj 4.ipynb>) | pandas, numpy, seaborn, scikit-learn |
| 7 | Twitter Sentiment Analysis | [Twitter Sentiment Proj 7](<Twitter Sentiment Analysis Proj 7/Twitter Sentiment Analysis.ipynb>) | pandas, numpy, nltk, scikit-learn |
| 8 | Customer Churn Prediction | [Customer Churn Proj 8](<Customer Churn Predictor Proj 8/Customer Churn Predicter.ipynb>) | pandas, scikit-learn, tensorflow |

### Deep learning
| # | Project | Notebook | Core tools |
|---|---|---|---|
| 6 | Dogs vs Cats Image Classifier | [Dogs Vs Cats Proj 6](<Dog Vs Cats Classifire Proj 6/Dogs Vs Cats.ipynb>) | tensorflow, opencv-python, matplotlib |
| 9 | Stock Price Predictor | [Stock Price Proj 9](<Stocks Price Predicter Proj 9/Stock Price Predicter Proj 8.ipynb>) | pandas, numpy, scikit-learn, tensorflow |
| 10 | Neural Network From Scratch | [Neural Network Proj 10](<Neural Network From Scratch Proj 10/neural_network_from_scratch.ipynb>) | numpy |
| 11 | Face Recognition (Deep Learning) | [Face Recognition Proj 11](<Face Recognition System using DL Proj 11/Facial Recognition using Deep Learning.ipynb>) | deep-learning stack (see notebook) |

### Recommender systems
| # | Project | Notebook | App | Core tools |
|---|---|---|---|---|
| 12.1 | Movie Recommender (content-based) | [Movie Recommender Proj 12.1](<Movie Recommendation System Proj 12.1/Movie Recommender.ipynb>) | [app.py](<Movie Recommendation System Proj 12.1/app.py>) | pandas, scikit-learn, streamlit |
| 12.2 | Book Recommender (collaborative filtering) | [Books Recommender Proj 12.2](<Book Recommendation System Proj 12.2/Books Recommender.ipynb>) | [app.py](<Book Recommendation System Proj 12.2/app.py>) | numpy, scikit-learn, streamlit |

### LLM / transformers
| # | Project | Notebook | Core tools |
|---|---|---|---|
| 13 | LLM From Scratch | `LLM From Scratch Proj 13/LLM_from_Scratch.ipynb` | torch, tiktoken, numpy |

> Project 13 (LLM From Scratch) is a work in progress and may not yet be committed to the
> repository. The folder also contains a local `.venv/` and training corpus that are not tracked.

---

## 🛠️ Tech stack across the portfolio

- **Language:** Python
- **Data & analysis:** pandas, numpy, matplotlib, seaborn
- **Classic ML:** scikit-learn, xgboost
- **Deep learning:** tensorflow / keras, pytorch (`LLM From Scratch`)
- **NLP:** nltk, tiktoken
- **Computer vision:** opencv-python
- **Apps:** streamlit
- **Tooling:** Jupyter, Git

Exact dependencies vary per project — use each folder's own `requirements.txt` where present.

---

## ▶️ How to run a project

Clone the repository:

```bash
git clone https://github.com/Kinks106/ML-Portfolio.git
cd ML-Portfolio
```

Each project is self-contained. Create a fresh virtual environment per project you want to run:

```bash
# from inside a project folder, e.g. "EDA Proj 1"
python -m venv .venv

# Windows PowerShell
.venv\Scripts\Activate.ps1
# macOS / Linux
source .venv/bin/activate

python -m pip install --upgrade pip
python -m pip install -r requirements.txt   # if the folder has one
jupyter lab                                   # then open the project's .ipynb
```

For the two Streamlit recommender apps:

```bash
python -m pip install streamlit
streamlit run "app.py"
```

---

## ⚠️ Data, models & large files

Some projects reference datasets or saved models that are **not fully reproducible from a
clone alone**:

- **Dogs vs Cats (Proj 6):** contains a large `PetImages/` dataset and a saved `my_model.h5`.
  The dataset is heavy to clone; the notebook documents where the images come from.
- **Recommender apps (Proj 12.1 / 12.2):** the Streamlit apps load `.pkl` artifacts
  (`similarity.pkl`, `movies.pkl`, book model pickles) that are generated by running the
  corresponding notebook first. Regenerate them before launching the app.
- **Movie app:** requires a TMDB API key, supplied via the `TMDB_API_KEY` environment
  variable — never hard-code it.
- Large model files (`.h5`, `.pkl`, `.sav`) may or may not be tracked depending on `.gitignore`.
  See each project folder for specifics.

---

## 👤 About

**Kinnshuk Bhaduri** — AI & Data Science engineering student. I enjoy turning messy data and
repetitive workflows into clear, documented tools.

- **GitHub:** https://github.com/Kinks106
- **LinkedIn:** https://www.linkedin.com/in/kinnshuk-bhaduri/
