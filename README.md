# Image-Denoiser
This is a Project I made as a final week submission for the CSOC camp conducted by my university IIT-Varanasi. In this project I leverage the concept of Autoencoders(took motivation) in order to denoise images document PHOTOS. The notebook attach contains three models all of which made using the Sequential API of tensorflow keras. 

### Link to Project Drive - [Drive](https://drive.google.com/drive/u/3/folders/1zFM-DcUZPHcVVuA-JoL29p20Pu3nHHFG)
This Drive contains the notebook and the presentation report for the project.

Autoencoders :
![image](https://github.com/GARV-k/Image-Denoiser/assets/117428410/5cce2ba8-cfd7-4ffa-8502-b4ed8b532cb9)
The image shown above is that of a Autoencoder Neural network. Like tradiional CNN's the Encoder part of Autoencoder aims at import feature extraction. But unlike traditional CNN's it doesn't terminate into fully connect layers from which classification is concluded. Rather in place of Fully connected layers a Decoder network is attached (Consisting of Upsampling layers(in case of third model) or transpose Convolutional layers(in case of my first and second model)) reconstructs the image back. Usually in autoencoders the X_train and y_train are the same dataset as its recosntructing the images itself. As a beginner I see no potential use of just reconstructing the image back. But the motivation is explained below.

Motivation : 
Rather than y_train being the same dataset of images as the X_train, y_train contains the corresponding clear images. In this way a tweek is made to the tradional Autoencoder network to denoise images.

(Notebook also contains the loss functions, feature maps and some sample filters.)
