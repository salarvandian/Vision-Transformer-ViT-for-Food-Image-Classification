# Vision-Transformer-ViT-for-Food-Image-Classification
This project demonstrates the use of a Vision Transformer (ViT) model for classifying Indian food images. The ViT model is fine-tuned on a custom dataset to classify images into various food categories. The implementation leverages the Hugging Face transformers library and includes preprocessing, training, and evaluation steps.

# Vision Transformer (ViT) for Food Image Classification

## Overview
This project uses a Vision Transformer (ViT) model to classify Indian food images into predefined categories. The model is fine-tuned on a custom dataset (`rajistics/indian_food_images`) using the Hugging Face `transformers` library. The implementation includes data preprocessing, model training, and evaluation with accuracy metrics.

## Dataset
The dataset used in this project is `rajistics/indian_food_images`, which contains labeled images of various Indian food items. Each image is associated with a label representing its food category.

## Key Steps
1. **Data Loading**: Load the dataset using the `datasets` library.
2. **Preprocessing**:
   - Map labels to IDs and vice versa.
   - Apply transformations such as resizing, normalization, and tensor conversion.
3. **Model Fine-Tuning**:
   - Use the pre-trained `google/vit-base-patch16-224-in21k` model.
   - Fine-tune the model on the custom dataset.
4. **Evaluation**: Compute accuracy metrics during training and validation.
5. **Saving the Model**: Save the fine-tuned model for future use.

## Dependencies
To run this project, you need the following libraries:
- `datasets`: For loading and managing datasets.
- `evaluate`: For computing evaluation metrics.
- `transformers`: For loading pre-trained models and tokenizers.
- `torch`: For tensor operations and GPU acceleration.

Install the required libraries using:
```bash
pip install datasets evaluate transformers torch torchvision
