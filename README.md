# bostonhousepricing


create a new environment

```
conda create -p venv python -y

```

```

conda activate C:\Users\mokas\bostonhousepricing\venv

```

When you run the cells, you may get an error if you don't have ipykernel installed.

Install it using this command: conda install -p c:\Users\mokas\bostonhousepricing\venv ipykernel --update-deps --force-reinstall

if you get this error:

CondaSSLError: OpenSSL appears to be unavailable on this machine. OpenSSL is required to
download and install packages.

Exception: HTTPSConnectionPool(host='repo.anaconda.com', port=443): Max retries exceeded with url: /pkgs/main/win-64/current_repodata.json (Caused by SSLError("Can't connect to HTTPS URL because the SSL module is not available."))

then you need to go to your local anaconda3 folder and do the following:

copy libcrypto-1_1-x64.* and libssl-1_1-x64.* from anaconda3>library>bin to ananconda3>dlls

There should be a total of 4 files to be copied.

Exit the command prompot and try again: conda install -p c:\Users\mokas\bostonhousepricing\venv ipykernel --update-deps --force-reinstall

