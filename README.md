# 2025 PIFuHD working notebook (finger cross for you) 


From my experience, the original PIFuHD code encounters compatibility issues with the latest versions of libraries. These issues arise due to updates in Python, pre-compiled wheels, or the latest PyTorch versions. To ensure smooth execution, I followed these steps:

* Ensure Python Compatibility:
The first and most crucial step is to use a compatible version of Python. In this notebook, I am using Python 3.9, as the latest versions may introduce breaking changes.

* Override the Default Python Version in Google Colab:
After installing Python 3.9, we need to override the default Python version in the Colab runtime. By doing this, we ensure that the correct version is used throughout the execution of the script.

* Install PIFuHD Dependencies:
Next, we must install all the required dependencies for PIFuHD. The original requirements may not always be compatible with the latest library versions, so it is important to verify each package installation.

* Fix Deprecated Code in the Original Script:
The original codebase contains deprecated functions that are no longer supported in the latest versions of Python and PyTorch. I have updated multiple parts of the code, including modifications to recon.py and other related scripts, to align with current standards.

* Handling the Renderer Block Issue: The final step involves executing the renderer block. However, this particular section did not work for me. The issue seems to stem from Colab not properly recognizing the correct Python version internally at this step. To work around this, I modified the execution approach by running the Python code directly from the interpreter.


-------------

⚠ Note 1 - If this last step fails for you, don’t worry! The final output will still be available inside:

```
pifuhd/results/pifuhd_final/recon
```


⚠ Note 2 - Please ignore this sort of warnings
WARNING:
    You currently have a PYTHONPATH environment variable set. This may cause
    unexpected behavior when running the Python interpreter in Miniconda3.
    For best results, please verify that your PYTHONPATH only points to
    directories of packages that are compatible with the Python interpreter
    in Miniconda3: /usr/local

⚠ Note 3 - Also, ignore any message from COLAB to reload the Session or runtime in order to take the latest changes. Just ignore the alert and carry on. 

⚠ Note 4 - You can find the generated OBJ file there, which can be loaded into Blender or Mixamo for further processing.


⚠ Note 5 - At one point, you will need to manually select the correct path for Python 3.9. Refer to the following image for guidance on how to do this.
