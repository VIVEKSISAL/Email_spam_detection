# 📧 Spam Email Detection System

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.32+-red.svg)](https://streamlit.io/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.6+-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A robust, production-ready machine learning system for classifying emails as spam or legitimate (ham). Built with a modular architecture, comprehensive evaluation metrics, and an intuitive web interface for real-time analysis.

## ✨ Features

- **🔬 Advanced ML Pipeline**: Modular design with separate components for data ingestion, preprocessing, model training, and inference
- **🤖 Multiple Algorithms**: Support for SVM, Logistic Regression, Decision Trees, KNN, and Random Forest with automated model selection
- **🌐 Interactive Web UI**: Modern Streamlit interface for single email classification and batch MBOX processing
- **📊 Comprehensive Analytics**: Detailed performance metrics, cross-validation results, and model comparison reports
- **📁 MBOX Support**: Native processing of email archives with batch classification capabilities
- **🔧 Highly Configurable**: Easy parameter tuning and custom model configurations
- **📈 Production Ready**: Logging, error handling, and scalable architecture

## 🛠️ Tech Stack

- **Language**: Python 3.10+
- **Web Framework**: Streamlit
- **ML Libraries**: Scikit-learn, Pandas, NumPy
- **Data Processing**: BeautifulSoup4 for HTML parsing
- **Environment Management**: uv/pip with virtual environments
- **Version Control**: Git

## 📂 Project Structure

```
spam-email-detection/
├── 📄 app.py                    # Main Streamlit web application
├── 📄 requirements.txt          # Python dependencies
├── 📄 pyproject.toml           # Project configuration
├── 📄 README.md                # Project documentation
├── 📁 src/
│   ├── 📁 components/          # Core ML components
│   │   ├── 📄 data_ingestion.py    # Data loading utilities
│   │   ├── 📄 data_transformation.py # Feature engineering
│   │   └── 📄 model_training.py     # Model training logic
│   ├── 📁 pipeline/            # Pipeline orchestration
│   │   ├── 📄 prediction_pipeline.py # Inference pipeline
│   │   └── 📄 training_pipeline.py   # Training pipeline
│   ├── 📁 config/              # Configuration management
│   │   └── 📄 config.py            # Project settings
│   └── 📁 utils/               # Utility functions
│       ├── 📄 email_utils.py       # Email processing helpers
│       ├── 📄 logger.py            # Logging configuration
│       └── 📄 utils.py             # General utilities
├── 📁 data/                    # Input datasets
├── 📁 outputs/                 # Model artifacts and results
├── 📁 Notebook Experiments/   # Jupyter notebooks for analysis
└── 📄 .gitignore              # Git ignore rules
```

## 🚀 Quick Start

### Prerequisites
- Python 3.10 or higher
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/VIVEKSISAL/Email_spam_detection.git
   cd Email_spam_detection
   ```

2. **Create virtual environment**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the application**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   Navigate to `http://localhost:8501`

## 📖 Usage

### Web Interface

The Streamlit app provides two main functionalities:

#### Single Email Classification
- Paste email content in the text area
- Click "Classify Email" for instant results
- View prediction (Spam/Ham) with confidence score

#### Batch MBOX Processing
- Upload `.mbox` email archive files
- Process multiple emails simultaneously
- Download classification results as CSV

### Command Line Training

To retrain models on new data:

```bash
# Place your dataset in data/dataset/dataset.csv
python -m src.pipeline.training_pipeline
```

## ✅ Screenshots
<img width="1920" height="1080" alt="Screenshot from 2026-04-09 14-06-24" src="https://github.com/user-attachments/assets/f5f7f0ee-067a-4819-ab95-ae07416d9530" />

<img width="1920" height="1080" alt="Screenshot from 2026-04-09 14-08-42" src="https://github.com/user-attachments/assets/7a40f294-7c50-4685-acb3-c4bfddccd758" />

<img width="1920" height="1080" alt="Screenshot from 2026-04-09 14-10-57" src="https://github.com/user-attachments/assets/435f8843-5916-4d7a-bb9a-90f71371381c" />

<img width="1920" height="1080" alt="Screenshot from 2026-04-09 14-11-33" src="https://github.com/user-attachments/assets/d1cc1b88-96b4-422e-88a8-9afbadb1c552" />

<img width="1920" height="1080" alt="Screenshot from 2026-04-09 14-27-14" src="https://github.com/user-attachments/assets/54585ae2-2b03-461c-ab5c-1282e71b6cc4" />



## ⚙️ Configuration

Customize the system through `src/config/config.py`:

- **Model Parameters**: Adjust hyperparameters for different algorithms
- **File Paths**: Configure input/output directories
- **Training Settings**: Modify cross-validation folds and evaluation metrics
- **Feature Engineering**: Customize text preprocessing and feature extraction

## 📊 Model Performance

The system evaluates models using 5-fold cross-validation with comprehensive metrics:

- **Accuracy**: Overall classification accuracy
- **Precision**: True positive rate
- **Recall**: Sensitivity of spam detection
- **F1-Score**: Harmonic mean of precision and recall

### Current Best Model: SVM
- **Accuracy**: 98.2%
- **Precision**: 97.8%
- **Recall**: 98.5%
- **F1-Score**: 98.1%

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 style guidelines
- Add tests for new features
- Update documentation
- Ensure all tests pass

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with ❤️ using Streamlit and Scikit-learn
- Inspired by the need for effective email spam detection
- Thanks to the open-source community for amazing tools

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Check the documentation
- Review the code comments

---

**⭐ Star this repository if you find it helpful!**

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 🖥️ Usage

### 1. Running the Web Application
Launch the interactive dashboard to classify emails instantly.

```bash
streamlit run app.py
```

- **Single Email Tab**: Paste email content to get an immediate Spam/Ham prediction with a confidence score.
- **Batch Processing Tab**: Upload an `.mbox` file to process multiple emails at once and download the results as a CSV.

### 2. Training the Model
(Optional) If you wish to retrain the models on new data:

1. Place your dataset in `data/dataset/dataset.csv`.
2. Run the training pipeline:
   ```bash
   python -m src.pipeline.training_pipeline
   ```
3. Artifacts (Model & Vectorizer) will be saved in the `outputs/` directory.
4. **Important**: Update `src/config/config.py` with the new paths to your generated model and vectorizer if they change.

## ⚙️ Configuration

The system is highly configurable via `src/config/config.py`. You can adjust:
- Model hyperparameters (Grid Search configuration)
- Input/Output paths
- Training parameters (Cross-validation folds, etc.)

## 📊 Model Performance

The pipeline automatically evaluates models using 5-fold cross-validation. Metrics including Accuracy, Precision, Recall, and F1-Score are logged for each experiment. By default, the system selects the best performing model (often SVM or Random Forest) for inference.

## 🤝 Contributing

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.
