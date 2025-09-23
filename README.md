# knowledge-distillation-fashion-mnist
This project is a practical implementation of knowledge distillation, a model compression technique, completed for a hackathon. A large "teacher" model (ResNet18) is trained on the Fashion-MNIST dataset, and its knowledge is then distilled into a smaller, more efficient "student" CNN. The goal is to create a lightweight model with minimal loss in accuracy.

## Key Features
- **Teacher Model:** A ResNet18 architecture adapted and trained for Fashion-MNIST.
- **Student Model:** A lightweight, custom-built CNN with significantly fewer parameters.
- **Distillation:** Implemented using soft labels and KL Divergence loss to transfer knowledge from the teacher's output probabilities.
- **Evaluation:** The final models are compared based on accuracy, model size (parameter count), and inference speed.


## Technologies Used
- Python
- PyTorch
- NumPy
- Matplotlib
- Google Colab (for GPU-accelerated training)
