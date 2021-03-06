## NeatLatex
Neatly compiles PDF of a given latex project (the main document) and then moves the resulting PDF file to ./output and the rest of the intermediate files to ./auxlog

## Options
`-c` : Cleans up the working project directory from all the intermediate aux and log files.

`-b <bib_file>` : Cleans up the references (the .bib file) from "abstrac", "files", "keywords", etc. fields autogenerated by Mendeleys reference management.

`-v` : Verbosity.

## Install
You need super user privileges to install NeatLatex.

run `installer.py` with option `-i` and indicate the directory where you want NeatLatex to be installed.

Example:

`sudo ./installer.py -i /opt/neatlatex`

## Uninstall
run `installer.py` with option `-u`. The script will look for `neatlatex` caller script at `/usr/local/bin/` and sort out the rest from there.

`sudo ./installer.py -u` 

## Usage
### To compile a PDF for a latex project with the main document named as "main.tex": 

`neatlatex main`

### To clean up the reference file named as "refs.bib" auto-generated by Mendeley:

`neatlatex main -b refs.bib`

### To clean up the intermediate aux and log files from the working project directory without compiling the project:

`neatlatex main -c`

