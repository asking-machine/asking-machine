# Asking-Machine
A Machine that asks questions.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Do you have any questions, machine?" \
  | uvx asking-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install asking-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
asking-machine -a multilogue.txt
```
Or:
```bash
asking-machine multilogue.txt > response.txt
```
Or:
```bash
asking-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import asking_machine
```
