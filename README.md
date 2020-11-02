# DeepHeart

Code for Deep convolutional neural networks to predict cardiovascular risk from computed tomography. This code was developed and tested with Python 2.7.17.

For the code to run as intended, all the packages under `requirements.txt` should be installed. In order not to break previous installation, it's highly recommend to create a virtual environment to install such packages in. Here follows an example of set-up using `python virtualenv`:

```
# install python's virtualenv
sudo pip install virtualenv

# parse the path to the python2 interpreter
export PY2PATH=$(which python2)

# create a virtualenv with such python2 interpreter named "venv"
# (common name, already found in .gitignore)
virtualenv -p $PY2PATH venv 

# activate the virtualenv
source venv/bin/activate
```

At this point, `(venv)` should be displayed at the start of each bash line. Furthermore, the command `which python2` should return a path similar to `/path/to/folder/venv/bin/python2`. Once the virtual environment is activated:

```
# once the virtualenv is activated, install the dependencies
pip install -r requirements.txt
```

To deactivate the virtual environment, run:

```
deactivate
```

## Input Data

This section will describe how the input data should be formatted for the model to work as intended.
