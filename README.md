# Full Resolution Image Compression

In this repostiroy is a recreation of the architecture of the 2016 Google [paper](https://arxiv.org/pdf/1608.05148.pdf) by the same name. 

There are a few modifications:
- The loss function was changed to SSIM instead of the residual loss.
- Due to hardware constraints on my end, the number of iterations in the implementation of the model was reduced to 1, from 16


### General Conclusion

Overall, the SSIM loss performs fairly well, and with more data and hardware I believe that it could perform just as well as the residual loss in the original paper.

#### TODO:

1. Implement GRU based version using custom models in Tensorflow. This is a the LSTM implementation
2. Image generator to slowly feed more data into the model
