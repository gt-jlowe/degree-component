# Degree Component (Paragraph) Recipe

## Description

This Drupal recipe adds a "Degree" Paragraph type. It is designed to be used for things like academic history on a profile, providing fields for the degree name, institution, year, and more.

This recipe configures the "Degree" paragraph to use Inline Entity Form for a better content editing experience.

## Features

* Creates a new Paragraphs type with the machine name `degree` and label "Degree".
* Adds the following fields to the "Degree" paragraph:
    * **Degree** (`field_degree`) - Text (String)
    * **Institution** (`field_institution`) - Text (String)
    * **Year** (`field_year`) - Text (String)
    * **Location** (`field_location`) - Text (String)
    * **Honors** (`field_honors`) - Text (String)
    * **Honorary** (`field_honorary`) - Boolean
* Configures the default entity form display for the `degree` paragraph.
* Configures the default entity view display for the `degree` paragraph.

## Requirements

This recipe requires the following modules:

* **Paragraphs** (`drupal/paragraphs`)
* **Inline Entity Form** (`drupal/inline_entity_form`)
* **Entity Reference Revisions** (`drupal/entity_reference_revisions`)

## Installation

1.  Ensure all required modules (listed above) are installed and enabled.
2.  Place this recipe in your site's `/recipes` directory (e.g., `/recipes/custom/degree_component`).
3.  Apply the recipe using Drush:
    ```bash
    drush recipe apply degree_component
    ```
    (Replace `degree_component` with the actual directory name if different).
4.  Alternatively, apply the recipe from the Drupal admin UI at `/admin/config/development/recipes`.
