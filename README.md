# pkgexample

Last updated 28th August 2022

Welcome to the readme for this simple package.
More information [Click Here](##Introduction)

## Introduction

This is a README file for the RexBytes simple example.
It's created using Github-flavoured Markdown, you can 
create a README for your project, for more information 
[Click Here](https://guides.github.com/features/mastering-markdown/)

## Build Instructions

A full detailed instruction on python package building [is available here](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
You should read it in full to understand the following overview of the process.

Here we use the "setuptools" build system, others are availble ("Hatching","Flit", and "PDM") in the guide linked above.

In short, these are the steps.

### (1/4) Create the following files in your project root directory,
   
   - README.md
   - LICENCE
   - pyproject.toml

### (2/4) Build a PyPi release. 

   From the root of your project directory, run the following command,

   python3 -m build

   This command will create a ./dist/ directory containing your distribution files.

### (3/4) Check your distribution files.

   You should really check your distribution files for errors before submitting them to pypi.org
   Run the following command from the root of you project directory to do so.

   python3 -m twine check ./dist/*

### (4/4) Upload your fresh package to pypi

   If your packages passed the checks you can upload them to your pypi.org repository.
   Run the following command from the root of your project directory to do so.

   python3 -m twine upload ./dist/* 

   You will be asked for your pypi user name and password.

## Enjoy!

Have fun packaging python!
