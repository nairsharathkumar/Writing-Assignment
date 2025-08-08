# How to install MkDocs on Ubuntu 22.04
## Prerequisites
1. You should have Python 3.7 and above running on the machine.
2. pip 19.0 and above should be installed on the machine.
3. A user account with sudo privileges.

### Check python and pip version on the machine
#### Command to check Python version
 Run the following commands on the terminal to check the version of python installed on the machine.
 ``` 
 python3 --version
 ```
 If the python version is less than **3.7**, run the follwing commands to upgrade Python.
 ```
sudo apt update
sudo apt install software-properties-common -y
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.11 python3.11-venv python3.11-distutils -y
```
##### Verify the Python version
Run the follwong command to verify the python version
```
python3 --version
```
#### Command to check pip version on the machine
```
pip --version
```
If the **pip** version is less than **19.0**, run the following command to upgrade pip.
```
python3 -m pip install --upgrade pip
```
##### Check pip version
Run the following command to to verify the pip version
```
pip --version
```
---

## Install MKDocs
Run the following commands to install MkDocs. Make sure the Python and pip versions on your machine meet the prerequisites outlined earlier.
1. Run the following command to check for updates.
  ```
  sudo apt update
  ```
2. Run the following commands to create and activate a virtual environment
```
python3 -m venv mkdocs-env
source mkdocs-env/bin/activate
```
3. Run the following commands to install MkDocs
```
pip install mkdocs
```
### Verify Mkdocs installation

1. Run the following command to verify Mkdocs installation.
```
mkdocs --version
```
## Install Read the Docs theme
MkDocs comes with built-in themes. However, you can download and install customized themes for your MkDocs project.
Run the following command to install the **Read the Docs** theme.
```
pip install mkdocs-readthedocs-theme
```
### Use Read the Docs theme
1. Access the **mkdocs.yml** file on your machine.
2. Modify the **name** sub-key inside the **theme** key to **readthedocs**
3. Save the changes to the **mkdocs.yml** file.
4. Run the command below to restart the live server.
``` 
mkdocs serve
```



 
