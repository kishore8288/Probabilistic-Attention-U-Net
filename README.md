# Probabilistic-Attention-U-Net
Propsed method for efficient segmentation of MR brain tumor images.

We used 
**finetuned Efficient Net-B4** as an encoder.\
**Dual Inception Resnet** which bridges between encoderand decoder.\
**Single stage Decoder** duplicated this layer in each upsampling.\
**VAE upsampled features** and **Residuals** with **Decoder Outputs** are added with weight combinations.\
A final **Window based self attention transformer** is used. \

This technique resulted in the recall of 93% with precision 89%.
