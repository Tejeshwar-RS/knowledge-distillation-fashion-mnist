# knowledge-distillation-fashion-mnist
This project demonstrates the concept of knowledge distillation, a technique used in machine learning to transfer knowledge from a large, high-performing model (teacher) to a smaller, more efficient model (student). The project uses the Fashion-MNIST dataset, which consists of a dataset of Zalando's article images.

## Project Overview
- **Training the Teacher Model:**  A high-performance convolutional neural network is trained on the Fashion-MNIST dataset to achieve high accuracy. This model serves as the knowledge source.
- **Training the Baseline Student Model:**  A smaller, lightweight student model is trained from scratch on the same dataset for comparison. This model serves as the performance baseline.
- **Training the Distilled Student Model:** The student model is trained again, but this time it is guided by the teacher model's outputs (soft labels) in addition to the standard hard labels. This process allows the student model to learn not just the correct class, but also the nuances of the teacher's predictions.
- **Performance Analysis** The project concludes with a detailed comparison of the three models' performance metrics.

## How to Run
1. Ensure you have all the required libraries installed. You can install them using the provided requirements.txt file.
     pip install -r requirements.txt
2. Run the Jupyter Notebook Knowledge-Distillation.ipynb in a compatible environment like Google Colab or a local Jupyter server.
3. The notebook will automatically download the dataset, train the models, and display the results and visualization.
4. The final output includes a Gradio interface for a real-time demo.
