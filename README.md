# learn-tensorflow-udemy
My notes &amp; codes from Jose Portilla's Deep Learning course on Udemy


## Setting up work environment
### Create `conda env`
Go to where `tfdl_env.yml` is, and run
```bash
conda create env -f tfdl_env.yml
```
For Mac users, instead run
```bash
conda create env -f mac_tfdl_env.yml
```
The `.yml` file simply specifies a list of Python packages and versions to define an environment, and give such environment a name.  
In our case, this `.yml` file is provided by Jose, and it describes a virtual environment called `tfdeeplearning`.  
(You can run `head mac_tfdl_env.yml` to take a look at what's inside.)

### Activate `tfdeeplearning` environment for Jupyter Notebook
You need to first activate the environment before the Jupyter Notebook session can know where to find `tensorflow` and other packages as requested by the `.yml` file.
Otherwise, Jupyter Notebook would go to your default Python installation to look for tensorflow, which might be absent or of a different version from what the course uses.  
To activate virtual environment `tfdeeplearning`, run:
```bash
source activate tfdeeplearning
```
Then when you run `jupyter notebook`, it'll know to find python packages in the `tfdeeplearning` environment.  
To deactivate the virtual environment and go back to default python environment, run
```bash
source deactivate
```

### Set up Python interpreter for PyCharm project
If you're using an IDE like PyCharm, you'll need to tell the IDE where to find the virtual environment (thus the needed python packages).  
Refer to [this post from Anaconda](https://docs.anaconda.com/anaconda/user-guide/tasks/integration/pycharm) for how to tell PyCharm to use the virtual environment for this project.  




