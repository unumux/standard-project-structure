# standard-project-structure

```
styles/
|-- _styles.scss                        # Imports files from components/ and theme/
|
|-- components/                         # For component related styles
| |-- _components.scss                  # Imports files from each component folder
|
| |-- my-component/                     # Project components get their own folders
|   |-- _my-component.scss              # Base scss for component and imports sub-element files
|   |-- _sub-element-1.scss             # Styles for a specific sub-element
|   |-- _sub-element-2.scss
|
| |-- overrides                         # For overriding component styles from external libraries - willow, bootstrap
|   |-- _overrides.scss                 # Imports files from each library folder
|
|   |-- willow                          # Each library used gets their own folder for their overrides
|     |-- _willow.scss                  # Imports files for each component
|
|     |-- primary-nav/                  # Each library component gets their own folder
|       |-- _primary-nav.scss           # Base scss for component and imports for sub-element files
|       |-- _list.scss                  # Styles for list sub-element of the primary-nav
|
|-- theme/                              # For theme styles: base-elements & variables - new and library overrides
| |-- _theme.scss                       # Imports files from each sub-folder
|
| |-- base-elements/                    # Base element and normalizing styles
|   |-- _base-elements.scss             # HTML tag styles
|   |-- _normalize.scss                 # Normalize file - name any files like this after the source library
|
| |-- variables/                        # All variables
|   |-- _variables.scss                 # Imports files from each sub-folder
|
|   |-- colors/                         # Color specific variables
|     |-- _colors.scss                  # Imports palette files
|     |-- _color-palette.scss           # Defines HEX colors as variables
|     |-- _theme-palette.scss           # Assigns priority to each color-palette variable
|     |-- _component-palette.scss       # Assigns theme-palette variables to component parts/pieces - these variables are used in component style files for property values.
|
|   |-- fonts/                          # Font specific variables
|       _font-variables.scss            # Defines font families and variables for groups of font specific properties
|
|   |-- sizing/                         # Sizing specific variables
|       _sizing-variables.scss          # Defines padding, margin, border, etc. variables
```

