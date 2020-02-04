# KrypApp
File Encryption GUI App with Python

![Screenshot](https://raw.githubusercontent.com/ahmednooor/KrypApp/master/screenshot.png)

### Tech Stack
* Python 3
* Tkinter for GUI
* pycryptodomex for Cryptodome
* AES Encryption
* cx_freeze to build executable

### External Dependencies
* `pycryptodomex` for AES encryption.
```sh
pip install pycryptodomex
```

* `cx_freeze` to build executable.
```sh
pip install cx_freeze
```

### To Build Executable
* Open `setup.py` and replace `<path/to/your/python_directory>` with your python installation directory.
* Open Terminal in directory where `setup.py` is; and type,
```sh
python setup.py build
```
> Executable files will be created in the `build` directory.
> Build tested on `Windows 10 Pro (1903)`

### How to Encrypt/Decrypt
1. Open the App and Click SELECT FILE Button and select your file e.g. "abc.jpg".
2. Enter your Secret Key (This can be any alphanumeric letters). Remember this so you can Decrypt the file later.
3. Click ENCRYPT Button to encrypt. A new encrypted file with ".kryp" extention e.g. "abc.jpg.kryp" will be created in the same directory where the "abc.jpg" is.
4. When you want to Decrypt a file you, will select the file with the ".kryp" extention and Enter your Secret Key which you chose at the time of Encryption. Click DECRYPT Button to decrypt. The decrypted file will be of the same name as before with the suffix "__dekrypted__" e.g. "abc__dekrypted__.jpg".
5. Click RESET Button to reset the input fields and status bar.
6. You can also Click CANCEL Button during Encryption/Decryption to stop the process.
> Tested on `Windows 10 Pro (1903)`

### Credits
> `EncryptionTool` class from [`nsk89`](https://github.com/nsk89) for file encryption.
> `flaticon.com` for icon file.
