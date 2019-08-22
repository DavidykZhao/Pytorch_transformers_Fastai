# Pytorch_transformers_Fastai
A small adjustment to fastai to use a pre-trained Pytorch_transformers model 

Pytorch-transformers is a comprehensive package consisting multiple SOTA NLP pretrained models. It was called pytorch-pretrained-bert. There were some good tutorials and blog posts explaining how to apply pytorch-pretrained-bert models to fastai API. 
However, after the update of pytorch-pretrained-bert models to Pytorch-transformers. There are some notable differences in its API as well. The most notable would be the output from the model now becomes a tuple rather than a single output. This small change has broken all of the codes from the past tutorials and blog posts.
The solution is to adjust the script in fastai to accomodate this change and the specific change happens at loss_batch function in basic_train.py 
See the script for more details...
Please let me know if you experience any exceptions. 
