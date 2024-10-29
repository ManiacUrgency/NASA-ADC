# NASA-ADC
NASA ADC challenge

## Running the app
While you can run the python project directly, Poetry also can run it for you without python.
```
poetry run app
```
## Poetry & Development
Poetry turns python into a sort of java where there exists an intermediate tarball/wheel file that can be executed on any machine so long as you have Poetry.

Lazy? Just run:
```
poetry build; poetry install; poetry run app
```
### Actual Poetry documentation
```
poetry add <python package name>
```
- add python dependencies to the build. Required every time we add new dependencies

```
poetry install
```
- actually install python dependencies. Run after adding dependencies.

```
poetry build
```
- compiles project to distribution files

**ONLY `.py` FILES ARE EDITABLE. DO NOT EDIT OTHER FILES IN THE CODE DIRECTORY!!!**


## Dependencies
poetry allows us to build python into an inter-computer form so that the compiled code can be run on any computer.
However, poetry must be installed.

### MACOS
Dependency chain: `Poetry < Pipx < Brew`
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install pipx

pipx ensurepath
sudo pipx ensurepath --global
pipx install poetry
```
### WINDOWS
Dependency chain: `Poetry < Pipx < Scoop`

(using PowerShell)
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression

scoop install pipx

pipx ensurepath
pipx install poetry
```

### WINDOWS alt
Dependency chain: `Pipx < pip < python3 / python / py`

(find the one that works of the top three)
```
py -m pip install --user pipx
python -m pip install --user pipx
python3 -m pip install --user pipx
```
and then:
```
pipx ensurepath
pipx install poetry
```

README written with [Online Github Markdown Editor](https://jbt.github.io/markdown-editor/) by jbt
