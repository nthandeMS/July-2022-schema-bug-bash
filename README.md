# July-2022-schema-bug-bash
A repository for the schemas used in the July 2022 bug bash.

## Getting Started

 Clone the repo to your computer using `git clone https://github.com/nthandeMS/July-2022-schema-bug-bash.git`.

## Setting up a Schema Test File

To validate a YAML against a schema from your local repo, you will need to update the `$schema` property at the top of your YAML.
For example, if you want to test a YAML against the Command Job Schema, you would place `$schema: file:C:\<path-to-July-2022-schema-bug-bash>\schema\commandJob.schema.json` at the top of your YAML.

Make sure there is only one `$schema` property at the root level of the YAML.

## Using the Visual Studio Code Extension

Install the "Azure Machine Learning" Visual Studio Code extension from the extension marketplace:

This extension works with the Azure ML Schemas to provide autocompletion and suggestions to make it easier to create Azure ML objects through YAML files. By setting the `$schema` property above, the extension will use the test schemas instead of the latest publicly available version.

Once the extension is active, you can see red underlines for YAML that doesn't match the given schema. You can use `Ctrl + Space` (`Command + Space` on a Mac) to see suggestions and autocomplete for a given property.


