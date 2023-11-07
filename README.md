
# OCR Handwriting BKAI

This project is an optical character recognition (OCR) system for handwritten Vietnamese text, based on the BKAI dataset. The system consists of two main components: a text detection model and a text recognition model. The text detection model is a deep neural network that locates and extracts text regions from an input image. The text recognition model is a convolutional recurrent neural network that transcribes the text regions into Vietnamese characters.

## Installation

To run this project, you need to install the following dependencies:

- Python 3.7 or higher
- PyTorch 1.8 or higher
- OpenCV 4.5 or higher
- Numpy 1.19 or higher
- Scikit-image 0.18 or higher
- Scikit-learn 0.24 or higher
- Tqdm 4.59 or higher

You can install them using pip:

```bash
pip install -r requirements.txt
```

## Usage

To use this project, you need to download the BKAI dataset from [here](https://drive.google.com/drive/folders/1dlhSYYrLE0GMUOUV-GDmNcJs2_Tu4KYa?fbclid=IwAR2JHnQkTvMC0sKDtqtV7l7LxdBvmyTppV0Z7mDQe0NfJJ-qSZyhJkLm66A) and unzip it in the `data` folder. The dataset contains 103,000 images of handwritten Vietnamese text with annotations.

First create the dataset, run the following command:

```bash
python OCRDataset.py
```

To train the text recognition model, run the following command:

```bash
python train.py
```

## Results

The text detection model achieves an CER(Character Error Rate) is 0.66 point, i think it not a good number, but if i have free time, i will make the model better.

## License

This project is licensed under the MIT License - see the [LICENSE](^5^) file for details.

