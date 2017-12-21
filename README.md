# AI-Resources
## Introduction

AI is becoming a very large and fast moving area that is rapidly changing all of our lives.  This list of resources is intended to help people getting started in this field to know where to go, and to help minimise the early problems of deciding what approach to take.

While I intend to keep this resource list as up to date as possible, if anybody finds links that are out of date or finds some solutions that are better than the ones I have suggested please let me know.

## The Environment

### Hardware

Before covering the software environment it is also necessary to cover the computational hardware / facilities needed.  For most of the training course exercises that can be found below I found a reasonably modern Intel i5 or i7 desktop or laptop is adequate.  It helps if it has a GPU but not any GPU, pretty much all of the software frameworks are designed to work with Nvidia GPUs and a software library from Nvidia called CUDA.

As you move from small training course cases to real world examples then you are certainly going to need some more powerful kit, at which point you need to either invest in a workstation with lots of RAM, dosk (ideally solid state), and the most powerful GPU you can affort.  The other alternative which does not require capital investment is to setup a virtual machine on Amason Web Services. There are several links on the web that explain how to do this and I will add one shortly once I have established the easiest to follow.  If you need something more urgently then follow one of the early items covered in the fast.ai training course below is how to setup an AWS instance.
Whilst there are many machine learning and AI frameworks out there it seems to me that the centre of mass is in the Python open source community. There are resources based around R, mainly used by people that have come from a data science background, and there are resources based around Matlab and its open source equivalent Octave.  My recommendation would be for somebody to start with Python since this seems to be the way it is going and where I see most examples / open-source applications.



Whichever language you choose to use you will need to setup a local environment and code editor.  I would suggest the following but there are many others to choose from:

### Software

#### Anaconda-navigator  
This very useful framework lets you setup a dedicated environment for a particular application, and helps to load all of the required libraries and keep this up to date.  If you wish to use different frameworks (see section further down) you will find that each framework seems to need different versions of libraries and hence, unless you have a dedicated one for each, it is very difficult to get them all to work properly.  Anaconda navigator makes this easy to manage. It also provides ready and easy access to other resources that are useful, and including:
- Jupyter Notebooks.
- iPython Console.  An interactive Python console that supports inline figures syntax highlighting etc.  It is often useful to use a notebook and a console with the same session.
- Spyder – scientific python development IDE.  Has good features including debugging though I find Pycharm more capable
- Orange – a shareware graphical data mining and analysis tool

Jupyter notebooks is a very useful tool that allows software to be written and run in a web browser and also facilitate effective narration of what is happening in the code (much more so than the old comments that traditional programmers rely upon).  It also allows a good blend of interactive and scripted coding.  For this reason such notebooks are extensively used for tutorials and examples.  Personally, I like the way this works with a couple of caveats. Firstly code auto-complete does not work (or at least I haven’t found a way to make it do so).  Secondly, I find debugging with notebooks very cumbersome compared to traditional software tools.
To overcome the latter limitations, I also make extensive use of another free resource called PyCharm.  Pycharm is a more traditional IDE which works very well with Python and has excellent code completion, debugging and project management tools.

