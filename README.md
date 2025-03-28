Multi-ConDoS ⚡ PyTorch Lightning ⚡

John Mark Alexis Marcelo - 1850518 

My notebook aims to implement Multi-ConDos in PyTorch Lightning ⚡, a novel approach for multimodal contrastive self-supervised medical image segmentation designed to address domain shift and multimodality challenges. It employs a novel strategy that combines CycleGAN and Pix2Pix to facilitate domain translation, essential for managing multimodal data. Additionally, it introduces domain sharing layers to capture both domain-specific and shared information across modalities.

SYSTEM USED: MacOS 14.2.1

INSTRUCTION:

1)INSTALL
!pip install torch torchvision torchaudio pytorch-lightning matplotlib numpy

2)OPEN MultiConDos_Light.ipynb

3)UNZIP DATA.zip and modify

     DATA_CONFIG with your desired path for train the DSGAN (one for t1ce and one for t2)
     
     DATA_CONFIG_FINE for the finetuning part (one for t1ce and one for the mask)
   
4)RUN ALL

5)FINAL RESULTS:
     
     We can see here on the first raw the loss of the DSGAN
     
     On the second row we see some mask generated by the finetuning
     
     In the last one we see the focal (for object detection) and binary dice loss (binary segmentation)

![Image 1](https://raw.githubusercontent.com/sanjohngiangino/MultiConDos/main/architecture.png)

6)The files mask_generated.zip and dsgan_pred_image.zip contain the final generated masks and the T1CE to T2 image transformations, respectively.
