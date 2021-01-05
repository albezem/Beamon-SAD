# BEAMON

Beamon is a Static Analysis Design Software for 3D Beam truss structures. 
Both database and simulation are based on SQLite3 and CALFEM-Python respectively.

## Installation
### Python Package
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requirements from requirements.txt file.

```bash
pip install -r requirements.txt
```
### Windows Executable
Download windows executable in releases directory.

## Usage
### How to use beamon package
To run Beamon package use the following command in your python environment
```bash
python -m beamon
```
This will execute the user interface of Beamon

Available command line arguments are:
- -i \<path to geometry file\>
- -o \<path to output geometry file\> **(will be removed in future releases)**
- -t test mode (lunches all submodules on start)
- -r ram mode (runs database on RAM)
- -d \<path to database file\>

## Contributing
Both `make.bat` and `make.sh` contain functions to run on your command line.
For example on your linux machine run
````shell script
./make install_requirements
````
and on your Windows machine run
````bash
make.bat call install_requirements
````
to install all requirements in your python environment.

### How To: requirements 
you will be able to install all required packages inside the python environment of your choice (I personally recommend Anaconda environments).
Running the command `pip install -r requirements.txt` inside the root project directory  

### How To: Sphinx Documentation

- build html documentation using `make html` command inside `docs` directory
- build PDF documentation using `sphinx-build -b rinoh . _build/rinoh` command inside `docs` directory


Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
Maher Albezem