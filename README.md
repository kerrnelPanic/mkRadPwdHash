# mkRadPwdHash
A simple python class and cli tool to generate salted password-hashes for FreeRadius.

### How it works

    python3 mkradpasswd>mkRadPwdHash.py -a sha512
    Enter your password:
    Enter your password again:
    SSHA2-384-Password := "/syZi0m+fnK/BPh9yrFY85gOaiMCeycQt3AmI0DxoKRUmNBTxcoGIa7odiRavKWB31zVzDZVmaYyzZWrZyH96w=="
    
Copy and paste output line to yout FreeRadius config with the username as prefix:

    user SSHA2-384-Password := "/syZi0m+fnK/BPh9yrFY85gOaiMCeycQt3AmI0DxoKRUmNBTxcoGIa7odiRavKWB31zVzDZVmaYyzZWrZyH96w=="
