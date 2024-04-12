# EECS_6322
This is the official repo for EECS 6322 Reproducibility project

Original Paper: https://arxiv.org/abs/2104.09367


Hello. The main github contains all of the important (and small!!!) files that are, in essence, required for this project to run. Below, we will be giving the link to the datasets that were used (since that is waaay too big for a Github repo) and also the generated log files (if you wish to check them out).

dataset: https://drive.google.com/drive/folders/14J6yuXtvITT_EdpM428a85Foe1cgR05a?usp=sharing

logs: https://drive.google.com/drive/folders/1Mb67NPVjouZMGKNKqadIzD9DfsWaPBNb?usp=drive_link

# What to do if you wish to run this.

Soo.., the main code files are in the notebook. You might need to modify certain filepaths e.g where you are going to store the dataset and what not. For our project, we stored the datasets within the root folder (which in our case was a Google Drive folder, so you might have to change that part). Make sure that the DCNv2 is in the root folder as well.

There are 6 main notebooks:

1. EECS_6322_Project --> This is the notebook where we implemented the network proposed in the paper, (ITS + SOTS) 

2. EECS_6322_Project_DH+NH --> This is the notebook where we implemented the network with the NH and DH datasets

3. [Ablation_1_Final]_of_EECS_6322_Project_BASE_Model --> This is where we performed the first Ablation Study, where the trained network was simply the upsampling and downsampling layer with no Contrastive Regularization (base network).

4. [Ablation_2_Final]_of_EECS_6322_Project_BASE_Model + Mixup --> This is where we performed the second Ablation Study, where we added the adaptive mixup layer to the base network

5. [Ablation_3_Final]_of_EECS_6322_Project_BASE_Model + DFE --> This is where we performed the third Ablation Study, where we added the DFE modules to the base network

6. [Ablation_4_Final]_of_EECS_6322_Project_BASE_Model + DFE + Mixup --> This network is similar to the one in the first notebook, where we combined the base network with the mixup and DFE modules, except without the Contrastive Regularization


To run these notebooks, simply run the cells in order (after modifying the directory paths). One weird thing that we found while running is that you should run the dataloader cells twice. If you run them once, there seems to be some sort of error
