# gatorgrade-action

This GitHub Action runs GatorGrade.

## Usage

Basic workflow to run GatorGrade on every push to GitHub:

'''
name: Grader
on: [push]
jobs:
    grade:
        run-on: ubuntu-latest
        steps:
            - name: Checkout repository
                uses: actions/checkout@v2
            - name: Run Gatorgrade
                uses: GatorEducator/gatorgrade-action@v1
'''