# Jarvis Resume Builder

## Introduction

Jarvis Resume Builder is a bash utility tool that converts your markdown resume into PDF. This utility requires docker. 

## Quick Start 

Please follow the steps below to setup this tool in your Github repo. 

```
#cd to your Github repo parent directory
cd jarvis_data_eng_NAME

#make sure docker engine is started
docker info

#switch to the feature branch
git checkout feature/resume

#init resume
mkdir resume && cd resume && wget https://raw.githubusercontent.com/jarviscanada/jarvis_resume_builder/master/gen_resume.sh -O gen_resume.sh && bash gen_resume.sh init

#you should have the following files
cd jarvis_data_eng_NAME
ls README.md resume/gen_resume.sh resume/resume.pdf
```

## Usage

Note: `gen_resume.sh` will remove all markdown quotes (e.g. lines start with `>`) when generating the PDF file. 

```
#Update jarvis_data_eng_NAME/README.md

#generate a new PDF version
./resume/gen_resume.sh

#verify resume/resume.pdf
```

## Resume Style

If you have setsup the resume build in your Github, the resume style requirements are documented in the top level `README.md`. For your reference, [resume_template.md](./resume_template.md) is the original template document.
