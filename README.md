# Feliz dias das Mulheres :woman:
```php
<?php

use Carbon\Carbon;
use Illuminate\Support\Facades\Route;
use Spatie\Holidays\Holidays;
use Spatie\Holidays\Countries\Angola;

Route::get('/holidays', function () {

    $today = Carbon::now(); //2024-03-08
    return Holidays::for(Angola::make())->getName($today); //Dia Internacional da Mulher

});
```
