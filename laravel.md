# edit request value
```php
    /**
     * Handle a passed validation attempt.
     *
     * @return void
     */
    protected function passedValidation()
    {
        if ($this->filled('password')){}
        $this->merge(['password' => bcrypt($this->password)]);
    }
```
# model

## see raw query
1:
```php
\DB::enableQueryLog();
 
User::all();
 
dd(\DB::getQueryLog());
```
2:
```php
$query = \DB::table('users')->where('id', '<>' , 29)->limit(5)->toSql();
dd($query); // "select * from `users` where `id` <> ? limit 5"
```
## get randoom record from db
```php
$randomPost = Post::inRandomOrder()->first();
```
```php
$randomPost = Post::all()->random();
```
```php
$randomPosts = Post::all()->random(5);
```

# چطوری یک متغیر رو همیشه توی یک View داشته باشیم؟
`
https://ditty.ir/snippets/laravel/view-composer/XpP9X
`
# artisan

## roll back
```bash
php artisan migrate:rollback --step=5
```

# migration

## foreign, relation

```php
$table->foreign(['role_id'])
    ->references(['id'])
    ->on('roles')
    ->onUpdate('CASCADE') // ->cascadeOnUpdate()
    ->onDelete('SET NULL'); // ->nullOnDelete()
    
```

```php
$table->unsignedInteger('service_id');
$table->foreign('service_id')
    ->references('id')
    ->on('services');
```

## edit column in migration
`
https://ditty.ir/snippets/laravel/migration-alter-table-column/XNb7X
`
