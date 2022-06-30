# Image_Coloring_using_CGAN

In this project I have used conditional GAN to implement image colorization as proposed in Pix2Pix paper. During training, the input RGB image is converted into LGB space and the L channel acts like the grey image input to the generator. The generator then produces the A and B channels which when concatenated with the original L channel are sent to the patch discriminator. The patch discriminator outputs a score for each patch, telling whether it's real or not and thus hepls the generator to learn.

## Outputs
### After 20 epochs
![20220626_102644](https://user-images.githubusercontent.com/84125572/175800742-3d9a3db8-4c7b-4b60-b6b2-893f1807fbec.jpg)
### After 40 epochs
![Screenshot_20220626-110825_Adobe Scan](https://user-images.githubusercontent.com/84125572/175801099-241dabd8-11bc-424d-8315-4cbd1ae3af09.jpg)
### After 50 epochs
