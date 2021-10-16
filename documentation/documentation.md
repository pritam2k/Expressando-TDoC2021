<h1 align="center">EXPRESSANDO - TDoC 2021</h1>
![expressando](https://user-images.githubusercontent.com/76585827/137585523-2ff41a7e-3859-44e9-85ae-d0014a4fc661.png)



## What is a virtual environment?

what is an environment so environment is nothing but a it is basically a location it is like a container where you have your python and you have all other libraries installed. Now this is your base environment, base environment basically means where you have installed all your packages whenever you are working on any machine learning application or any other application but what happens let’s say you are specifically working on a project/task so in that case you might not need all these packages right you might not need everything so you may need a python but different version of python. And need some other packages. What you can do you can create a different container and this container is nothing but an environment. So when you have the base environment it is like the first environment or the like it is a default environment that is always present in your system but you can create some some additional environments also so these are know as your virtual environments.

Virtual environments allow us to create isolated environments for each of our python projects. Each virtual environment will be independent of one another due to this they can have different python versions and their own versions of packages and modules to resolve our earlier problem of conflicting versions of the module/library. We can have separate virtual environments for each project each of these virtual environments can then have their own separate packages of different versions.

## Why Virtual Environments?

When we start working on larger python projects we have to use different packages and modules that don't come pre-installed with the standard python library these packages and modules are constantly being updated with every new release let's suppose that we worked on a project that uses a library of specifically the version, after a few months you then worked on another project that uses a different version of that module, now if we have to go back to wroking on your first project you will either need to change the entire code base of the porject to make it compatible with new version or you'll have to uninstall new version and reinstall the old version more often that not your python projects will use different versions of many such packages or even an entirely different version of python that won't be compatible with one another. Virtual environments allow us to solve this problem instead of using a single and global python installation for all our projects we can create different virtual enviroments for dirfferent projects.

---

## Create Virtual Environments

In order to create a virtual environment we can use built-in module named **virtualenv**.
let's look at how we can create virtual environments i'll first create a directory or open directory if already and i'll open the terminal/cmd in this workspace. By default we are using the global python environment.
if you wnat to check which environment you use than. 

```bash
which python
```

and check how many library/modules are install that environment. 

```bash
pip list
```

now let's create an isolated python environment. To create an isolated pyhton environment use this command.

```bash
python -m virtualenv <name_of_venv>
```

then my new virtual enivronmnet has beeb created. Now you can see that there's a folder called (name_of_venv) in this folder. This directroy contains minimal python setup and executables for our python project.


## Activate Virtual Environments

No that we have created a virtual environment let's activate it we'll go to our terminal/cmd and use.

**FOR LINUX** <br>
```bash
source <name_of_venv>/bin/activate
```

**FOR WINDOWS** <br>
```bash
./env/Scripts/activate
```

now you can check which virtual environment use or list of packages in that virtual environment.
None of the global packages and modulea are available in this virtual environment now we kan install a specific library.
That version of library is available only for this virtual environment. it will not have any effect on our global python setup.


## Deactivate Virtual Environments

In order to deactivate a virtual environment we can simply use the deactivate command on our terminal/cmd. You can see that currently the (name_of_venv) virtual environment is activated let me deactivate this virtual environment.

```bash
deactivate
```

and you can see that the virtual env is deactivated now if i do **which python** than show your global environment.


if we create a another virtual environment , this won't affect our previous virtual environment in any way. No that we have learned about virtual environments. I highly encourage you to use separate virtual environments for each of your python projects this will prove very useful once you start working on a number projects with different requirements. 
you can then put all these requirements in a requirements file this requirements file can then be used to set up the same type of virtual environment on any machine.
if you want to remove a virtual environment you cna just delete the folder containing the virtual environment.

# **NumPy**

**NumPy** is a Python package that stands for ‘Numerical Python’. It is the core library for scientific computing, which contains a powerful n-dimensional array object.

## Where is NumPy used?

Python NumPy arrays provide tools for integrating C, C++, etc. IT is also useful in linear algebra, random number capability etc. NumPy array can also be used as an efficient multi-dimensional container for generic data. Now, let me tell you what exactly is Python NumPy aaray.

## How do I install NumPy?

To install Python NumPy, go to your command prompt and type:

```bash
pip install numpy
```

Once the installation is completed, go to your IDE/editor and simply import it by typing:

```python
import numpy as np
```


You can also refer to the following resources to know further about [**NumPy**](https://numpy.org/)

# What is Computer Vision?

Computer vision is an interdisciplinary field that deals with how computers can be made to gain high level understanding from digital images or videos so the idea is to automate tasks that the human visual systems can do so a computer should be able to recognize that this is a face of a human being, this is what a lamppost looks like so things like that right so i hope i'm clear what is meaning of computer vision.

Computer Vision is a field of study which enables computers replicate the human visual system. As already mentioned above, it's a subset of artificial intelligence which coolects information form digital images or videos and processes them to define the attributes. The entire process involves image acquiring, screening, analysing, identifiying and extracting information. This extensive processign helps computers to usnderstand any visual content and act on it accordingly.

Computer vision projects translate digital visual content inot explicit descriptons to gather multi-dimensional data. This data is then turned into a computer-readable language to aid the decision-making process. The main objective of this branch of artificial intelligence is to teach machines to collect information from pixels.

# How does a computer read an image?

How does a human mind apprehend an image? When you see the image below whtat do you actually see and how do you say what is in the image?

you most probably look for different shapes and colours in the image and that might help you decide that this is an image of a dog. But does a computer also see it in the same way? The answer is no.

A digital image is an image composed of picture elements, alsso knows as pixels, each wiht finite, discrete quantities of numeric representation for its intensity or grey level. So the computer sees an images as numerical values of these pixels and in order to recognise a certain image, it has to recognise the patterns and regularities in this numerical data.

Here is a hypothetical example of how pixels form an image. The darker pixels are represented by a number closer to the zero and lighter pixels are represented by numbers approaching one. All other colours are represented by the numbers between 0 and 1. 

But usually, you will find that for any colour image, there are 3 primary channels – Red, green and blue and the value of each channel varies from 0-255. In more simpler terms we can say that a digital image is actually formed by the combination of three basic colour channels  Red, green, and blue whereas for a grayscale image we have only one channel whose values also vary from 0-255.

# Waht is OpenCV?

OpenCv (Open Soucre Computer Vision Library) is an open source software library for computer vision and machine learning. OpenCV was created to provide a shared infrastucture for applications for computer vision add to speed up the use of machine perception in consumer products. OpenCV, as a BSD-licensed software, makes it simple for companies to use and chagne the code. There are some predefined packages and libraries that makes our life simple and OpenCV is one of them.


# Install OpenCV

## For Windows Or Linux 

you can use pip to install OpenCV on windows. Pip is a de facto standard package-management system used to install and manage software packages written in Python and it usually comes in installed when you install Python. If you do not have Python installed, I would suggest download it from here. Use this command in the command prompt to install OpenCV:

```bash
pip install opencv-python
```

## For Mac

You can use homebrew to intall OpenCV as it makes it really easy and you just have to use this command for installing:

```bash
brew install opencv
```

You can also refer to the following resources to know further about **[OpenCV](https://opencv.org/)**

# **TensorFlow**

## What is tensorflow?
**TensorFlow** is a free and open-source software library for machine learning and artificial intelligence. It can be used across a range of tasks but has a particular focus on training and inference of deep neural networks. Tensorflow is a symbolic math library based on dataflow and differentiable programming.

# **Keras**

## What is keras?
**Keras** is an open-source neural-network library written in Python. It was developed by Francois Chollet while he was at Google. In simple words, Keras is a high Level API(Application Programmable Interface) that allow to build the Deep learning or Machine Learning models easily without detail understanding about internal architecture how the ML algorithm works internally.