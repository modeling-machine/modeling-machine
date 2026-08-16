# Modeling-Machine
A machine that creates semantic models.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: What is the semantic model of it, machine?" \
  | uvx modeling-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install modeling-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
modeling-machine -a multilogue.txt
```
Or:
```bash
modeling-machine multilogue.txt > response.txt
```
Or:
```bash
modeling-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import modeling_machine
```
