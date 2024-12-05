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
   <li>php artisan route:cache</li>
 </ul>
</p>

## Utiles
<p>
 para por si compras o adquieres un hosting el cual no permite ssh y quieres lanzar comandos se puede hacer mediante una ruta de la siguiente manera.
 <br>
 <ol>
  <li>Creamos la ruta y el controlador</li>
  <li>Añadimos la siguiente libreria: <sub>use Illuminate\Support\Facades\Artisan;</sub>  </li>
  <li> Mediante el comando  <sub>Artisan::call($command, $arguments);</sub>   vamos generando comandos </li>
  <li>Ejemplo  <sub>Artisan::call("cache:clear");</sub></li>
 </ol>
</p>
## Script con los comandos de limpieza por si no dispones de ssh.
### Ejecuta los comandos de Artisan para refrescar el entorno
<sup>
    Artisan::call('cache:clear');
    Artisan::call('config:clear');
    Artisan::call('view:clear');
    Artisan::call('route:clear');
    return "Entorno limpiado y refrescado correctamente.";
</sup>   

