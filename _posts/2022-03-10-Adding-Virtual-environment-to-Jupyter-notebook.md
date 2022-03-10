---
layout: single
permalink: /posts/
title: Adding Virtual Environment to Jupyter Notebook
---
## Adding a new virtual environment to Jupyter Notebook
After we create a virtual environment, we need to add the created virtual environment to Jupyter notebook. 
1. Make sure you have activated the virtual environment and execute below code:
```
pip install --user ipykernel
```
2. Manually add the kernel / virtual environment to the Jupyter notebook:
```
python -m ipykernel install --user --name=NewVirtualEnvironment
```
3. Close the command prompt and open jupyter notebook:
```
jupyter notebook 
```
4. Select the "New" dropdown and you should be able to find newly created virtual environment.

5. Uninstalling: If you need to uninstall the kernel, we can use below command:
```
jupyter kernelspec uninstall VirtualEnvironment
```