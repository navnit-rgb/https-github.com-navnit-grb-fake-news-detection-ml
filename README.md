# https-github.com-navnit-grb-fake-news-detection-ml
# Fake News Detection Using Machine Learning

A beginner-friendly machine learning project that classifies news as **Fake** or **Real** using TF-IDF text features and Logistic Regression.

## Features
- Text preprocessing
- TF-IDF vectorization
- Logistic Regression classifier
- Accuracy, classification report and confusion matrix
- Streamlit web interface
- Saved trained model
- Easy GitHub deployment

## Project Structure

```text
fake-news-detection-ml/
├── app.py
├── train_model.py
├── predict.py
├── requirements.txt
├── README.md
├── .gitignore
├── data/
│   └── news.csv
└── model/
    └── (generated after training)
```

## 1. Install Python

Install Python 3.10+ and make sure `python --version` works in your terminal.

## 2. Create and activate a virtual environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

## 3. Install dependencies

```bash
pip install -r requirements.txt
```

## 4. Prepare the dataset

Put your dataset at:

```text
data/news.csv
```

The CSV should contain these columns:

```text
title,text,label
```

Use labels such as `fake` and `real` (or `0` and `1`).

If your dataset has different column names, edit the column names in `train_model.py`.

## 5. Train the model

```bash
python train_model.py
```

The trained files will be created inside the `model/` folder.

## 6. Test prediction from terminal

```bash
python predict.py
```

## 7. Run the web app

```bash
streamlit run app.py
```

Then open the local URL shown by Streamlit, normally:

```text
http://localhost:8501
```

## 8. Upload to GitHub

Initialize Git:

```bash
git init
git add .
git commit -m "Initial fake news detection ML project"
```

Create a new repository on GitHub named:

```text
fake-news-detection-ml
```

Then connect your local project:

```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/fake-news-detection-ml.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

## Important

Do not upload:
- `venv/`
- passwords/API keys
- very large datasets
- private or copyrighted data you are not allowed to redistribute

This project demonstrates ML classification and should not be treated as a definitive fact-checking system.
#
