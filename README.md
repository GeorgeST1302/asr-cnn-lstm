# Speech Recognition with DeepSpeech2 (TensorFlow)

This project demonstrates end-to-end speech recognition using the LJSpeech dataset and a DeepSpeech2-like model implemented in TensorFlow/Keras. The code was originally developed and tested on Kaggle, but you can run it locally or on other platforms by following these steps.

---

## Step-by-Step Instructions

### 1. Clone or Download the Repository
- Download this repository from GitHub to your local machine.

### 2. Install Python and Jupyter Notebook
- Make sure you have Python 3.7+ installed.
- Install Jupyter Notebook:
  ```sh
  pip install notebook
  ```

### 3. Install Required Python Packages
- Open a terminal in the project directory and run:
  ```sh
  pip install tensorflow pandas numpy matplotlib jiwer
  ```

### 4. Download the LJSpeech Dataset
- Download the LJSpeech-1.1 dataset from [https://keithito.com/LJ-Speech-Dataset/](https://keithito.com/LJ-Speech-Dataset/)
- Unzip the dataset so you have the following structure:
  ```
  LJSpeech-1.1/
      metadata.csv
      wavs/
          LJ001-0001.wav
          ...
  ```
- Place the `LJSpeech-1.1` folder in the same directory as the notebook file (`speech-recognition.ipynb`).

### 5. Open the Notebook
- Start Jupyter Notebook:
  ```sh
  jupyter notebook
  ```
- Open `speech-recognition.ipynb` in your browser.

### 6. Update Data Path (if needed)
- If your dataset is not in the default location, update the `data_path` variable in the notebook to point to your dataset folder.
- Example:
  ```python
  data_path = "./LJSpeech-1.1"
  ```

### 7. Run All Cells
- Run each cell in order (from top to bottom).
- The notebook will:
  - Load and preprocess the data
  - Build and train a speech recognition model
  - Evaluate and display results

### 8. Notes and Troubleshooting
- If you encounter missing package errors, install them using `pip install <package-name>`.
- Training is resource-intensive. For best performance, use a machine with a GPU.
- If you use Kaggle, you can upload the notebook and dataset directly to a Kaggle notebook environment and run all cells without changing paths.

---

## Credits
- Dataset: [LJSpeech-1.1](https://keithito.com/LJ-Speech-Dataset/)
- Model: DeepSpeech2-inspired architecture in TensorFlow/Keras

---

For questions or issues, please open an issue on the GitHub repository.
