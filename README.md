Scaffold repository for custom templates for Harold.

Use it with [create-harold-app](https://github.com/harold-js/create-harold-app)

You must pass the path to a zip or tar file with the template to use your custom template. In this case, it would be:

```
npm init harold-app@latest my-app -t https://github.com/harold-js/harold-template-scaffold/archive/refs/heads/main.zip
```

with npm 7+
```
npm init harold-app@latest my-app -- -t https://github.com/harold-js/harold-template-scaffold/archive/refs/heads/main.zip
```

For now, Harold supports remote and local paths to archive files. So you need to point the archive file directly.

The structure of your template archive should look like this:

```
// my-custom-template.zip file:

my-custom-template-name-directory
  |- assets // optional
  |- blog-layouts
  |- pages
  |- partials
  |- posts
  |- styles
  |- .gitignore // optional
  |- .haroldrc // optional
```

All custom templates should start with a similar file and directories structure. You can also check examples of ready-to-use templates:

- [Default Template repository](https://github.com/harold-js/harold-template-default)
- [Docs Template repository](https://github.com/harold-js/harold-template-docs)
