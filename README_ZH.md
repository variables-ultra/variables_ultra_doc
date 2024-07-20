# Variables Ultra

Variables Ultra | Rebind, Import & Export Variables

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
- 批量修改多个变量的 scopes

---

## One more thing

1. [变量重绑定](#变量重绑定)
2. [导入/导出](#导入和导出)
3. [Material3 规范模版](#Material3规范模版)

> 请注意，这些功能需要一个可用的订阅以解锁

---

### 变量重绑定

***想要切换主题？Mode不够用？使用变量集作为你的主题，快速为图层切换不同的变量集合，轻松实现主题替换***

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

***这适用于任意嵌套的图层，以及任意数量的变量***

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

### Material3 规范模版

* 想生成一个新的M3变量集？
    1. 输入一个种子色，点击【Generate Variables】
    2. 选择【Create】选项并输入名称，即可生成变量集
* 想将现有蓝色主题风格变量集A修改为绿色主题怎么办？
    1. 输入色值，点击【Generate Variables】
    2. 选择【Update】选项，并选择变量集A，即可将现有变量更新为新的主题色
* 已有一个红色主题变量集R，删去了tertiary相关的变量，现在想要新建tertiary相关的变量，如何快速实现？
    1. 输入色值，点击【Generate Variables】
    2. 选择【Merge】选项，并选择变量集R，被删去的变量将会被重新添加到集合R中

如果你遇到错误，或者有功能请求，请到github上
