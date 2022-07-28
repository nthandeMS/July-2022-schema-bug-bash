# July-2022-schema-bug-bash

A repository for the schemas used in the July 2022 bug bash.

## Getting Started

The goal of this bug bash is to identify holes in the Azure ML schemas using the Azure ML Visual Studio Code Extension. To get started, you will need to set up a YAML to use the bug bash schemas and set up the VSCode extensioln.

## Validating YAMLs against the bug bash schemas

To validate a YAML against a schema from your local repo, update the `$schema` property at the top of your YAML.
For example, if you want to test a YAML against the Command Job Schema, you would place `$schema: https://azuremlschemasdevelopment.azureedge.net/July-2022-bug-bash/commandJob.schema.json` at the top of your YAML.

Make sure there is only one `$schema` property at the root level of the YAML.

## Using the VSCode Extension

Install the ["Azure Machine Learning" Visual Studio Code extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.vscode-ai) from the extension marketplace.

This extension works with the Azure ML Schemas to provide autocompletion and suggestions to make it easier to create Azure ML objects through YAML files. By setting the `$schema` property above, the extension will use the test schemas to provide suggestions.

Once the extension is active, you can see red underlines for YAML that doesn't match the given schema. You can use `Ctrl + Space` (`Command + Space` on a Mac) to see suggestions and autocomplete for a given property.

## List of Available Schemas

To view a schema or use it in your YAML, append the schema name to this URL format: "<https://azuremlschemasdevelopment.azureedge.net/July-2022-bug-bash/>"

- amlCompute.schema.json
- autoMLClassificationJob.schema.json
- autoMLForecastingJob.schema.json
- autoMLImageClassificationJob.schema.json
- autoMLImageClassificationMultilabelJob.schema.json
- autoMLImageInstanceSegmentationJob.schema.json
- autoMLImageObjectDetectionJob.schema.json
- autoMLJob.schema.json
- autoMLNLPTextClassificationJob.schema.json
- autoMLNLPTextClassificationMultilabelJob.schema.json
- autoMLNLPTextNERJob.schema.json
- autoMLRegressionJob.schema.json
- azureBlob.schema.json
- azureDataLakeGen1.schema.json
- azureDataLakeGen2.schema.json
- azureFile.schema.json
- batchDeployment.schema.json
- batchEndpoint.schema.json
- commandComponent.schema.json
- commandJob.schema.json
- computeInstance.schema.json
- data.schema.json
- environment.schema.json
- kubernetesOnlineDeployment.schema.json
- kubernetesOnlineEndpoint.schema.json
- managedOnlineDeployment.schema.json
- managedOnlineEndpoint.schema.json
- MLTable.schema.json
- model.schema.json
- pipelineJob.schema.json
- sweepJob.schema.json
- vmCompute.schema.json
- workspace.schema.json
