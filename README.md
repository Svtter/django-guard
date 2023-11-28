# django-guard

Disable new connection when memory usage is high.

## Motivation

Almost all server down developed by django framework was caused by exhausted memory.

## Installation

`pip install django_guard # not upload to pypi since 2023/11/27`

## TODO

- [ ] Upload to pypi
- [ ] Add user documentation

## Usage

1. Add `django_guard` to your `INSTALLED_APP`.
2. Add `django_guard.middleware.GuardMiddleware` to `settings.middleware`.`
3. Set threshhold to `settings`

```python
GUARD_THRESHOLD = {
    'memory': 0,
}
```
