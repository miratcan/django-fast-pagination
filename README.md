## Fast Paginator for Django

Fast is a simple Django app to paginate Django Querysets. Core Django Paginator uses **LIMIT** and **OFFSET** when creating queries to execute. This application is not using **LIMIT** and **OFFSET**, so it gets faster results. If you have millions of entries in a table, then Django will make you wait a lot longer than this app!

## Quick Start

1. Add "fast_pagination" to your INSTALLED_APPS setting like this:
```python
    INSTALLED_APPS = [
        ...
        'fast_pagination'
    ]
```
2. Import FastPaginator like this:
```python
    from fast_pagination.helpers import FastPaginator
```
3. Then, you are ready. All you have to do is give your queryset and number of entries when creating FastPaginator object.