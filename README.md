﻿

# TensorflowFaceDetect

docker run -it -v /c/Users/nirav/Desktop/svsapp:/tf_files/ gcr.io/tensorflow/tensorflow:latest-devel


 python NiravImg.py Ntest.jpg
 python /tensorflow/tensorflow/examples/image_retraining/retrain.py --bottleneck_dir=/tf_files/bottlenecks --how_many_training_steps 500 --model_dir=/tf_files/inception --output_graph=/tf_files/retrain_graph.pb --output_labels=/tf_files/retrain_labels.txt --image_dir=/tf_files/office
 
 python retrain.py \
--bottleneck_dir=/tf_files/bottlenecks \
--how_many_training_steps 500 \
--model_dir=/tf_files/inception \
--output_graph=/tf_files/retrain_graph.pb \
--output_labels=/tf_files/retrain_labels.txt \
--image_dir=/tf_files/office



root@109a6912371d:/tf_files# python NiravImg.py Ntest.jpg
W tensorflow/core/framework/op_def_util.cc:332] Op BatchNormWithGlobalNormalization is deprecated. It will cease to work in GraphDef version 9. Use tf.nn.batch_normalization().
nirav (score=0.68884)
kumar (score=0.19092)
jass (score=0.12024)

root@109a6912371d:/tf_files# python NiravImg.py JTest.jpg
W tensorflow/core/framework/op_def_util.cc:332] Op BatchNormWithGlobalNormalization is deprecated. It will cease to work in GraphDef version 9. Use tf.nn.batch_normalization().
jass (score=0.63106)
kumar (score=0.28253)
nirav (score=0.08641)

root@109a6912371d:/tf_files# treed
bash: treed: command not found
root@109a6912371d:/tf_files# tree
bash: tree: command not found
root@109a6912371d:/tf_files# ls
JTest.jpg  NiravImg.py  Ntest.jpg  Thumbs.db  bottlenecks  inception  office  retrain_graph.pb  retrain_labels.txt
root@109a6912371d:/tf_files# python /tensorflow/tensorflow/examples/image_retraining/retrain.py --bottleneck_dir=/tf_files/bottlenecks --how_many_training_steps 500 --model_dir=/tf_files/inception --output_graph=/tf_files/retrain_graph.pb --output_labels=/tf_files/retrain_labels.txt --image_dir=/tf_files/office


