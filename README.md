To build the paper run the command: `make <target>`. After that pdf will appear in the `<repo_root>/build` folder.
Targets:
* `clean` - clear the `build` folder
* `texfirst` builds the initial version of pdf without references and generate metadata to perform the next steps
* `refs` runs bibtex to build intermediate representation of references according to metadata generated on the previous step
* `texsecond` run pdflatex again to build the final version of paper
* `all` runs consequently `texfirst`, `refs` and `texsecond` targets, thus building the whole document
* `release` runs `clean` then builds `all` and copies pdf to the repo root folder. Can be used for generating ready-to-commit document
