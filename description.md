# Variables Ultra

Variables Ultra | Rebind, Import & Export Variables

English | [Chinese](#Chinese)

**Variables Ultra** is a powerful variable management plugin that implements almost all of the vanilla variable
management functionalities in Figma, but with some differences. We have optimized it based on user feedback and added
several premium features such as `Import/Export`, `Variable Rebinding`, and `Generating Variable Set Templates`, among
others.

## Quick Start

After opening the plugin, create your variable collection.

![home](https://bppleman.blob.core.windows.net/variables-ultra/readme/home.png)

- A brand new, unified UI/UX design
- Place `Collection` in the same viewport to avoid dropdown menus, enabling quick selection
- Click the icon button before the variable name to view/edit details
- More user-friendly options for single selection, multi-selection, and select all
- More intuitive linking of variables (alias), making operations smoother
- Batch modification of multiple variable's scopes

---

## One More Thing

1. [Variable Rebinding](#variable-rebinding)
2. [Import/Export](#import-and-export)
3. [Material3 Specification Templates](#material3-specification-templates)

> Please note, these features require a valid subscription to unlock.

---

### Variable Rebinding

***Want to switch themes?
Modes amount limit?
Use variable sets as your themes to quickly switch different variable
sets for layers, making theme switch effortless.***

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

***This applies to any nested layers and any number of variables. For more usage, please try playground***

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

   Click the export button in the bottom right corner to generate a JSON file containing all the variable sets and
   variables.

2. Import
    1. Switch to `Import/Export` tab and select the JSON file to import.

---

### Material3 Specification Templates

Material3 specification templates are provided to help you quickly set up variables according to the Material3 design
guidelines.

![template_01](https://bppleman.blob.core.windows.net/variables-ultra/readme/template_01.png)

---

# Chinese

**Variables Ultra**
是一款强大的变量管理插件，实现了几乎所有香草的变量管理的功能，但又不完全一样，我们统计了一些样本，专门针对使用体验进行了优化，同时也增加了一些付费功能: `导入/导出`、`变量重绑定`、`生成变量集模板`
等等

## 快速开始

打开插件后，创建你的变量集

![home](https://bppleman.blob.core.windows.net/variables-ultra/readme/home.png)

- 全新且统一设计语言的 UI/UX
- 将 `Collection` 放入同一视口避免使用下拉框，方便快速选择
- 点击变量名前面的图标按钮以查看/编辑详情
- 更人性化的单选、多选、全选
- 更人性化的链接变量（别名），操作更流畅
- 批量修改多个变量的可选范围

---

## One more thing

1. [变量重绑定](#变量重绑定)
2. [导入/导出](#导入和导出)
3. [Material3 规范模版](#Material3规范模版)

> 请注意，这些功能需要一个可用的订阅以解锁

---

### 变量重绑定

***想要切换主题？Mode数量限制？使用变量集作为你的主题，快速为图层切换不同的变量集合，轻松实现主题替换***

为你的设计增加一个不同的主题风格，很简单。

你需要按照以下步骤做一些准备：

1. 准备两个不同名称的变量集，以表示你的不同主题

    1. 创建变量集 `Collection A`，并创建变量 `background`

       ![rebind_var_01](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_01.png)

    2. 创建变量集 `Collection B`，并创建变量 `background`

       ![rebind_var_02](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_02.png)

2. 选择任意一个图层，将它的 Fill 绑定一个变量，比如 `Collection A` - `backgroud`

   ![rebind_var_03](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_03.png)

3. 打开插件，切换到 `Rebind Var` 标签页

    - 在 Source Collection 中选择 `Collection A`

    - 在 Target Collection 中选择 `Collection B`

      ![rebind_var_04](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_04.png)

4. 确保在 figma 中已经选中了红色图层，并按下 `Rebind` 按钮

   最终你会看到图层的 Fill ，重新绑定到 `Collection B` - `backgroud`

   ![rebind_var_05](https://bppleman.blob.core.windows.net/variables-ultra/readme/rebind_var_05.png)

***这适用于任意嵌套的图层，以及任意数量的变量。更多的用法请尝试playground***

> 请注意，`Rebind Var` 无法对以下属性进行重新绑定

- 带有渐变颜色的 Fill
- 对于富文本来说，你只能在以下二选一
    - 将 `String Variable` 绑定到 Text Content
    - 将任意变量绑定到 Text Style 而不是文本内容本身

---

### 导入和导出

我们经常需要将变量应用到多个 figma 文件中，一个一个手动重建将会是一个巨大的工程

但现在有了导入/导出，只需要两个按钮就可以做到

1. 我们准备了一个 `Shared Collection`
    1. `a-background` 链接到 `Collection A` - `backgroud`
    2. `b-background` 链接到 `Collection B` - `backgroud`
    3. `blue` 设置为 `#0000FF`
    4. `blue-alias` 链接到 `blue`
    5. `a-background-alias` 链接到 `a-background`

   ![import_01](https://bppleman.blob.core.windows.net/variables-ultra/readme/import_01.png)

   点击右下角的导出按钮，将会生成一个 json 文件，包含了所有的变量集和变量

2. 导入
    1. 切换到 `Import Var` 标签页，并选择刚才导出的 json 文件
       ![import_02](https://bppleman.blob.core.windows.net/variables-ultra/readme/import_02.png)
    2. 正如我们刚才导出的一样，你会看到所有的变量集和它们的依赖关系
    3. 选择需要导入的变量集，对于有依赖关系的变量集，插件会自动导入依赖的变量集
       ![import_03](https://bppleman.blob.core.windows.net/variables-ultra/readme/import_03.png)
    4. 点击导入按钮，完成操作
       ![import_04](https://bppleman.blob.core.windows.net/variables-ultra/readme/import_04.png)

### Material3规范模版

只需要选择一个种子色，即可生成一个 Material3 规范的变量集

生成多个变量集，即可使用 `Rebind Var` 功能，快速切换主题

![template_01](https://bppleman.blob.core.windows.net/variables-ultra/readme/template_01.png)
