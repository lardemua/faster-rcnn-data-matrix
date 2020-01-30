# faster-cnn-data-matrix
This work presents an implementation of a Faster R-CNN model to detect Data Matrix. This architecture demonstrated quite accurate and consistent results by detecting the landmarks in almost all frames.

The  Faster  R-CNN  was  trained  through  [Detectron2](https://github.com/tmralmeida/detectron2),  a  research  platform  for  object  detection  and  segmentation.
This approach achieves an AP@0.5 of 89% on our test set. If you want our dataset please contact me. 
Moreover, it can detect Data Matrix in the full set of the test set, while classical techniques based on the libdmtx library only achieved 45%. Finally, in terms of running time speed these classical algorithms processing in one CPU are 40 times slower (at minimum) than the model that I present here running in one Nvidia RTX2080ti for the same set of frames.

If you find this implementation or the analysis conducted in our report helpful, please consider citing:

(Sumitted paper) - Updating

Or the Detetcton 2 platform:

```
@misc{wu2019detectron2,
  author =       {Yuxin Wu and Alexander Kirillov and Francisco Massa and
                  Wan-Yen Lo and Ross Girshick},
  title =        {Detectron2},
  howpublished = {\url{https://github.com/facebookresearch/detectron2}},
  year =         {2019}
}
```

For convenience, here is the faster RCNN citation:

```
@inproceedings{renNIPS15fasterrcnn,
    Author = {Shaoqing Ren and Kaiming He and Ross Girshick and Jian Sun},
    Title = {Faster {R-CNN}: Towards Real-Time Object Detection
             with Region Proposal Networks},
    Booktitle = {Advances in Neural Information Processing Systems ({NIPS})},
    Year = {2015}
}
```
