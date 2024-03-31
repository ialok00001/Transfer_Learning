# Transfer Learning

This project is an attempt in learning the method of Transfer Learning, specifically in computer vision.

We have taken the ResNet18 pre-trained model and the CIFAR-10 dataset. Since ResNet18 is trained on 1000 classes, we had to remove its last layer and set its output layer dimension to 10, the number of labels in CIFAT-10. Then we trained this model, while freezing the entire model (except the last output layer), unfreezing its latter layers in stages and comparing its accuracies.

Transfer Learning is a great method in neural network training, where we use a pretrained model on one set of task, and then train that model, either completely or partially (not all layers) for another task and test its accuracy on this task. This method is a much faster way of learning, mostly in the cases when the pre-trained model task and the current task have high similarity.


All the foundation models are fine-tuned using transfer learning and its variants to achieve higher throughput on specific tasks.
