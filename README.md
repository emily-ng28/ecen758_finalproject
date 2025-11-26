# CNN vs ResNet18 on STL-10 — Deep Learning Image Classification

Our project compares the performance of a custom Convolutional Neural Network (CNN) and a fine-tuned ResNet18 model on the STL-10 dataset.

### **Dataset**
- **STL-10** (train: 5,000 labeled images, test: 8,000 images)
- 10 classes: airplane, bird, car, cat, deer, dog, horse, monkey, ship, truck

### **Model Selection**
- **Basic CNN**
- **ResNet18** (pretrained on ImageNet + fine-tuned)

## **Training Setup**
- Optimizer: Adam with Cosine Annealing Learning Rate scheduler 
- Loss: Cross-Entropy with label smoothing of 0.1
- CNN: learning rate = 1e-3, weight decay = 1e-3, epcohs = 50
- ResNet18: learning rate = 1e-4, weight decay = 1e-3, epochs = 20 
- Batch size: 128
- Augmentations: random crop, horizontal flip, random erasing, random augmentations
