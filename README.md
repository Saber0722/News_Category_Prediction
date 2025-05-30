# 📰 News Category Prediction

This project focuses on classifying news articles into their respective categories using machine learning techniques. It encompasses data preprocessing, exploratory data analysis (EDA), and training multiple classification models to achieve optimal performance.

## 📂 Directory Structure

```
News_Category_Prediction/
├── data/
│   └── News_Category_Dataset_v3.json
├── notebooks/
│   ├── preprocessing.ipynb
│   ├── EDA.ipynb
│   └── train_model.ipynb
├── outputs/
│   ├── plots/
│   └── models/
├── README.md
└── .gitignore
```

* `data/`: Contains the raw dataset and will store the cleaned data after preprocessing.
* `notebooks/`: Jupyter notebooks for preprocessing, EDA, and model training.
* `outputs/`: Directory to store generated plots and trained models.

  * `plots/`: Visualizations from EDA and model evaluations.
  * `models/`: Serialized trained model files.
* `README.md`: Project overview and instructions.
* `.gitignore`: Specifies files and directories to be ignored by Git.

## 📊 Dataset Overview

The dataset used is [`News_Category_Dataset_v3.json`](https://www.kaggle.com/datasets/rmisra/news-category-dataset), which comprises news articles with attributes such as:

* `headline`: The title of the news article.
* `short_description`: A brief summary of the article.
* `category`: The category label for the article (e.g., Politics, Entertainment, Tech).

This dataset is instrumental in training models to accurately predict the category of a news article based on its content.

## 🛠️ Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Saber0722/News_Category_Prediction.git
   cd News_Category_Prediction
   ```

2. **Create Necessary Directories**

   Ensure the following directory structure exists:

   ```bash
   mkdir -p outputs/plots
   mkdir -p outputs/models
   ```

   These directories will store the output plots and trained models respectively.

3. **Install Dependencies**

   It's recommended to use a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

   *Note: Ensure that a `requirements.txt` file is present with all necessary dependencies listed.*

## 🔄 Workflow

1. **Data Preprocessing**

   Run the `preprocessing.ipynb` notebook to clean and preprocess the raw data. This will generate a `cleaned_data.csv` file stored in the `data/` directory.

2. **Exploratory Data Analysis (EDA)**

   Execute the `EDA.ipynb` notebook to perform EDA on the cleaned data. This step utilizes `cleaned_data.csv` and generates various visualizations stored in `outputs/plots/`.

3. **Model Training**

   Run the `train_model.ipynb` notebook to train multiple classification models on the preprocessed data. The trained models will be saved in the `outputs/models/` directory.

## 🤖 Models Implemented

The following machine learning models are trained and evaluated:

* **Logistic Regression**
* **Naive Bayes**
* **Random Forest**
* **Support Vector Machine (SVM)**
* **XGBoost**

Each model's performance is assessed using appropriate evaluation metrics, and the best-performing model is identified for deployment.

## 📄 License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this project as per the license terms.

---

Feel free to contribute to this project by submitting issues or pull requests. For any queries or suggestions, please open an issue in the repository.
