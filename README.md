# web-blockchain
Blockchain-based ledger, with [Streamlit](https://docs.streamlit.io/) web interface.

---

## Overview
Web-blockchain is an [application](app/pychain.py) which allows the user to view, add, and validate blocks on a blockchain, via a web interface.  

## Assumptions & Process
Web-blockchain applicaton will use [python](https://www.python.org/), and highlight the [Streamlit](https://docs.streamlit.io/) web interface library, along with the use of Python classes as they pertain to modeling Record, Block and Chain dataclasses.

**High-level steps:**  
1. Create a `Record` data class which will encapsulate the data in the transaction of the block.
2. Update the `Block` class to work with `Record` data.
3. Add Web UI functionality via [Streamlit](https://docs.streamlit.io/) which handles `sender`, `receiver` and `amount`, and works with the `Record` data type.

**Submission:**  
- Final [web application](app/pychain.py)
- videos of testing and running application (see below)

## Web Application Testing and Validation

**Testing** of Add Block, View Chain:  
![UI Test](media/testing.gif)  

**Validation** of Blockchain:  
![Block Validation](media/validation.gif)  


---

## Technologies

This challenge uses [python](https://www.python.org/) 3.7 and the following modules:  
- [datetime](https://docs.python.org/3.7/library/datetime.html)
- [dateutil](https://dateutil.readthedocs.io/en/stable/)
- [streamlit](https://github.com/streamlit/streamlit)
- [dataclasses](https://docs.python.org/3/library/dataclasses.html)
- [typing](https://docs.python.org/3/library/typing.html)
- [pandas](https://pandas.pydata.org/)
- [hashlib](https://docs.python.org/3/library/hashlib.html)  

See [installation](#installation) and [usage](#usage) below for specifics.

---

## Installation

You will need Python 3.7, that supports for this application to run. An easy way to install python 3.7 is to download and install [Anaconda](https://www.anaconda.com/products/individual). After installing anaconda, open a terminal/command-prompt, and setup a python 3.7 environment, and then activate it like so:

```
# create an anaconda python 3.7 environment
# name can be any friendly name to refer to your environment, eg 'dev'
conda create --name dev python=3.7 anaconda

# activating the environment
conda activate dev

# use pip to install the above modules, eg:
pip install dateutil
...etc...
```

---

## Usage

To run the application, use the CLI and launch streamlit like:  

```
# activating the environment
conda activate dev

# change to application directory
cd <repo_root>/app

# launch streamlit application
streamlit run pychain.py

```

---

## Contributors

[David Lopez](https://github.com/sububer)

---

## License

MIT