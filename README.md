# README #

### Pathway ###

Usage:
```
#!bash
pathway --csv domain_order.csv student_tests.csv
```

* This tool take the two input CSVs, and produce the learning path for each student.
* 1.0

### Setup ###

The apps was built using python 3.5, after download use the help option like so:

```
#!bash
pathway -h
```
If you see the following you are ready to go!

```
#!bash

usage: pathway [-h] [--csv] student_scores_file domain_priority_file

Calculate Learning Path
positional arguments:
   student_scores_file   a file representioning a list of student scores
   domain_priority_file  a file representing domain priority by grade

optional arguments:
h, --help            show this help message and exit
--csv                input type is CSV (ONLY OPTION Currently)

```


### Testing ###
A Rakefile is include with the project
to run unit test.
To run unit test use the following command:

```
#!bash

rake unit
```
**The rake command requires ruby be installed**

If you don't have ruby you can simply run unit test using the following python commond: 
(*All test were written in python 3.5 environment)*

```python -m unittest discover -f -s test/pathway_service_test -p '*_test.py'"_test.py'"
```