# stacco-data

A Jupyter notebook to explore the data collected from the **Stack Overflow Annual Developer Survey**, with particular focus on the developers compensation. 

The dataset can be downloaded [here](https://insights.stackoverflow.com/survey).

## How to run it with Docker
The script `jupyter.bat` creates and runs a [miniconda](https://docs.conda.io/en/latest/miniconda.html)-based Docker container with Jupyter and all the required dependencies. The container:
- maps the Jupyter listening port to http://localhost:7777
- mounts the local folder `./notebooks` as the Jupyter working folder

When  Jupyter is initialized, the token to access the first time via browser is printed on standard output. Something like this:
```text
[I 10:31:35.145 NotebookApp] Serving notebooks from local directory: /opt/notebooks
[I 10:31:35.145 NotebookApp] Jupyter Notebook 6.4.3 is running at:
[I 10:31:35.145 NotebookApp] http://1cc93404b18f:8888/?token=3964ca1fb3b8c41083ceec547f882af2736bc99b61c1aa4f
[I 10:31:35.145 NotebookApp]  or http://127.0.0.1:8888/?token=3964ca1fb3b8c41083ceec547f882af2736bc99b61c1aa4f
[I 10:31:35.145 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 10:31:35.149 NotebookApp]

    To access the notebook, open this file in a browser:
        file:///root/.local/share/jupyter/runtime/nbserver-1-open.html
    Or copy and paste one of these URLs:
        http://1cc93404b18f:8888/?token=3964ca1fb3b8c41083ceec547f882af2736bc99b61c1aa4f
     or http://127.0.0.1:8888/?token=3964ca1fb3b8c41083ceec547f882af2736bc99b61c1aa4f
```
Copy the token and append it to http://127.0.0.1:7777 to get the correct URL (e.g. `http://localhost:7777/?token=3964ca1fb3b8c41083ceec547f882af2736bc99b61c1aa4f`)

