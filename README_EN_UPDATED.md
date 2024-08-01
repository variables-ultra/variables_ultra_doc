# Variables Ultra

Variables Ultra | Rebind, Import & Export Variables

**Variables Ultra** is a powerful variable management plugin that implements almost all of the native variable management functionalities in Figma, but with some differences. We have optimized it based on user feedback and added several premium features such as `Import/Export`, `Variable Rebinding`, and `Generating Variable Set Templates`, among others.

## Quick Start

After opening the plugin, create your variable set.

![home](https://bppleman.blob.core.windows.net/variables-ultra/readme/home.png)

- A brand new, unified UI/UX design
- Place `Collections` in the same viewport to avoid dropdown menus, enabling quick selection
- Click the icon button next to the variable name to view/edit details
- More user-friendly options for single selection, multi-selection, and select all
- More intuitive linking of variables (aliases), making operations smoother
- Batch modification of multiple variables' scopes

---

## One More Thing

1. [Variable Rebinding](#variable-rebinding)
2. [Import/Export](#import-and-export)
3. [Material3 Specification Templates](#material3-specification-templates)

> Please note, these features require a valid subscription to unlock.

---

### Variable Rebinding

***Want to switch themes? Running out of modes? Use variable sets as your themes to quickly switch different variable sets for layers, making theme changes effortless.***

Follow these steps to prepare:

1. Prepare two variable sets with different names to represent your different themes.

    1. Create a variable set `Collection A` and create a variable `background`.

       ![rebind_var_01](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_01.png)

    2. Create a variable set `Collection B` and create a variable `background`.

       ![rebind_var_02](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_02.png)

2. Select any layer and bind its Fill to a variable.

   ![rebind_var_03](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_03.png)

3. Open the plugin and switch to the `Rebind Var` tab.

   Select `Collection A` in the Source and `Collection B` in the Target.

4. Ensure the red layer is selected in Figma and press the `Rebind` button.

   You will see the layer's Fill rebind to `Collection B - background`.

   ![rebind_var_05](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_05.png)

***This applies to any nested layers and any number of variables.***

> Please note, `Rebind Var` cannot rebind the following attributes:

- Fill with gradient colors
- For rich text, you can only choose one of the following:
    - Bind `String Variable` to Text Content
    - Bind any variable to Text Style instead of the text content itself

---

### Import and Export

We often need to apply variables to multiple Figma files, and manually recreating them one by one can be a massive task.

1. We have prepared a `Shared Collection`:
    1. `a-background` links to `Collection A - background`
    2. `b-background` links to `Collection B - background`
    3. `blue` is set to `#0000FF`
    4. `blue-alias` links to `blue`
    5. `a-background-alias` links to `a-background`

   ![import_01](https://bppleman.blob.core.windows.net/variables-ultra/readme/import_01.png)

   Click the export button in the bottom right corner to generate a JSON file containing all the variable sets and variables.

2. Import
    1. Switch to `Import/Export` tab and select the JSON file to import.

---

### Material3 Specification Templates

Material3 specification templates are provided to help you quickly set up variables according to the Material3 design guidelines.

---
