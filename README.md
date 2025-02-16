# Disabling Reflex Branding
A guide to disable the branding banner introduced in Reflex version 0.7.0

## Instructions
The branding can be disabled by modifying `reflex/app.py`. Find and comment out these lines (approximately around line 1139-1140):

```python
if is_prod_mode() and config.show_built_with_reflex:
    self._setup_sticky_badge()
```

## Background
Starting with version 0.7.0, Reflex adds a "Built with Reflex" badge to all pages in production environments. This badge can be officially removed by purchasing a license.

For more information about the branding policy, visit the official documentation:
https://reflex.dev/docs/hosting/reflex-branding/

If you'd like to share feedback about this change, you can participate in the community discussion:
https://github.com/orgs/reflex-dev/discussions/4828
