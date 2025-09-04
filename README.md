# AnimeGANs
A few notebooks showing CycleGAN and UNet pix2pix approaches for anime sketches colorization + hf demo link

## ***Demo***
There is a Streamlit **[demo](https://huggingface.co/spaces/igor-saprygin/anime-sketch-color-gan)** on hf you can try yourself

![alt text](images/pix2pix.png)
![alt text](images/cycle.png)

## CycleGAN
Was initially implemented for Monet2Photo dataset for which the notebook is also uploaded. The approach implies an unpaired training, hence the generators do not know about the original pictures unlike pix2pix.
![alt text](images/image.png)
Interestingly, CycleGAN tends to use a cold violet/blue pallete on validation data. Maybe it got collapsed during training, though mid-training samples are diverse.

Rem: the first two are from val data, the last are from train
![alt text](images/image-1.png)
![alt text](images/image-2.png)
![alt text](images/image-3.png)
![alt text](images/image-4.png)

## Pix2pix (UNet)
The next approach leverages  given "answers" and uses UNet as the Generator. The result is apparently more diverse in colors though the general OOD quality of colorings seems lower than of those from CycleGAN. 
![alt text](images/image-5.png)
![alt text](images/image-6.png)
![alt text](images/image-7.png)

