# Image_Coloring_using_CGAN
Image-Coloring
In this project I have used conditional GAN to implement image colorization as proposed in Pix2Pix paper. During training, the input RGB image is converted into LGB space and the L channel acts like the grey image input to the generator. The generator then produces the A and B channels which when concatenated with the original L channel are sent to the patch discriminator. The patch discriminator outputs a score for each patch, telling whether it's real or not and thus hepls the generator to learn.
