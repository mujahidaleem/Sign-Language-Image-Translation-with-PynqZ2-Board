# Sign-Language-Image-Translation-with-PynqZ2-Board
Worked on the machine learning environment, training parameters/data-set manipulation, setting up the PYNQz2 board.

Inspiration
We wanted to learn more about Machine Learning. We thought of sign language translation after hearing the other theme was connectivity, even though that meant the technology more than the word itself.

What it does
The board interfaces with a webcam, where it takes a picture. The picture is then processed into a gray-scale image, and then centered around the hand. After using the Binary Neural Network (and the weights generated from our machine learning training) the image is judged and then outputs a string saying what the hand sign is.

How we built it
We found a MNIST type sign language data set on Kaggle. Using Pynq's library and CUDA we trained our own neural network on one of our personal laptops. This generated weights to be implemented on PynqZ2 with their Binary Neural Network Overlay. We then used their example scripts as a foundation for our own scripts for taking pictures and processing images.

Challenges we ran into
Some of the challenges we faced were mostly centered around creating the machine learning environment that generated the weights used to judge the images taken by the webcam. A lot of libraries that we had to use (ie Theano) were often outdated, causing us to downgrade/reinstall many times to get the whole thing working. Additionally, setting up the board to interface with the webcam was also an issue. The SD card would often be corrupted and slow down our progress.

Accomplishments that we're proud of
Considering our lack of experience using machine learning libraries, we were proud to be able to setup the machine learning environment that allowed us to train. Additionally, we were able to learn about the generally approach machine learning.

What we learned
We learned how to set up the CUDA library and how to use the basics of the PynqZ2 Board and a few of its overlays.

What's next for Sign Language Image Translation with PynqZ2 Board
Ideally, we would like to have the board read from a video instead of a set of images. This would allow for live and much more accurate image translation, and would also allow us to push the board to its full capabilities.

Built With
cuda
pynqz2
python
theano

Demo Link: https://www.youtube.com/watch?v=BW_27-82W9c
Devpost Link: https://devpost.com/software/sign-language-image-translation-with-pynqz2-board#updates
