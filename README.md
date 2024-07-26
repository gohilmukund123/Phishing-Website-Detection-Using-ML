# Phishing Website Detection Using ML

This project focuses on detecting phishing websites using machine learning techniques. The goal is to identify fraudulent websites and protect users from online scams by analyzing various features of the websites.

## Aim of Project
Phishing is a type of online scam where attackers deceive users into providing sensitive information such as usernames, passwords, and credit card details by pretending to be trustworthy entities. This project leverages machine learning algorithms to detect phishing websites by examining various features extracted from the URLs and website content.

## Project Overview
The project is divided into two main stages:
1. **Feature Extraction**: Extracting relevant features from URLs and website content to build a dataset for training the machine learning model.
2. **Model Training and Evaluation**: Training a machine learning model using the extracted features and evaluating its performance.

## Dataset
The dataset used in this project contains URLs of benign (legitimate) websites. Below are some details about the dataset:

- **Number of entries**: 35,377
- **Number of columns**: 1
- **Column name**: The dataset consists of a single column containing the URLs of benign websites.

### Sample Data
Here are a few examples of the benign URLs in the dataset:

| URL |
| --- |
| http://1337x.to/torrent/1110018/Blackhat-2015-BRRip-XviD-EVO/ |
| http://1337x.to/torrent/1122940/Blackhat-2015-720p-WEB-DL-H264-AC3-EVO/ |
| http://1337x.to/torrent/1124395/Fast-and-Furious-7-2015-DVDRip-XviD-EVO/ |
| http://1337x.to/torrent/1145504/Avengers-Age-of-Ultron-2015-DVDRip-XviD-EVO/ |
| http://1337x.to/torrent/1160078/Avengers-age-of-ultron-2015-720p-WEB-DL-AC3-EVO/ |

## Feature Extraction
Feature extraction involves deriving meaningful attributes from the raw URLs to serve as input for the machine learning model. The following features are extracted:
- **Domain Age**: Age of the domain in years.
- **Presence of HTTPS**: Whether the URL uses HTTPS (secure) protocol.
- **Length of URL**: The total length of the URL.
- **Number of Dots**: Number of dots in the URL.

These features are crucial in distinguishing between phishing and legitimate websites.

## Model Training and Evaluation
The project uses various machine learning algorithms to train the model and evaluate its performance. The key steps include:

1. **Model Selection**: Choosing appropriate machine learning algorithms such as Decision Tree, Random Forest, and XGBoost.
2. **Training**: Training the model on the preprocessed dataset.
3. **Evaluation**: Evaluating the model's performance using metrics such as accuracy, precision, recall, and F1-score.

### Example Model Output
```
XGBoost: Accuracy on training Data: 0.979
XGBoost : Accuracy on test Data: 0.979
```

## Usage
To use this project, follow these steps:
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```
2. **Install Dependencies**:
   Install the required Python packages using pip:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Notebooks**:
   Open the Jupyter notebooks (`FeatureExtraction.ipynb` and `Stage2.ipynb`) in Jupyter Lab or Jupyter Notebook and run the cells to execute the feature extraction and model training steps.

## Contributing
Contributions are welcome! If you have any suggestions or improvements, please feel free to create a pull request or open an issue.
