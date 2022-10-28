# Laravel Comandos basicos

# iniciar applicacion
```bash
$ php artisan serve
```

# crear modelo (representa una tabla llamada products)
```bash
$ php artisan make:model Product
```

# crear migracion 
```bash
$ php artisan make:migration crear_tabla_products
```
# este comnando genera un archivo
# abrir dicho archivo y agregar los campos requeridos

```php
Schema::create('products', function (Blueprint $table) {
    $table->id();
    $table->string("name");
    $table->string("description");
    $table->integer("quantity");
    $table->float("price");
    $table->timestamps();
});
```

# aplicar migraciones (crear tablas )
```bash
$ php artisan migrate
```

