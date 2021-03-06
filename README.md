# TransRank
[CVPR2022 Oral] The official code for "[TransRank: Self-supervised Video Representation Learning via Ranking-based Transformation Recognition](https://arxiv.org/abs/2205.02028)"

Since I'm busy with some new projects now, I may not be able to release a clean implementation with sufficient guidance right now. But I promise to do it **in late 2022**. 

Besides, if you are interested to check our implementation now, you can refer to the [`selfsup` branch of my mmaction2 fork](https://github.com/kennymckormick/mmaction2/tree/selfsup). It includes all the implementation of this paper, but may be a little bit messy. I also provide an example config: [transrank_ucf_r3d_rotate_mlp_200e.py](https://github.com/kennymckormick/mmaction2/blob/selfsup/configs/transrank_ucf_r3d_rotate_mlp_200e.py), which trains TransRank with 3 temporal transformations and 1 spatial transformation. Once you have cloned the repo and switched to the `selfsup` branch, you can run training with following command (8 GPUs):

```bash
bash tools/dist_train.sh configs/transrank_ucf_r3d_rotate_mlp_200e.py 8
```

Also, please send me an email to me or open a new issue under this repo if you have any questions regarding to the implementation. My email is dhd.efz@gmail.com. 