Anaconda-navigator is supplied by Continiuum Dynamics Inc and can be downloaded from [here](https://anaconda.org/anaconda/anaconda-navigator)

#### Pycharm
PyCharm can be downloaded from [here](https://www.jetbrains.com/pycharm/?fromMenu). Note that I have found the community free version perfectly meets my needs so far.

## Training / Self Learning

In terms of training I would suggest the following:
- fast.ai.  The courses can be found from the home page [here](http://www.fast.ai/)
This is Python based and free.   It gets good reviews and is a very practical approach although they do suggest and almost require you to use an AWS instance which will cost you a few $ in fees.

- Coursera: Machine Learning by Andrew Ng and Stanford University.  This is the course I (and many others) started with and can be found here [here](https://www.coursera.org/learn/machine-learning). The only issue with this course is that it is based around Octave (a shareware version of Matlab), and learning this is a bit of a waste of time when you want to move to Python eventually.  The course is free until you want a certificate, for which there is a small fee

- Another very good Coursera course that is also free unless you want a certificate is Neural Networks for Machine Learning by Geoffrey Hinton and Toronto Univerity.  The course can be found [here](https://www.coursera.org/learn/neural-networks). I did this course after the one above.  This course also uses Octave / Matlab.  The course creator is one of the father figures of AI and very insightful (though he leaves you to do a lot of research and work on your own, much less hand holding than the above course).

- Andrew Ng, the creator of the first Coursera course above has now launched a five module course on AI which is Python based and seems to get good reviews but you do have to pay to take it.  I think it’s about $30 per month.  The course curriculum can be found [here](https://www.coursera.org/specializations/deep-learning)
 
There are many other online resources such as Udemy.  Udemy courses were quite expensive but I note that at the time of writing prices have been reduced considerably.  People tell me these are very good but I haven’t tried them personally.  If you are interested more details can be found [here](https://www.udemy.com/courses/search/?ref=home&src=ukw&q=AI)

## Software Frameworks

There are many opensource or freely available frameworks that can use used by anybody.  The list below is not comprehensive but covers many of the major packages.  At present I tend to use PyTorch and Keras / Tensorflow.  I like Pytorch because it is very integrated with Python and offers considerable scope to customise it as you feel fit.  I also like the dynamic gradient calculation.  Having said that, if you just want to run relatively standard applications as quickly and easily as possible I think Keras takes some beating.

The frameworks are:
- [Tensorflow](https://www.tensorflow.org/) from Google (can be used via [Keras](https://keras.io/))

- [PyTorch](http://pytorch.org/) (supported by Facebook and others, I believe this is usually used for research and then production solutions are moved to [caffe2](https://research.fb.com/downloads/caffe2/)

- A recent release from Uber Labs is found [here](https://eng.uber.com/pyro/).  This uses PyTorch as a backend and adds substantial probabilistic deep learning capability.

- Microsoft Cognitive Toolkit, which can be found [here](https://www.microsoft.com/en-us/cognitive-toolkit/)

- Deep Learning for Java from Skymind.  This can be found [here](https://deeplearning4j.org/). This framework is the main one that is focussed upon the Java environment and will hence be of considerable interest to people used to programming in Java.

- MXNet – note this has now been integrated into the Apache environment.  There has been a lot of support for MXNet from Amazon.  The framework can be found [here](https://mxnet.incubator.apache.org/)

- OpenAI.  Open AI has produced some extremely useful tools for people working on AI as well as doing some very good research and development.  The main things of relevance here are:
	- Gym – a toolkit and playground for testing and developing re-enforcement learning AI software and models
	- Universe – a toolkit to test the intelligence of AI systems
    
The Open AI tools can be found [here](https://openai.com/systems/)

- Deepmind.  Deepmind is best known by many for its development of the systems that won the AlphaGo competition.  In addition they are doing some other very interesting work and their opensource frameworks are [here](https://deepmind.com/research/open-source/)

- Theano.  Theano has been a widely-used platform for many years and, at least until recently, there were probably more examples of solutions using Theano than any other platform.  Theano can be found [here](http://deeplearning.net/software/theano/).  Personally I find Theano more complex to use than PyTorch or Keras.

- Apache Singa / Spark / Mlib.  As well as MXNet above there are a number of ML solutions within the Apache Software Framework including Singa, Spark, Mahout, Scala

- Scikit-learn.  This is a simple and easy to use set of tools that help with data pre-processing and post processing.  There are also libraries for classification regression, clustering etc.  The library can be found [here](http://scikit-learn.org/stable/)

- H2O.  H2O.ai provide many powerful deep learning and data analysis tools.  I might be wrong but I think the main user base is Data Scientists and and many examples I have seen are based on R.  There are Python and Java interfaces as well.  This also looks to have good interfaces to commonly used databases to help with data management.  The tools can be found [here](https://www.h2o.ai/)

- Octave.  This is an open-source software that uses Matlab language.  It is often used to learn ML.  It can be found [here](https://www.gnu.org/software/octave/)

## Useful papers and resources

There are a plethora of papers and resources and I will not attempt to reference them all myself when many people have already done so and hence in many cases it is most appropriate simply to link to lists other people have already developed.

Specifics that are worth mentioning include:
- Neural Networks and Deep Learning, an e-book by Michael Nielsen.  This is easy to follow and an excellent introduction.  It can be found [here](http://neuralnetworksanddeeplearning.com/)

- Deep Learning – a book by Ian Goodfellow, Yoshua Bengio and Aaron Courville.  It can be found [here](http://www.deeplearningbook.org/).

- [Kaggle](www.kaggle.com) is a very valuable resource.  The site hosts many competitions for machine learning and the datasets are available for everybody to use for their own development.  Additionally, in most cases the software that other people have used is also available for inspection and use, which can be really valuable in helping to identify possible approaches to specific problems

- Github is an invaluable resource that contains tutorials, examples and projects for almost every conceivable application.  Whilst it will almost always be necessary to adapt these for your own purposes it provides a very good starting point.

- There are many very good online talks by leaders in the field.  Some of the best are:
	- [Yann LeCunn - Shannon Lecture](https://www.youtube.com/watch?v=zaoL0LUctK4&t=8s)
this provides a very good history and view of where AI is going and some of the most important developments including GAN
	- Jason Yosinski - a very powerful video of how a convolutional neural network learns and how the different layers work.  It is also possible to access a toolbox that can be installed locally.  The video is [here](https://www.youtube.com/watch?v=AgkfIQ4IGaM)
	- More to be added

- The link [here](https://github.com/terryum/awesome-deep-learning-papers) contains references to many of the leading papers in fields including object recognition, NLP, speech, re-enforcement learning etc.

- This link from Robbie Allen contains links to many good tutorials that I have used many times.  The site is [here](https://github.com/terryum/awesome-deep-learning-papers)

 - a very good tutorial on data pre-processing techniques has been produced by Guido Zuidhof.  It is especailly valuable since it covers 3D images using DICOM files, as are used for medical scans etc.  The link is [here](https://www.kaggle.com/gzuidhof/full-preprocessing-tutorial)




