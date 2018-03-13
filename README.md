# Swagger UI Field Formatter

## Credits
This module was forked by UC Santa Barbara from https://www.drupal.org/project/swagger_ui_formatter.

## Introduction

This module provides a field formatter for file fields which renders the uploaded json or yaml file using the Swagger UI. This module uses the
[Swagger UI Library](https://github.com/swagger-api/swagger-ui) using [UNPKG](https://unpkg.com) to load the js and css.

## Requirements

This file entity module is required to allow for upload of json or yaml files.

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
- On the Manage display tab, for the file field set Label to `<Hidden>` and Format to `Swagger UI Formatter`. Click Save then click Update.
- Click gear button on the right. Good options are Doc Expansion=List, and Show Request Headers=checked. Click Update.

## Usage

Create new content of the type you created. Upload a swagger/openAPI file.

You can see that the uploaded swagger file is rendered using the Swagger UI.
