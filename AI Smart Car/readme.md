# Self Driving Car AI using Kivy and PyTorch/Keras

I designed a car using Kivy framework used 3 sensors in the car to perceive the enviornment.
Then I trained the car using Reinforcement Learning(Deep Q Network)

## Requirements

* [Kivy](https://kivy.org/#home)
Kivy is an Open source Python library for rapid development of applications that make use of innovative user interfaces, such as multi-touch apps.

* [PyTorch](https://pytorch.org/)
PyTorch is an open source machine learning library based on the Torch library, used for applications such as computer vision and natural language processing, primarily developed by Facebook's AI Research lab.

OR

* [Keras](https://keras.io/)
Keras is an open-source neural-network library written in Python. It is capable of running on top of TensorFlow, Microsoft Cognitive Toolkit, R, Theano, or PlaidML. Designed to enable fast experimentation with deep neural networks, it focuses on being user-friendly, modular, and extensible.

* Some Python libraries such as Numpy and Matplotlib.

# To Run Self Driving Car:
- Run below command, to start an emulated environment where you can see a toy car (Do ensure that the enviornment is set up)
- Use your mouse, left click and drag, to drop sands
- With mouse now you can create your own road/sand ways, where the car will learn to drive on its own.
- Go ahead and create different paths and see how it adopts to the environment 
- I implemented this project using both PyTorch and Keras to implement Deep Learning based Q Learning, a special Reinforcement Learning algorirthm that learns the environment and helps the agent(car) to navigate avoiding the sand
(By default ai used is based on PyTorch, if you are using Keras then change line19 to - "from ai_keras import Dqn")

```
python map.py
```

## Description

We need an environment to emulate our car and sensors with our own rules. Kivy is a Python UI development framework, which can be used for this purpose, as it allows user interaction programming very easy, like mouse / touch interactions.
I used Kivy to make the car environment .

Then I used Experience Replay and Deep Q intuition to create an AI which uses 3 sensors(front, left & right) in the car to detect 'sand(yellow)' i.e. out of it's road areas . If it runs on the sand it gets punishment/penalized and it tries not to repeat that again.

I used a deep neural network comprising of two hidden layers. First layer having 30 nodes and Second layer having 20 nodes.

## Reference

* https://medium.com/@mageswaran1989/self-driving-car-with-deep-learning-8eb2c418acb6
