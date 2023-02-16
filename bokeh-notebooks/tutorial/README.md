## Clone or download the repo
First get local copies of the tutorial notebooks:


```
$ git clone https://github.com/bokeh/bokeh-notebooks.git
```


Or download from: https://github.com/bokeh/bokeh-notebooks/archive/master.zip


**Note:** 

The bokeh repo above uses some previous versions of packages and dependencies, which might not work exactly the same as the ones used in our version of environment. We recommend getting the tutorial notebooks from the repo we are using for this course: https://github.com/rongliyuan/DVC-FS23.git


## Install the dependencies

The tutorial notebooks in the DVC-FS23 repo has been tested on:

* bokeh 3.0.3
* pandas 1.5.3
* notebook 6.5.2
* pillow 9.4.0
* selenium 4.7.2

Other combinations may also work.

The quickest, easiest way to install is to use Anaconda (or Miniconda):

#### Installing with anaconda

Install [anaconda](http://anaconda.com/downloads)

Anaconda should come with all the dependencies included, but you may need to update your versions.

#### Installing with miniconda

Install [miniconda](http://conda.pydata.org/miniconda.html).

Use the command line to create an environment and install the packages:

In the folder `bokeh-notebooks` where the `environment.yml` file is, run the following command:

```bash
$ conda env create
```
<br>  
When it is done, run the following command to activate the environment:

```bash
$ source activate bokeh
```
<br>  
Now the name of the current environment "bokeh" should appear in front of the path:

```bash
(bokeh) .../bokeh-notebooks 
 ```
<br>  
To show the list of packages in the current environment:<br>

```bash
$ conda list
```  
<br>
If later you find some dependency missing, e.g. `pillow`, you can install it with:

```bash
$ conda install pillow
```

## Get the sample data

Bokeh has a [sample data](https://docs.bokeh.org/en/latest/docs/reference/command/subcommands/sampledata.html) download that gives us some data to build demo visualizations. To get it run the following command at your command line:

```bash
$ bokeh sampledata
```
  
or run the following from within a Python interpreter:

```python
import bokeh.sampledata
bokeh.sampledata.download()
```

### Install Datashader and Holoviews (optional)

Some optional sections require the additional packages Flask, Datashader, and Holoviews.
These  can be installed with:

```bash
$ conda install -c pyviz datashader holoviews flask
```


## Run the Jupyter notebook

From this folder run 

```
$ jupyter notebook
```

and open the `00 - Introduction and Setup.ipynb` notebook in the `tutorial` folder.