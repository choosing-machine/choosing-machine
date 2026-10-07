# Choosing-Machine
A machine that chooses.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: What would be your choice, machine?" \
  | uvx choosing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install choosing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
choosing-machine -a multilogue.txt
```
Or:
```bash
choosing-machine multilogue.txt > response.txt
```
Or:
```bash
choosing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import choosing_machine
```
