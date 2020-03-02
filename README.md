# Assignment 1 - Introduction to Python!

Hi All, as we progress on the course, assignments needs to come, so there you go, your very first assignment!

As I said, this assignment won't be a full coverage on python, but rather it would be a warmer for you to get hands on experience to the stuff we need in the upcoming weeks of this course. Therefore, in this repository, we will use python to solve some basic tasks, work with jupyter notebooks, set an environment, in a proper way, using python standard environments.

## How You Should Start to a Project!

By creating an **environment!**

Environments is a box for your project in order to keep a clean definition of what your project needs as dependencies, makes your project works safely by not messing up with your local packages, and so on. It is a good practice to use environments as you get yourself involved in more complicated projects!

Before talking about environments, I want to give you a brief description of how python works. You can install python through standard python distribution or other distributions such as Anaconda. 

When you install it with Anaconda, it comes with additional packages in addition to standard python libraries. Therefore, when you launch anaconda, conda starts the base environment, which has all the additional packages in, and you will be able to use imports right in there. 

If you choose to install the standard python, then you only get the standard python libraries, with no additional package. 

Python or Anaconda lets you install packages using packages managers, pip and conda, and the packages will be downloaded and installed to your `site-packages` folder. The packages installed in your local system, will be accessible to all the projects, where you use your local python.

Now, lets assume that you are working on two projects, where you use a third party package that both of the projects depends on it. In one of your projects, you built so much using this third party package, and you don't want to upgrade the package for stability reasons. In this situation if you do `pip install --upgrade dependency_package`, both of your projects will use the upgraded version of this dependent package.

This is a common use case for environments. You keep your dependency packages fixed! Luckily, working with environments is very easy.

<h3> Create an Environment </h3>

You can create an environment like this using standard python. For Anaconda, use [managing environments documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) to create conda environments. For our class, you can create one environment to use for all future assignments!

``` sh
python -m venv spu-bigdataanalytics-env
```

Installing package dependencies will be easy with a `requirements.txt` file. 

``` sh
python -m pip install -r requirements.txt
```

There are more commands of pip like `pip list`, `pip freeze`, and so on.

### Use an Environment

To use an environment, you need to **activate** it. You can google all this stuff, but for assignments sake, I am putting it here. It changes based on your operating system.

For mac and linux, like following.

``` sh
# mac/ linux
source path/to/your/envronment/bin/activate
```

For windows, as in below.

``` ps1
# windows
C:\Path\to\Your\Environment\Scripts\Activate.ps1
```

To deactivate, like in below for all operating systems.

```
deactivate
```

Very easy.

## How to Use Jupyter Notebooks

Jupyter notebooks is a python package. You can install it like this. After installing, verify the installation by using the command `jupyter --version` to get the version.

``` sh
python -m pip install jupyterlab
```

To run a jupyter notebook, you can use the following. You can use `--generate-config` to customize jupyter, or you can pass options during launching.

``` sh
jupyter notebook --notebook-dir="path/to/your/project/"
```

## Your To-Do List for This Task

- [ ] Create your environment and install the requirements folder.
- [ ] Complete the tasks in the jupyter notebook.
- [ ] Once you done, do your final commit and zip it to upload to the blackboard!
