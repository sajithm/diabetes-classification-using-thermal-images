# Diabetes Classification Using Thermal Images

## Dataset
Courtesy, Ms. Sudha BG

## Experiment
We are using the High Contrast images for this experiment. All images were resized to 320x240 IN RGB color. From each category, 10 images were used as validation set, the remaining were used for training. This meant we had 77 non diabetic images and 83 diabetic images available to use in training.

## Code
 + acgan_hc -> trains an Auxiliary Classifier GAN and generated 256 images of each type. 
 + cnn_hc_o -> trains a CNN network from scratch using the original dataset (77 and 83 images)
 + cnn_hc_g -> trains a CNN network from scratch using the synthetic dataset generated by AC-GAN (256 and 256 images)
 + cnn_hc_og -> trains a CNN network from scratch using a combination of original dataset augmented using the synthetic dataset generated by AC-GAN (77+83 and 83+77 images)
