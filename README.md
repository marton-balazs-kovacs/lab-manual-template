# lab-manual-template

## Introduction

Lab manuals are effective tools for recording who we are and how we do things in a research laboratory. This repository contains a JSON schema for storing information of lab manuals in a machine- and human-readable format. The repository also contains the lab manual template that has been developed to aid researchers to create their own manuals by providing a general topics that could be included in lab manuals in a structured format and boilerplate texts for certain topics. The [bluerint](https://github.com/mjaquiery/lab-manual) webapp provides an easy-to-use interface to edit the lab manual template to create your own lab manual or other lab manual templates.

## Project structure

The lab manual JSON schema can be found in the `lab-manual-template-schema.json` file. Our general purpose lab manual template is in the `lab-manual-template.json` file, while the `lab-manual-template.docx` file contains a rendered version. The `templates.json` file contains meta-information on the lab manual templates formatted according our schema and available through the `blueprint` app.

## Contributions

If you would like to submit your own lab manual template to help others from a specific institution or research field to create their own manual more easily you can submit your template formatted to our JSON schema. To submit a new template please supplement the `templates.json` file with a new object formatted the following way and create a pull request:

```
{
  "title": "Human readable name of the template",
  "template": "URL to the raw json file containing the template",
  "usecase": "Short description of who is the target audiance of the template"
}
```

If you used our lab manual template to write your own lab manual and you shared the resulting document publicly, please consider adding the manual to our collection of lab manuals in the `manuals.json` file. To do so please use the following format:

```
{
	"link": "Link to the openly shared lab manual.",
	"pi": "Name of the PI of the lab.",
	"name": "Name of the lab."
}
```
