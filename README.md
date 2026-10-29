# Fruit Health Detection

A deep learning project that identifies a fruit (apple, banana, orange) and checks whether it is fresh or rotten from a photo.

## Features
- Fruit name classification (apple, banana, orange)
- Fresh vs rotten (health) classification
- Live demo with webcam or image upload using Gradio

## Tech Stack
Python, TensorFlow/Keras, MobileNetV2 (transfer learning), Gradio, Google Colab

## Dataset
Kaggle: "Fruits fresh and rotten for classification" (sriramr)
About 2,400 images used for training.
Dataset is not included here because of its size. Download it from Kaggle.

## Model
- Base model: MobileNetV2 (pretrained on ImageNet)
- Two separate models: one for fruit name, one for fruit health
- Trained for 2 epochs on CPU in Google Colab

## Results
| Model | Validation Accuracy |
|---|---|
| Fruit name | 100% |
| Fruit health (fresh/rotten) | 98.33% |

## How to Run
1. Open the notebook `fruit-phase1.ipynb` in Google Colab.
2. Download the dataset from Kaggle and place it in Google Drive.
3. Run the cells from top to bottom.
4. Models are saved to Google Drive and can be loaded again with `load_model(...)`.

## Future Work
- Add fruit shape and size analysis
- Phase 2: coating/wax detection
- Add more fruit types
- Deploy as a web app (Streamlit or Hugging Face Spaces)
