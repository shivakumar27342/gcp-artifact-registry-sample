# gcp-artifact-registry-sample

### Steps
#### Step 1: Install twine

```bash
    pip3 install -U twine
```

#### Step 2: Build the package
```bash
    python3 -m build
```
The package's distribution files should be located in the **dist** folder

#### Step 3: Upload the package
```bash
    python3 -m twine upload --repository-url <ADD_REPOSITORY_URL_HERE> dist/*
```

#### Step 4: Upload the package

```bash
    pip3 install --index-url <ADD_REPOSITORY_URL_HERE>/simple/ sampleplugin
```