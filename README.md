# local_llm_webscraping_test

### Installation Guide
https://github.com/imartinez/privateGPT

https://stackoverflow.com/questions/60631933/install-detectron2-on-windows-10/72784255#72784255

https://medium.com/@yogeshkumarpilli/how-to-install-detectron2-on-windows-10-or-11-2021-aug-with-the-latest-build-v0-5-c7333909676f

https://dotnet.microsoft.com/pt-br/download/dotnet-framework



#### About Poetry on win 11
in Windows 11, after long and painful experiments with powershell and reading the poetry installation documentation, I solved the problem like this:

installed poetry with the command:
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
When the system reported that poetry was successfully installed and for poetry you need to register the path to the folder where it was installed. typing the poetry --version command there was an error in powershell that poetry is unknown, I could not register path through the command line.

through the windows folder window settings, I made the hidden folders and files visible and went to where poetry was installed: C:\Users\user\AppData\Roaming\Python\Scripts.

In order for python to see the path to poetry, I copied poetry.exe from the spot C:\Users\user\AppData\Roaming\Python\Scripts in the python work environment at: C:\Users\user\AppData\Local\Programs\Python\Python310\Scripts this way.

Pip also lies in Local. The problem was solved and the command in powershell poetry --version showed the poetry version. I hope this will help you!

## About CUDA
1. install cuda before Visual 2022 toolkit
2. install visual 2022 toolkit
3. install cuda again

https://medium.com/@piyushbatra1999/installing-llama-cpp-python-with-nvidia-gpu-acceleration-on-windows-a-short-guide-0dfac475002d

depois 

https://anaconda.org/conda-forge/cudatoolkit-dev
