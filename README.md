# dronenodrone
## Inspiration
The proliferation of cheap, consumer-oriented drones has become a common feature of the modern battlefield, posing a new risk to American troops. Detecting and classifying drones in real-time provides enhanced situational awareness, enabling military forces to identify potential threats promptly and take appropriate action to mitigate them. By distinguishing between friendly, hostile, and civilian drones, such a system enhances operational effectiveness, reduces the risk of friendly fire incidents, and safeguards both military personnel and civilian populations. 
## What it does
Different types of drones use specific radio frequency bands and transmission schemes. As such our model, by leveraging machine learning algorithms trained on labeled datasets containing samples of various drone radio signals, is capable of interpreting a drone’s radio signals as a fingerprint identifying its type. 
## How we built it
To build our model, we made use of feature extraction, which is a machine-learning technique that allows us to extract the most important features of a drone’s radio signal for identification. After extracting relevant features from the radio signals using feature detection techniques, we fed the output into a Convolutional Neural Network for further processing and classification. We sourced data for this project from a dataset that was published by an academic research team in Switzerland, and we trained the model using compute rented through Google Colab.
## Challenges we ran into
Prior to this project, we were unfamiliar with signal processing and working with radio signals, which meant we had to spend some time learning how to work with them. Another challenge that we faced was that we originally were attempting to implement a complex-valued neural network but the machine learning architecture of Tensorflow and Pytorch do not yet support such technology.
## Accomplishments that we’re proud of
Our model is able to predict enemy drones within roughly **90%**. Furthermore, our model is able to detect drones and classify their make and model with an accuracy of about 50%. As such, our model could be used to help warfighters to quickly understand the nature of a potential aerial threat. 
What we learned
During this project, we learned much about signal processing / interpreting radio frequencies. We also gained more experience with implementing AI systems.
What’s next for Drone or No Drone
There are several potential extensions for this project. The first of which would be to gather more data on the radio frequencies emitted by drones as they fly and to give our model more time and computing to train with, thus creating a model with a greater level of accuracy. Another plan would be to expand the model to also take input from cameras and other sensors in order to further improve accuracy. Lastly, combining our model with a weapons system to shoot down drones would allow soldiers to respond more quickly to threatening situations

