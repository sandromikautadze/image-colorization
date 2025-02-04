# Image Colorization With Deep Learning

**Authors**: Diego Cerretti, Beatrice Citterio, Mattia Martino, Sandro Mikautadze

**Web App**: https://imagecolorizationwithdeeplearning.streamlit.app/

# Abstract 
In this work, we assess the performance of various deep learning architectures to colorize grayscale images, using the MS COCO dataset. We train three main models: a convolutional neural network (CNN), a U-Net, and a generative adversarial network (GAN). For the CNN and U-Net, we use three loss functions to understand their impact on the colorization properties. We evaluate the models' performances using mean squared error (MSE), peak signal-to-noise ratio (PSNR), structural similarity index measure (SSIM), and Fréchet inception distance (FID) score. The results indicate that CNNs struggle to capture the color structure of images, whereas U-Nets achieve significantly better colorization across all evaluation metrics. GANs, although challenging to train, demonstrate comparable performance to U-Nets and show potential for improvement with additional tuning. 

# Repo Structure

- **losses/**: Contains the loss values of the trained models.
- **models/**: Contains the weights of the trained models, including weights at various epochs during training.
- **outputs/**, **test_images/**, **report_images/**: Contain the black-and-white test images used for evaluation, colorized images and plots used in the report.
- **utils/**: Contains a library with functions and classes used in the code, including:
  - **dataset.py**: Functions related to data loading and preprocessing.
  - **metrics.py**: Functions to compute evaluation metrics.
  - **models.py**: Definitions of the CNN, U-Net, and GAN architectures.
  - **plots.py**: Functions for plotting results.
  - **training.py**: Functions related to the training process.
- **report.pdf**: Report of our project.
- **vm_cnn.ipynb**: Code used to train the final CNN models on the virtual machine.
- **vm_unet.ipynb**: Code used to train the final U-Net models on the virtual machine.
- **vm_gan.ipynb**: Code used to train the final GAN model on the virtual machine.
- **vm_gan_local.ipynb**: Code used to train the final GAN model on a local machine (since it failed on the VM).
- **baseline.ipynb**: Contains code for baseline models and experiments.
- **cnn.ipynb**: Contains code for initial CNN models and experiments.
- **unet.ipynb**: Contains code for initial U-Net models and experiments.
- **gan.ipynb**: Contains code for initial GAN models and experiments.
- **report_plots.ipynb**: Code to generate the plots used in the report.
- **tests.ipynb**: Code to generate colorized images from test inputs.