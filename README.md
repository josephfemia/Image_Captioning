# Image Captioning
Utilize a Tensorflow Resnet 50 for encoding the image and a LSTM network to generate captions

## How to install and run the notebook
This project was made using [Pipenv](https://github.com/pypa/pipenv) for keeping track of dependencies. First you must have Pipenv installed:
```
pip install pipenv
```
After having Pipenv installed, you should create a virutalenv for the project. To do this, cd into the directory and run the command:
```
pipenv shell
```
Finally, to install the necessary dependencies run:
```
pipenv install
```
By calling ```pipenv install``` you install all of the necessary dependencies within the Pipfile.lock.

All that is needed to run the notebook now is just run the command below and check oyur browser instance for a new Jupyter Notebook tab:
```
jupyter notebook
```
The [MS COCO](https://cocodataset.org/#download) Captioning 2015 dataset was used to train the model. Follow the MS COCO documentation in order to download the dataset. I specifically used the validation set since I had restricted CPU memory and a limited GPU. If I trained on the training set was it would result in an unfesable training time per epoch. Thus, this model could perform better with training on the training set and running for more epochs.
