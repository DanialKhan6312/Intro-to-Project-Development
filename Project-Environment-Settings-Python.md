# How to Create a Virtual Environment in Python

*Note, many IDE's (PyCharm) already create a virtual environment by default when starting a new project*

## What are we going to do?

* Using Python and the Terminal, we are going to set up a virtual environment to download external libraries
* Some dependencies before we get started
  * Python version 3.3 or greater
  * A package installer for Python (Pip, Conda)
    * We will use PIp in this example

## Making a venv in Python

1. Open of the Command Line / Terminal, go to the project folder

   ```
   $ cd projectFolder\project
   ```

   

2. Create a venv in the current project folder

   ```
   $ python -m venv VENV_NAME
   ```

   

3. Activate your venv 

   ```
   $ VENV_NAME\Scripts\activate
   ```

   

4. Import External Libraries 

   ```
   $ ( VENV_NAME ) pip get numpy
   ```

   *This will download the dependency numpy and place it in your venv instead of a global environment*

   *Also note the round bracket with VENV_NAME, this is how you know if you successfully opened your venv*

   

5. Deactivate venv (to close / to switch)

   ```
   $ deactivate
   ```

   

   