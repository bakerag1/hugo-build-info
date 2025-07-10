# Hugo Build Info Module

This module provides a json endpoint to get information about the build. 

# Use

Add this to your hugo config and run `hugo mod tidy`. If you aren't already using modules, you'll need to run `hugo mod init <module name>` first.

```yaml
module:
  imports:
    - path: github.com/bakerag1/hugo-build-info
```

now you will have an `/api/build-info/index.json` file in your site.

It's recommended you add this to your config as well, assuming you have your site in source control.

```
enableGitInfo: true

frontmatter:
  lastmod:
    - :git
    - lastmod
    - date
    - publishDate
```
