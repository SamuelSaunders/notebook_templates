# Jupyter Notebook Templates

Collection of Jupyter Notebook templates and a virtualenv setup to run them.

## Setting up the Virtualenv

Create a new virtualenv:

  `$ virtualenv _notebook_venv --no-site-packages`

Activate the virtualenv:

  `$ source _notebook_venv/bin/activate`

Within the virtualenv install the packages within the requirements.txt file using pip:

  `$ pip install -r requirements.txt`

Run the ipykernel install command to ensure the notebooks can run in the virtualenv as documented [here](http://help.pythonanywhere.com/pages/IPythonNotebookVirtualenvs):

  `$python -m ipykernel install --user --name=my-virtualenv-name`

## Running the Notebook Server

Run the Notebook server in a screen session.

  `$ jupyter notebook`

Ensure the `Kernal` selected matches that of your virtualenv.


## Sharing Notebooks

### Public Notebooks

Use http://nbviewer.jupyter.org/ with the public URL of the notebook.

### Private Notebooks

Upload a secret Gist and link it via the secret URL on http://nbviewer.jupyter.org/.
