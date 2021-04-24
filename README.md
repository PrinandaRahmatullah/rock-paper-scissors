# Rock Paper Scissors Image Classifcation

Final Project of Belajar Machine Learning Pemula Course by Dicoding Indonesia

## Information

Run on Google Colaboratory with GPU accelerator

## Dataset

Dataset of Rock Paper Scissors can be downloaded [here](https://drive.google.com/drive/folders/1jwh_0uxDYu9cDEi83bHvPcGIoWejZ4Zq?usp=sharing)

## Submission Criteria

- Split data into train set 60% and validation set with size 40%.
- Implement image augmentation using ImageDataGenerator
- Using Sequential model
- Training of the model less than 30 minutes
- Model accuracy at least 85%
- Able to predict image uploaded to Colab widget

## Result

Model composed of 4 Convolutinal 2D layers with 16, 32, 64, and 128 channels, 4 MaxPooling2D layers, 1 Flatten layer, 1 Fully Connected Layer with 32 channels, and output layer with 3 channels and softmax activation function.

- Learning rate : 0.001
- Epoch : 30 epochs (supported by Model Checkpoint callback)
- Batch Size : 10 and 20

  | Batch Size | Loss   | Accuracy | Validation Loss | Validation Accuracy |
  | ---------- | ------ | -------- | --------------- | ------------------- |
  | 10         | 0.1217 | 0.9688   | 0.0628          | 0.9920              |
  | 20         | 0.0764 | 0.9711   | 0.0353          | 0.9897              |

## Conclusion

From the result above, we got batch size with value 10 has higher validation accuracy than batch size with value 20, but it has lower validation loss than batch size 20.
