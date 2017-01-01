---
layout: default
---

# A concise dive into Tensorflow

### General
* Tensorflow is an open-sourced machine learning library released by Google in November, 2015
* It can be used for any gradient-based methods
* The word 'tensor' means 'n dimensional array'

### Programming
* import tensorflow as tf  is used to import the tensorflow library into python
* Variables are declared as follows:
{% highlight python %}
W = tf.Variable(tf.random_uniform([1], -1.0, 1.0))
b = tf.Variable(tf.zeros([1]))
{% endhighlight %}
* Placehoders are like declaring variables but you don't need to assign it an actual value. Used for input/output (thing that stay fixed during the training)
{% highlight python %}
x = tf.placeholder(tf.float32, shape=[None, 784])
y_ = tf.placeholder(tf.float32, shape=[None, 10])
{% endhighlight %}

### Exercise 1:
* This [link](https://www.tensorflow.org/tutorials/mnist/pros/) is an essential starting point

### Exercise 2:
Next I will apply Tensorflow to my own project, in this case ...