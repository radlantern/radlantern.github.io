# Installation notes for Python 3.6 with pip in Windows 10

I recently installed python on my Windows 10 laptop and wanted to use pip to install
some modules.  There were a few snags that I will detail here.

## TL;DR

Git pip working on Windows 10 (maybe others too) by doing the following.

* Add the actual Python executable to your path:


    C:\Users\username\AppData\Local\Programs\Python\PythonXX

* Run pip as a module:


    python -m pip install ...
    python -m pip etc ...


## Installation Path Notes
The installer contains a nice option for adding Python to the PATH  However it is only the loader `py` that gets added.  Helpful, but so far attempts to run this as `py -m pip` or some variation of has not worked for me.

Most of the docs still indicate that the Python will be installed to something
like C:\Pythion_XX_ but in the current installer the default location for me was
`C:\Users\username\AppData\Local\Programs\Python\PythonXX`

## Running pip
Even once I found the python executable, I still wasn't sure how to get the pip module running directly in the command line under windows.  There may be some way to do this similar to how things work with NPM.  So far I have not figured it out.
