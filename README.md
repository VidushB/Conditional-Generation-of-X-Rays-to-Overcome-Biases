# Conditional-Generation-of-X-Rays-to-Overcome-Biases

In this project, we attempt to overcome the problem of biased datasets in medical imaging through the conditional generation of X-Ray images. We evaluate our approach by comparting the performance of a Case-Based Reasoning classifier (CBR) when trained on the original CheXpert dataset and then on the augmented dataset that is augmented with synthetic images generated by our conditional generative adversarial network (cGAN).

# Dataset
The CheXpert dataset is readily available on [their git](https://stanfordmlgroup.github.io/competitions/chexpert/). To access the dataset, you must fill up their form with your name, email adress, affiliation and role along with your phone number. Upon doing so, you should get an email with the option to download one of two datasets: the ```11 GB``` version or the ```436 GB``` version. For our project we will use the smaller dataset. The dataset is downloaded as a ```.zip``` file. Using our code Dataset_Preparation, you will be able to unzip the dataset and create tensors and panda dataframes to train models on.

# Models
We train a cGAN and a ResNet Model with skip connections for this project. Both these models are available under our Models function.

# Training
We also define our training function for our cGAN and our ResNet model that we used to produce results
