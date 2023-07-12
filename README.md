# DCSS
Code to run:
Open the run.ipynb file in google colab and be careful to check the directory：%cd /content/DCSS/Codes

You can change the parameters and dataset of the train.py file:

AE: The autoencoder model.  
MNet: The mutual information estimation network.  
data_loader: The data loader for accessing the dataset.  
dataset_size: The total size of the dataset.  
batch_size: The batch size used during training. Default is 500.  
pretraining_epoch: The number of epochs for autoencoder pretraining. Default is 200.  
MaxIter1: The maximum number of iterations for the first phase of DCSS. Default is 200.  
MaxIter2: The maximum number of iterations for the second phase of DCSS. Default is 20.  
num_cluster: The number of clusters. Default is 10.  
m: The fuzziness parameter for cluster membership calculation. Default is 1.5.  
T1: The interval for updating cluster centers during the first phase. Default is 2.  
T2: The interval for updating cluster membership during the second phase. Default is 5.  
latent_size: The size of the latent space in the autoencoder. Default is 10.  
zeta: The threshold for determining when to update cluster centers during the second phase. Default is 0.8.  
gamma: The threshold for determining when to update cluster membership during the second phase. Default is 0.2.  
dataset_name: The name of the dataset. Default is 'MNIST'.  

For example, this run sets MaxIter1 to 150.


PyTorch implementation of DCSS: Deep Clustering with Self-supervision using Pairwise Data Similarities

<center><img src="https://github.com/Armanfard-Lab/DCSS/blob/main/Figures/final_model-1.png" alt="Overview" width="800" align="center"></center>

Note that you should have CUDA installed for running the code.

## Citation

You can find the preprint of our paper on [TechRrxiv](https://www.techrxiv.org/articles/preprint/Deep_Clustering_with_Self-supervision_using_Pairwise_Data_Similarities/14852652/1).

Please cite our paper if you intend to use our code or results.
```
@article{Mohammadreza2021deepclustering,
  title={Deep Clustering with Self-supervision using Pairwise Data Similarities},
  author={M. Sadeghi, and N. Armanfard},
  journal={TechRxiv preprint DOI: https://doi.org/10.36227/techrxiv.14852652.v1},
  year={2021}
}
```
