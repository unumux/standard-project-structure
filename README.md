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
|   |-- willow                          # Each library used gets their own folder for overrides
|     |-- _willow.scss                  # Imports files for each component
|
|     |-- primary-nav/                  # Each library component gets their own folder
|       |-- _primary-nav.scss           # Base scss for component and imports for sub-element files
|       |-- _list.scss                  # Styles for list sub-element of the primary-nav
|
|-- theme/                              # For theme styles: base-elements & variables - new and library overrides
| |-- _theme.scss                       # Imports files from each sub-folder
|
| |-- base-elements/                    # Base element styles
|   |-- _base-elements.scss             # styles on element tags
|
| |-- variables/                        # All variables
|   |-- _variables.scss                 # Imports files from each sub-folder
|
|   |-- constants/                      # The starting point for variables
|     |-- _constants.scss               # Imports all files in constants/
|     |-- _colors.scss                  # Defines HEX colors as variables
|     |-- _fonts.scss                   # Imports fonts and sets them equal to font variables
|     |-- _theme-palette.scss           # Assigns priority to each color-palette variable
|     |-- _component-palette.scss       # Assigns theme-palette variables to component parts/pieces - these variables are used in component style files for property values.
|
|   |-- theme-specific/                 # Abstracts the constant variables to more generic variables
|       _theme-specific.scss            # For generic variables like primary-background-color
|
|   |-- component-specific/             # Abstracts the theme-specific variables to apply to specific components
|       _component-name.scss            # Defines variables for a specific component, such as card-background-color
|       _another-component-name.scss    # Each component has a separate file
```

