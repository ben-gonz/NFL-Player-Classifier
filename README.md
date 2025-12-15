# NFL Player Image Classifier

This repository contains a Jupyter Notebook script for building and training an image classifier using a fine-tuned Vision Transformer (ViT) model from Hugging Face. The classifier distinguishes between images of specific NFL players by scraping training images from Bing, preprocessing them, and training on a small dataset. It supports validation on held-out data and inference on new test images.

## Features
- **Image Scraping**: Automatically downloads images for user-specified search terms (e.g., player names) from Bing.
- **Dataset Preparation**: Organizes images into folders, splits into train/validation sets, and uses `ImageFolder` for loading.
- **Model**: Fine-tunes `google/vit-base-patch16-224-in21k` for multi-class classification.
- **Training**: Uses PyTorch Lightning for efficient training with mixed precision on CPU.
- **Evaluation**: Computes predictions on validation batches and new test images, with accuracy metrics and visualizations.
- **Example Terms**: Pre-configured for NFL players like Justin Herbert, Christian McCaffrey, Jason Myers, Nico Collins, and Devin Neal (all stars in my fantasy lineup this year with a top 3 league performance).

This model can be trained on any other test image set (e.g. dog breeds, plants, animals, materials, etc.)
