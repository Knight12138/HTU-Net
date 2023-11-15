# HTU-Net
[IJCB 2022]Implementation of Towards More Accurate And Complete Iris Segmentation Using Hybrid Transformer U-Net

We are busy with some things recently. The code will be uploaded as soon as we finish sorting it out. Thank you for your patience and attention to this work.

[Update 23.11.15]
Link：https://pan.baidu.com/s/188gfnq7BwBDjK9lHOmCuBg?pwd=ln38 
Code：ln38

Anyone interested can download our project via above link. Forgive us for not having enough time to maintain this project. We will update a Google Drive link for project downloads later. 

If you find any implementation problems in the code, you can contact me through this email (sunye20@mails.jlu.edu.cn). 

You can follow the description below to try to reproduce our project (single 1080Ti is enough for reproduce). 

#1. Our project is based on TensorFlow-GPU 2.0, 2.2 or 2.4 can also run normally. Some common packages, such as numpy, OpenCV, keras, scipy, etc. also need to be installed.

#2. We first process the data into tfrecords format to speed up model training. You can generate your own data through DataProcess.py or use the files we provide.

#3. All files can be simply loaded into Pycharm for easy operation. You can design your own model by modifying HTU_Net.py and run train_net.py to train (Note: Our model training uses multiple outputs, additional output (output named 'spa_0' in HTU_Net.py) need to be omitted during model inference).

#4. Before model inference, you need to modify the weight file path under the ckpt folder to ensure that the weights are loaded normally.

#5. Run post_process.py to get the final result.

#6. You can refer to the IrisParseNet(https://github.com/xiamenwcy/IrisParseNet) to evaluate the results.

