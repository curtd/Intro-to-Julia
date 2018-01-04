# Introduction to Julia

## How to Install Julia
Precompiled binaries for Windows, OS X, and Linux are available at https://julialang.org/downloads/. 

Usually your Julia installation is placed in /Applications/Julia-0.6.app. In this case, add the following to your ~/.bash_profile in OS X
```
    export PATH="/Applications/Julia-0.6.app/Contents/Resources/julia/bin/:${PATH}"
```
so that you'll be able to start the julia binary from the terminal. 

## How to Install Jupyter
If you don't already have Jupyter installed on your system, either install Anaconda [https://www.continuum.io/downloads] or, if you have an existing Python installation in your system, follow the instructions over at [http://jupyter.org/install.html]. 

## Hooking Julia into Jupyter
Open your Julia REPL, then type 
```
    ENV["JUPYTER"] = "location/to/jupyter/binary"
    Pkg.add("IJulia")
```

Julia will integrate the necessary files into Jupyter to allow you to run Julia notebooks. When this process is done, from the command line, enter
```
    jupyter notebook
```

A browser window should open up listing the files/folders in your home directory. To create a new Julia notebook, click on "New->Julia 0.\*.\*" corresponding to your version number. For more information and troubleshooting, visit [https://github.com/JuliaLang/IJulia.jl]. 

## Jupyter Notebook Tutorial
More information (albeit not complete) over in ``Julia Tutorial.ipynb``

## Calling Julia from Python
Check out the PyJulia library [https://github.com/JuliaPy/pyjulia]  