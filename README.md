# laravel
<p>Los comandos mas usados en laravel.</p>
<p>
<h3>Migraciones</h3>
 <ul>
  <li>php artisan migrate                                 //lanzar migraciones</li>
  <li>php artisan migrate:refresh                         //rollback y migraciones de nuevo</li>
  <li>php artisan make:migration create_categories_table  //creacion de tablas</li>
  <li>php artisan migrate:rollback                        //Rollback</li>
  <li>php artisan migrate:status                          //estado de las migraciones.</li>
 </ul>
</p>
<p>
  <h3>Seeder</h3>
 <ul>
  <li>php artisan make:seeder nombre_seeder</li>
  <li>php artisan db:seed</li>
 </ul>
</p>

<p>
<h3>Migraciones y seeder</h3>
 <ul>
  <li>  php artisan migrate --seed            //Lanzar migraciones y seeder secuencialmente</li>
  <li>php artisan migrate:refresh --seed   //Rollback y migraciones junto con seeder</li>
 </ul>
</p>


<p>
 <h3>Limpieza</h3>
<ul>
  <li>php artisan cache:clear</li>
  <li>php artisan config:clear</li>
  <li>php artisan config:cache</li>
 </ul>
</p>
