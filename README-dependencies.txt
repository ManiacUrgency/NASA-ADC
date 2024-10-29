poetry allows us to build python into an inter-computer form so that the compiled code can be run on any computer.
However, poetry must be installed.

	MACOS: Poetry < Pipx < Brew

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install pipx

pipx ensurepath
sudo pipx ensurepath --global
pipx install poetry

	WINDOWS: Poetry < Pipx < Scoop

(using PowerShell)
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression

scoop install pipx

pipx ensurepath
pipx install poetry

	WINDOWS: Pipx < pip < python3 / python / py

(find the one that works of the three)
py -m pip install --user pipx
python -m pip install --user pipx
python3 -m pip install --user pipx

pipx ensurepath
pipx install poetry


