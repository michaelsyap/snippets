# Laravel CLI Snippets

####  Clear the compiled classes and services in Laravel's application cache 

```bash
php artisan clear-compiled 
```

####  To remove the configuration cache file created by `config:cache` command
```bash
php artisan config:clear 
```
####  To clear any previously generated route cache
```bash
php artisan route:clear 
```
####  To create a symlink from `public/storage` to `storage/app/public`
```bash
php artisan storage:link
```

