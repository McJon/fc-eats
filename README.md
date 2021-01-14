# Northern x Fanshawe Shopify Course

## Prerequisites
- Bash CLI
- [Docker](https://docs.docker.com/install/)
- [GitHub Account](https://github.com/)
- IDE

## Downloading the Theme

In the project, run the following to download the theme from your Shopify store using Theme Kit:

```console
$ chmod +x theme
$ ./theme get --list -p=[your-password] -s=[your-store.myshopify.com]
$ ./theme get -p=[your-password] -s=[your-store.myshopify.com] -t=[your-theme-id]
```

The password can be obtained by creating a private app in your Shopify store [[gif]](https://shopify.github.io/themekit/assets/images/shopify-local-theme-development-generate-api.gif). The theme ID can be obtained from the `./theme get --list` command.

Full instructions can be found [[here]](https://shopify.github.io/themekit/#configure-an-existing-theme).

## Using Theme Kit

Theme Kit can be run using the `./theme` script in the project's root directory. A full list of commands can be found [[here]](https://shopify.github.io/themekit/commands/).

#### 4 Ways to Get Your Theme ID
1. From the URL
   - Go to your-store.myshopify.com/admin/themes select "Edit Code" from the "Actions" dropdown next to the theme
   - The ID should be in the URL of this page
   - e.g. your-store.myshopify.com/admin/themes/**80643031095**
2. your-store.myshopify.com/admin/themes.xml
3. your-store.myshopify.com/admin/themes.json
4. ./theme get --list -p=[your-password] -s=[your-store.myshopify.com]

## Setting up a GitHub account
For this course, you are required to set up and maintain your own GitHub account and repository for your project.

Here are a few links to get you started:
- [Adding a new SSH key to your GitHub account](https://help.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)
- [Adding an existing project to GitHub using the command line](https://help.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line)

## Setting up an IDE
The course lectures and workshops will be demoed using the VSCode IDE, but you are free to use any editor that you are comfortable with. Recommended extension are outlined below.

To maintain consistent coding styles across various editors and IDEs, we have included an [`.editorconfig`](https://editorconfig.org/) file. Be sure to install an EditorConfig extension on your IDE.

**VS Code**
- [The 20 Best Visual Studio Code Extensions for Front End Developers](https://www.shopify.ca/partners/blog/best-visual-studio-code-extensions)
- At the very least, it is recommend to install the following extensions:
   - [Liquid Languages Support](https://marketplace.visualstudio.com/items?itemName=neilding.language-liquid)
   - [Shopify Liquid Snippets](https://marketplace.visualstudio.com/items?itemName=killalau.vscode-liquid-snippets)
   - [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

#### Configure File Associations
- Update `settings.json` by searching for `Preferences: Open Settings (JSON)` and add the following:
```
"files.associations": {
  "*.liquid": "liquid",
  "*.scss.liquid": "scss",
  "*.js.liquid": "javascript"
},
```
