## **Variables Ultra | Management, Rebind, Import & Export, Templates**

Variables Ultra is a powerful variable management plugin that implements almost all of the vanilla variable management functionalities in Figma, but with some differences.

We have optimized it based on user feedback and added several extra features such as `Import/Export`, `Variable Rebinding`, and `Generating Variable Set Templates`, among others. **All features are free. No account or sign-in is needed.**

## ⚡️ Quick Start

After opening the plugin, create your variable collection.

- A brand new, unified UI/UX design
- Place `Collection` in the same viewport to avoid dropdown menus, enabling quick selection
- Click the icon button before the variable name to view/edit details
- More user-friendly options for single selection, multi-selection, and select all
- More intuitive linking of variables (alias), making operations smoother
- Batch modification of multiple variables' scopes

---

## One More Thing

- [Variable Rebinding]
- [Import/Export]
- [Material3 Specification Templates]

All of these features are free.

---

## Variable Rebinding

**Want to switch themes?**

**Modes amount limit?**

**Use variable sets as your themes to quickly switch different variable sets for layers, making theme switch effortless.**

Follow these steps to prepare:

1. Prepare two variable sets with different names to represent your different themes.
2. Create a variable set `Collection A` and create a variable `background`.
3. Create a variable set `Collection B` and create a variable `background`.
4. Select any layer and bind its Fill to `Collection A - background`.
5. Open the plugin and switch to the `Rebind Var` tab.
6. Choose the scope: `Selection`, `Current Page` or `All Pages`.
7. Select `Collection A` in the Source and `Collection B` in the Target.
8. Make sure the layer is selected in Figma and press the rebind button in the bottom right corner.
9. You will see the layer's Fill rebind to `Collection B - background`.

**This applies to any nested layers and any number of variables.** Variables are matched by name, and variable sets from enabled team libraries are supported too.

Please note, `Rebind Var` cannot rebind the following:

- Fills set to `Mixed`
- Text layers that bind a `String Variable` to the text content and also bind variables on several text ranges: only the text content is rebound, and the per-range text styles are skipped

Anything that can't be rebound is listed in the `Conflict View`.

---

## Import and Export

We often need to apply variables to multiple Figma files, and manually recreating them one by one can be a massive task.

We have prepared a `Shared Collection`:

- `a-background` links to `Collection A - background`
- `b-background` links to `Collection B - background`
- `blue` is set to `#0000FF`
- `blue-alias` links to `blue`
- `a-background-alias` links to `a-background`

**1. Export**

On the `Variables` tab, click the save button in the bottom right corner to generate a JSON file containing all the variable sets and variables, including the aliases between them.

**2. Import**

1. Switch to the `Import Var` tab and select the JSON file you just exported.
2. You will see all the variable sets and their dependencies.
3. Select the variable sets to import. The variable sets they depend on are imported automatically.
4. Press the import button to finish.

---

## Material3 Specification Templates

Material3 specification templates are provided to help you quickly set up variables according to the Material3 design guidelines.

Pick a seed color to generate a variable set with four modes: `Dark`, `Light`, `Light Medium Contrast` and `Light High Contrast`. You can create a new variable set, or update or merge into an existing one. Generate several variable sets, then use `Rebind Var` to switch themes quickly.

---

Variables Ultra 是一款强大的变量管理插件，实现了 Figma 自带变量管理的几乎所有功能，但又不完全一样。我们统计了一些样本，专门针对使用体验进行了优化，同时也增加了一些额外功能：导入/导出、变量重绑定、生成变量集模板等等。**所有功能免费，不需要注册或登录。**

## ⚡️ 快速开始

打开插件后，创建你的变量集。

- 全新且统一设计语言的 UI/UX
- 将 `Collection` 放入同一视口，避免使用下拉框，方便快速选择
- 点击变量名前面的图标按钮以查看/编辑详情
- 更人性化的单选、多选、全选
- 更人性化的链接变量（别名），操作更流畅
- 批量修改多个变量的作用范围

---

## One more thing

- [变量重绑定]
- [导入/导出]
- [Material3 规范模板]

这些功能全部免费。

---

## 变量重绑定

**想要切换主题？Mode 数量限制？使用变量集作为你的主题，快速为图层切换不同的变量集合，轻松实现主题替换。**

为你的设计增加一个不同的主题风格，很简单。

你需要按照以下步骤做一些准备：

1. 准备两个不同名称的变量集，以表示你的不同主题
2. 创建变量集 `Collection A`，并创建变量 `background`
3. 创建变量集 `Collection B`，并创建变量 `background`
4. 选择任意一个图层，将它的 Fill 绑定到 `Collection A - background`
5. 打开插件，切换到 `Rebind Var` 标签页
6. 选择范围：`Selection`（选中的图层）、`Current Page`（当前页）或 `All Pages`（所有页）
7. 在 `Source Collection` 中选择 `Collection A`
8. 在 `Target Collection` 中选择 `Collection B`
9. 确保在 Figma 中已经选中了这个图层，并按下右下角的重绑定按钮

最终你会看到图层的 Fill 重新绑定到 `Collection B - background`。

**这适用于任意嵌套的图层，以及任意数量的变量。** 变量按名称匹配，也支持已启用的团队库里的变量集。

请注意，`Rebind Var` 无法重新绑定以下内容：

- 值为 `Mixed` 的 Fill
- 如果一个文本图层既把 `String Variable` 绑定到了文本内容，又在多个文本片段上分别绑定了变量，只会重绑定文本内容，各片段的文字样式会被跳过

无法重绑定的内容会列在 `Conflict View` 里。

---

## 导入和导出

我们经常需要将变量应用到多个 Figma 文件中，一个一个手动重建将会是一个巨大的工程。但现在有了导入/导出，只需要两个按钮就可以做到。

让我们准备一个 `Shared Collection`：

- `a-background` 链接到 `Collection A - background`
- `b-background` 链接到 `Collection B - background`
- `blue` 设置为 `#0000FF`
- `blue-alias` 链接到 `blue`
- `a-background-alias` 链接到 `a-background`

**1. 导出**

在 `Variables` 标签页点击右下角的保存按钮，将会生成一个 json 文件，包含了所有的变量集和变量，以及它们之间的别名关系。

**2. 导入**

1. 切换到 `Import Var` 标签页，并选择刚才导出的 json 文件
2. 正如我们刚才导出的一样，你会看到所有的变量集和它们的依赖关系
3. 选择需要导入的变量集，对于有依赖关系的变量集，插件会自动导入依赖的变量集
4. 点击导入按钮，完成操作

---

## Material3 规范模板

只需要选择一个种子色，即可生成一个 Material3 规范的变量集，包含 `Dark`、`Light`、`Light Medium Contrast`、`Light High Contrast` 四个 mode。可以新建变量集，也可以更新或合并到已有的变量集。

生成多个变量集，即可使用 `Rebind Var` 功能，快速切换主题。
