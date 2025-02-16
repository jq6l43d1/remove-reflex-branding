# remove-reflex-branding
How to remove the new branding introduced in Reflex 0.7.0

Comment out the following lines in reflex/app.py on lines 1139 and 1140 as of this writing.

```python
if is_prod_mode() and config.show_built_with_reflex:
    self._setup_sticky_badge()
```
