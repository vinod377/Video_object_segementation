# Video_object_segementation
### Video Object Segmentation using One short Deep Learning. The Repository is implementation of the paper[](). OSVS is a CNN architecture to tackle the problem of semi-supervised video object segmentation, It basically consist of two stages. 
- Parent network training: Which produces a rough forground/Backround segmentation
- Fine tunning: The trained model is finetuned for specfic object/mask_ground truth pair for n number of epoch on sigle or few initial  frames of Video.(Hence called One shot learning).
For evaluation, region of similarity in terms of intersection over union is used. After finetunning with first single frame, the mean intersection over union for all subsequent frames in a sequence is around 70%.The average inference time for single frame on intel core i-7 processor is 1 second.

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



