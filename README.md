# CNN-Architectures
A Race classification which explore all the possible architecture to find the best model available

The models that we will use for this text will be:
- Model_1 : A Random(A control for this test)
- Model_2 : Model with extra layers and methods like Dropout, MaxPooling2D, LeakyReLU etc
- Model_3 : Using VGG16 as convolutional base
- Model_4 : Using ResNet50V2 as convolutional base
- Pretrained models(ResNet, VGG16)

About Dataset:
- The dataset was provided in kaggle with images of humans belonging to 3 races
      Caucasian
      Mongoloid
      Negroid
- Train and test Data had 1651 and 74 files respectively belonging to 3 classes.

Model Performances:
- Model_1: Being a baseline untuned model gave us the least results as expected
      - val_loss = 0.8837
      - val_accuracy = 0.6081
- Model_2: Adding a few extra layers such as Dropout, MaxPooling, changing the activation function from 'ReLU' to 'LeakyReLu' greatly improved our results
      - val_loss = 0.6309
      - val_accuracy = 0.7568
- Using the convolutional base of VGG16(untrainable) for our model did perform better than our baseline Model_1 but was not better than Model_2
      - val_loss = 0.7126
      - val__accuracy = 0.7432
- Using the convolutional base of Resnet50V2(untrainable) for our model did perform better than our baseline Model_1 and VGG16 but still was not better than Model_2
      - val_loss = 0.6770
      - val_accuracy = 0.6892
