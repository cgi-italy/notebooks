# Insula API and Insula AI Jupyter Examples

A set of Jupyter Notebooks showing the usage of Insula's APIs, in particular:

- [Access & Discovery](https://github.com/cgi-italy/notebooks/blob/main/Access%26Discovery.ipynb): query catalogs and collections, download files
- [SearchAPI](https://github.com/cgi-italy/notebooks/blob/main/SearchAPI.ipynb): catalog search, download api and WMS/WFS capabilities
- [Data Collections](https://github.com/cgi-italy/notebooks/blob/main/DataCollections.ipynb): create collections and upload files
- [Processing Services](https://github.com/cgi-italy/notebooks/blob/main/ProcessingServices.ipynb): see available services and launch one
- [OpenEO](https://github.com/cgi-italy/notebooks/blob/main/OpenEO.ipynb): learn how to use the OpenEO library and services to access external data.
- [Kubeflow Pipeline](https://github.com/cgi-italy/notebooks/blob/main/Kubeflow_Hello_world.ipynb): Jupyter Notebook to produce yaml file of a simple "Hello world!" pipeline

## Create a virtual environment for OpenEO
By creating a virtual environment, we can install the libraries needed by the OpenEO notebook in a way that they can survive Jupyter server reboots. To do this open a terminal inside Jupyter and use the following commands:

```bash
# Create a new environment:
python -m venv /home/jovyan/OpenEoEnv

# Make it active:
source /home/jovyan/OpenEoEnv/bin/activate

# Install the required packages:
pip install openeo
pip install rasterio
pip install matplotlib

# Enable the environment for usage in a notebook’s kernel
pip install ipykernel
ipython kernel install --user --name=OpenEoEnv
```