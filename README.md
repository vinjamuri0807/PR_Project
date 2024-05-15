******Facial Emotion Recognition using Deep Learning******

****Introduction****
This project develops a facial emotion recognition system using Convolutional Neural Networks (CNNs) to process human facial images, extracting and interpreting features for applications like identity verification and emotion classification.

****Dataset and Related Work****
The FER-2013 dataset, containing 35,887 grayscale images categorized into seven emotions, is used. Previous research has focused on ConvNets like VGG and ResNet to enhance emotion classification, using techniques such as transfer learning and data augmentation to address challenges like imbalanced data.

****Methodology****

**Initial Model**
A sequential CNN architecture achieved a test accuracy of 56% but showed overfitting.

**Advanced Architectures**
To improve generalization, VGG and MobileNet were implemented:

VGG: Uses small convolution kernels to capture complex features, achieving 86% accuracy.
MobileNet: Designed for efficiency with depth-wise separable convolutions, achieving 85% accuracy.

****Experimental Setup****
The FER-2013 dataset is preprocessed, and two CNN models (VGG and MobileNet) are trained using the Adam optimizer on categorical cross-entropy loss. An 80:10:10 split is maintained for training, validation, and test sets. Models are evaluated based on accuracy, precision, recall, F1-score, and inference time.

****Results and Comparison****

Sequential CNN Model : Showed significant overfitting with training accuracy reaching 80% but validation accuracy stalling at 60%.
MobileNet : Demonstrated better balance, performing well in recognizing 'happy' emotions but struggling with 'neutral'.
VGG : Excelled with high accuracy (85-86%) for both training and validation, indicating good generalization and minimal overfitting.

****Conclusion****
VGG: The most reliable model, suitable for precise emotion recognition.
MobileNet: Balances efficiency and performance, with room for improvement in generalization.
Sequential CNN: Needs optimization to address overfitting issues.
