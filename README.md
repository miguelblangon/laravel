# laravel
<p>Los comandos mas usados en laravel.</p>
<p>
## Migraciones.
 php artisan migrate                                 //lanzar migraciones
 php artisan migrate:refresh                         //rollback y migraciones de nuevo  
 php artisan make:migration create_categories_table  //creacion de tablas
 php artisan migrate:rollback                        //Rollback
 php artisan migrate:status                          //estado de las migraciones.
</p>



<p>
  ## Seeder
  php artisan make:seeder nombre_seeder
  php artisan db:seed 
</p>

<p>
  ## Migraciones y seeder
  php artisan migrate --seed            //Lanzar migraciones y seeder secuencialmente
  php artisan migrate:refresh --seed   //Rollback y migraciones junto con seeder
</p>


<p>
## Limpieza.
php artisan cache:clear
php artisan config:clear
php artisan config:cache  
</p>
