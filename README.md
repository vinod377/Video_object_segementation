# Video_object_segementation
### Video Object Segmentation using One short Deep Learning. The Repository is implementation of the paper[](). OSVS is a CNN architecture to tackle the problem of semi-supervised video object segmentation, It basically consist of two stages. 
- Parent network training: Which produces a rough forground/Backround segmentation
- Fine tunning: The trained model is finetuned for specfic object/mask_ground truth pair for n number of epoch on sigle or few initial  frames of Video.(Hence called One shot learning).
For evaluation, region of similarity in terms of intersection over union is used. After finetunning with first single frame, the mean intersection over union for all subsequent frames in a sequence is around 60%.The average inference time for single frame on intel core i-7 processor is 1.5 second.

- Parent Model is trained on DAVIS2017 dataset and sequence of cow, dog and kite-walk are kept for evaluation and testing. The trained parent model and some fine tunned model on first frame/mask pair of test sequence is provided in model folder. Few output results are:

![cow](https://github.com/vinod377/Video_object_segementation/blob/master/output__test_data_finetuned_model/cow_mask_00013.jpg)
![dog](https://github.com/vinod377/Video_object_segementation/blob/master/output__test_data_finetuned_model/dog__mask_00008.jpg)
![kite-walk](https://github.com/vinod377/Video_object_segementation/blob/master/output__test_data_finetuned_model/kite_walk_mask_00011.jpg)
## Dependencies
- Python-3.9
- Tensorflow-2.6
- Opencv-4.5
- Numpy

## References
<a id="1">[1]</a> 
Sergi Caelles, Kevis-Kokitsi Maninis, Jordi Pont-Tuset, Laura Leal-Taixé, Daniel Cremers, Luc Van Gool. 
One-Shot Video Object Segmentation. 
In CVPR 2015.

<a id="2">[2]</a>
Kevis-Kokitsi Maninis, Jordi Pont-Tuset, Pablo Arbelaez, and Luc Van Gool.
Deep retinal image understanding. 
In MICCAI, 2016.



