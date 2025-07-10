# Hugo Build Info Module

This module provides a json endpoint to get information about the build. 

# Use

Add this to your hugo config and run `hugo mod tidy`

```yaml
module:
  imports:
    - path: github.com/bakerag1/hugo-build-info
```

now you will have an `/api/build-info/index.json` file in your site.
