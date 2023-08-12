# QiHe-Portfolio

将colab编译的html文件导出至github的整个流程：

1. **在Colab生成HTML文件**：
    - 使用Python代码在Colab中生成HTML文件。例如，使用一些数据可视化库生成图表，并将其保存为HTML格式。

2. **从Colab上传HTML到GitHub**：（这样能够允许colab生成的html文件在github上实时更新）
    - 生成GitHub Token：进入GitHub设置 > Developer settings > Personal access tokens。（创建一个新的Token，确保至少选择了repo权限）
    - 先克隆GitHub仓库到Colab环境。（包括复制的token）
    - 将生成的HTML文件复制或移动到克隆的仓库目录中。
    - 提交这个HTML文件到仓库，并推送这些更改回GitHub。

3. **在GitHub上设置GitHub Pages**：（设置 GitHub Pages 主要是为了能够将静态文件（例如 HTML、CSS、JavaScript 文件等）渲染为一个可访问的在线网站，而不是源代码。）
    - 进入仓库的设置部分。
    - 找到GitHub Pages部分。
    - 选择一个源分支或目录。如果您直接在`main`或`master`分支上工作，那么选择该分支。
    - 选择一个目录。如果您直接在仓库的根目录上放置`index.html`，那么选择“root”。如果在一个叫`docs`的子目录里，那么选择“docs”。
    - 保存设置。

4. **获取页面链接**：
    - 在GitHub Pages设置部分，系统通常会给出一个链接，这个链接即为您的渲染后的HTML页面。链接通常的格式为：`https://[your_username].github.io/[repository_name]/`。
    - 由于`index.html`是默认的起始页面，所以您可以直接使用目录URL来访问它。

5. **分享链接**：
    - 一旦GitHub Pages构建成功（通常在几分钟内完成），您可以直接分享之前获取的链接，其他人就可以在浏览器中看到您渲染的HTML页面了。

如果有疑问可以一起讨论！
