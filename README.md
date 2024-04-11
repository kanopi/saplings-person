# Saplings-Person Repository

## Overview

Welcome to the Saplings-Person repository, the central hub for managing everything Person within the Saplings application. Saplings-Person handles the Person content type, Person taxonomies, Person views, and Person schema. This repository coordinates with several sub-repositories to handle different aspects of content creation and management.

## Sub-Repositories:

1. **[kanopi/saplings-content-base](https://github.com/kanopi/saplings-content-base)**
   - Contains base fields and configurations for all content types in Saplings.

   a. **[kanopi/saplings-media](https://github.com/kanopi/saplings-media)**
      - Handles Media entities and implements best practices configurations.
         - **[kanopi/imagemagick-configuration](https://github.com/kanopi/imagemagick-configuration)**
            - Configuration files for Imagemagick integration within Saplings.

   b. **[kanopi/saplings-theme](https://github.com/kanopi/saplings-theme)**
      - Configures the UI Patterns Suite, including modules and themes.
         - **[kanopi/saplings_child](https://github.com/kanopi/saplings_child) [Theme]**
            - Custom base theme, a child of the Ui Suite Bootstrap Contrib theme.
              
   c. **[kanopi/saplings_custom](https://github.com/kanopi/saplings_custom) [Module]**
            - Contributed module with utility commands.

2. **[kanopi/saplings-content-types](https://github.com/kanopi/saplings-content-types)**
   - Handles content types.
  
## Patches

smart_date may throw an error that looks like this:
```
* 		User deprecated function: Passing a string to Drupal\options\Plugin\Field\FieldType\ListItemBase::extractAllowedValues() is deprecated in drupal:10.2.0 and will cause an error from drupal:11.0.0. Use an array instead. See https://www.drupal.org/node/3376368 in Drupal\options\Plugin\Field\FieldType\ListItemBase::extractAllowedValues() (line 406 of core/modules/options/src/Plugin/Field/FieldType/ListItemBase.php).
```
To fix this, you can apply [this patch](https://www.drupal.org/project/smart_date/issues/3409287)