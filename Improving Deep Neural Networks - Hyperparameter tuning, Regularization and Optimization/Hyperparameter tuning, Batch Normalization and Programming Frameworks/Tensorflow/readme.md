## Tensorflow


Course 2 , Week 4   [Coursera](https://www.deeplearning.ai/)

Instructor: Andrew Wg



Welcome to the Tensorflow Tutorial! In this notebook you will learn all the basics of Tensorflow. You will implement useful functions and draw the parallel with what you did using Numpy. You will understand what Tensors and operations are, as well as how to execute them in a computation graph.

After completing this assignment you will also be able to implement your own deep learning models using Tensorflow. In fact, using our brand new SIGNS dataset, you will build a deep neural network model to recognize numbers from 0 to 5 in sign language with a pretty impressive accuracy.



![](images/demo.jpg)





one_hot_matrix = tf.one_hot(indices = labels, depth = C, axis = 0)

另一种：

def convert_to_one_hot(Y, C):
    Y = np.eye(C)[Y.reshape(-1)].T
    return Y

X_train_flatten = X_train_orig.reshape(X_train_orig.shape[0], -1).T

multi-class输出用softmax而不是sigmoid

X = tf.placeholder(tf.float32, [n_x, None], name="X")

tf.set_random_seed(1)                   # so that your "random" numbers match ours
        
    ### START CODE HERE ### (approx. 6 lines of code)

    W1 = tf.get_variable("W1", [25,12288], initializer = tf.contrib.layers.xavier_initializer(seed = 1))

It is important to know that the "logits" and "labels" inputs of tf.nn.softmax_cross_entropy_with_logits are expected to be of shape (number of examples, num_classes). We have thus transposed Z3 and Y for you.

看random_mini_batches（）的实现

看预处理自己image的方法