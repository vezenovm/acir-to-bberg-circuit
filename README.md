# ACIR to bb.js circuit

Convert an ACIR circuit generated by Noir.

How to use the repo:

1. Install the binary using the command below
```
cargo install --path=.
```

2. Then enter your Noir project directory

3. Compile a circuit using nargo. 
```
nargo compile test
```

4. Then run the command below
```
acir-to-bberg-circuit <path_to_nargo_compile_output>
```

The default path will be `./target/main.json`, and it will change the JSON file directly. It should be noted that it will also overwrite the proving key and verification key to be empty if exist in the original build artifact.