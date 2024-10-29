While you can run the python project directly, poetry also can run it for you without python.

poetry run app

	reference for poetry:

poetry add <python package name>
(add python dependencies to the build. Required every time we add new dependencies)

poetry install
(actually install python dependencies. Run after adding dependencies.)

poetry build
(compiles project to distribution files)

Lazy? Just run:
poetry build; poetry install; poetry run app

ONLY .py FILES ARE EDITABLE. DO NOT EDIT OTHER FILES IN THE CODE DIRECTORY!!!