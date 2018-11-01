# Resolve Permission Cache in CakePHP

## CakePHP error: cake_core_ cache was unable to write 'cake_dev_en-us' on Ubuntu

Run the follow comands
```
cd /var/www/html/project-folder/app;
```

```
find tmp -type d -print0 | xargs --no-run-if-empty -0 chmod 2755;
```

```
find tmp -type f -print0 | xargs --no-run-if-empty -0 chmod 0644;
```

```
chown -R www-data:www-data tmp;
```
