# 🌱 Seed Quality Detection System

An advanced deep learning-based application that automates seed quality assessment using computer vision and machine learning techniques. This system provides real-time analysis of seed images to determine their quality with high accuracy.

![Seed Quality Detection](https://img.shields.io/badge/Seed%20Quality-Detection-green)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![React](https://img.shields.io/badge/React-Latest-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## 📖 Table of Contents
- [Features](#-features)
- [Technology Stack](#-technology-stack)
- [System Requirements](#-system-requirements)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Configuration](#-configuration)
- [Model Training](#-model-training)
- [Testing](#-testing)
- [Performance](#-performance)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

- **Real-time Analysis**: Instant seed quality assessment through image processing
- **High Accuracy**: ~95% accuracy using ResNet50 architecture
- **User-friendly Interface**: Modern React-based web interface
- **Detailed Reports**: Comprehensive quality assessment reports
- **Cross-platform**: Works on Windows, Linux, and macOS
- **Fast Processing**: Average inference time under 1 second
- **Multiple Format Support**: Handles JPG and PNG image formats

## 🛠 Technology Stack

### Backend
- **Python 3.8+**
- **Flask**: Web framework
- **TensorFlow/Keras**: Deep learning framework
- **NumPy**: Numerical computations
- **Pillow (PIL)**: Image processing

### Frontend
- **React.js**: UI framework
- **JavaScript/ES6+**
- **CSS3/HTML5**
- **Axios**: HTTP client

### Machine Learning
- **TensorFlow 2.x**
- **ResNet50 Architecture**
- **Image Processing Libraries**

## 💻 System Requirements

- Python 3.8 or higher
- Node.js 14.x or higher
- npm or yarn
- 4GB RAM minimum (8GB recommended)
- 2GB free disk space
- NVIDIA GPU (optional, for faster processing)

## 📥 Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/tharun9392/seed-quality.git
   cd seed-quality
   ```

2. **Backend Setup**
   
   For Windows:
   ```powershell
   .\setup_dependencies.ps1
   ```

   For Linux/Mac:
   ```bash
   chmod +x setup_dependencies.sh
   ./setup_dependencies.sh
   ```

3. **Frontend Setup**
   ```bash
   cd frontend
   npm install
   ```

## 🚀 Usage

1. **Start Backend Server**
   ```bash
   cd backend
   python app.py
   ```
   Backend will run on http://localhost:5000

2. **Start Frontend Development Server**
   ```bash
   cd frontend
   npm start
   ```
   Access the application at http://localhost:3000

3. **Using the Application**
   - Upload a seed image through the web interface
   - Click "Analyze" to process the image
   - View the detailed quality assessment results
   - Download or export reports as needed

## 📁 Project Structure

```
seed-quality/
├── backend/               # Flask server and ML components
│   ├── app.py            # Main server file
│   └── requirements.txt  # Python dependencies
├── frontend/             # React frontend application
│   ├── src/             # Source code
│   ├── public/          # Static files
│   └── package.json     # Node dependencies
├── model/               # ML model files
│   ├── train_model.py
│   └── seed_classifier_resnet50.h5
├── dataset/             # Training and test datasets
├── evaluate/            # Evaluation scripts
├── test/               # Test suites
├── setup_dependencies.sh
├── setup_dependencies.ps1
└── README.md
```

## ⚙️ Configuration

### Backend Configuration
- Model path: `MODEL_PATH` in `backend/app.py`
- Server port: 5000 (default)
- Image size: 224x224 pixels (default)

### Frontend Configuration
- API endpoint: Configure in `.env` files
- Port: 3000 (default)

## 🧠 Model Training

To train the model with custom data:

1. Prepare your dataset in the `dataset` directory
2. Configure training parameters in `model/train_model.py`
3. Run training:
   ```bash
   python model/train_model.py
   ```

## 🧪 Testing

Run the test suite:
```bash
cd test
python -m pytest
```

## 📊 Performance

- **Model Accuracy**: ~95% on test dataset
- **Inference Time**: <1 second per image
- **Supported Formats**: JPG, PNG
- **Resolution**: Optimized for 224x224 pixels

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👥 Authors

- Your Name - Initial work - [GitHub Profile](https://github.com/tharun9392)

## 🙏 Acknowledgments

- ResNet50 architecture team
- TensorFlow development team
- Open source community



