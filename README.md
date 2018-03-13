# Swagger UI Field Formatter

## Introduction

This module provides a field formatter for file fields with allowed file types
as json or yml, which renders the uploaded json or yml file using the Swagger UI
if the uploaded json or yml file is a valid swagger file. This module uses the
Swagger UI Library available at https://github.com/swagger-api/swagger-ui

## Requirements

This module does not have any special requirements. However in order to be able
to allow json or yml file extensions in Drupal, you might need to install the
file entity module.

## Installation

- Extract it into your sites/all/modules/contrib. 
- Login as adminstrator.
- Go to admin/modules and enable Swagger UI Field Formatter.

## Configuration

Create a new Content Type


- Go to admin/structure/types (Add Content Type)
- Create Content Type with the name of your choosing. Click Save and add fields.
- Delete Body field, add File field with a name of your choosing. Click Save.
- On the Edit tab set allowed file extensions to `json, yaml, yml`.
- Set a File directory of your choosing. Save settings.
- On the Manage display tab, for the file field set Label to `<Hidden>` and the Format to `Swagger UI Formatter`. Click Save.
- Click gear button on the right. Good options are Doc Expansion=List, and Show Request Headers=checked. Click Update.

## Usage
Create new content of the type you created. Upload a swagger/openAPI file.

You can see that the uploaded swagger file is rendered using the Swagger UI.
