Some notes relating to implementation of my hotdog/not hotdog classifier 

## Architecture of network 

## How was it trained




## Optimizers used and comparison 

## Data augmentation 

## Batch normalization 

## Transfer learning 
Transfer learning refers to the process of taking one network that has been trained on a task A, to use it for another task B. We want to make use of the fact that the network has been often extensively trained with a lot of different data, and we think it will generalize well to our current task. We take all the weights and biases of the pretrained network, then change the last layer, so it ouputs something different than the original ResNet. 
It is called freezing the network, meaning we don't change any weights and biases, we just take it as such, only do forward pass on it. 
We believe that the frozen network will work well at feature extraction. 

For ResNet that we use, there are 512 features coming into last layer, and it outputs 1000 different classes. We replace this last layer, it still takes 512 features but now produces 2 outputs. This 

