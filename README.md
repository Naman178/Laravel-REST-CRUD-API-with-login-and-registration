## Author

-   [Naman Makwana](https://github.com/Naman178/)

## About

This is simple laravel REST API project with the login and registration functionality.

## DataManager class

    The DataManager class is one and only class in entire app which interact with database, perform business logic. Thus data pass from controller to DataManager via layer
    like

    Controller->OperationManagerInterface->OperationManager->DataManagerInterface->DataManager

    and data return by DataManager is in following way
    DataManager->OperationManager->Controller

## Database models

    I have declared all Database related models in App\Repository\Models\

## Database Configuration

    Create the database named "laravelapi"

    and then run the migration command to add the tables in the database 

    and then run the seeds command to add the data into the database.

## REST API information

    We have used Sanctum for the REST API 

    so you have to instal all packages for the Sanctum


## useful commands

    1. php artisan serve
    2. php artisan migrate:fresh
    3. php artisan optimize
    4. composer install
    5. php artisan route:cache
    6. php artisan make:model <modelname>
    7. php artisan cache:clear
    8. php artisan config:clear
    9. php artisan make:provider <providername>
    10.php artisan make:controller <controller name>
    11.php artisan schedule:work
    12.php artisan queue:listen
    13.php artisan passport:client --personal


## Run project
   
    1.composer install
    2.composer require laravel/sanctum
    3.php artisan vendor:publish --provider="Laravel\Sanctum\SanctumServiceProvider" 
    4.php artisan migrate:fresh
    5.php artisan route:cache
    6.php artisan config:cache
    7.php artisan optimize
    8.php artisan serve

# How to run APIs in local server

	run the url in postman and write appropriate method and run the files

# API Information

	1.Registration (http://localhost:8000/api/register) (https://prnt.sc/hT3FbhwplOwF)
	2.Login (http://localhost:8000/api/login) (https://prnt.sc/EWE84f09XhI6)
	3.Product List (http://localhost:8000/api/products) (https://prnt.sc/6rW0m7q7W5_h)
	4.Add Product (http://localhost:8000/api/products) (https://prnt.sc/VzSk_9yo1gYm)
	5.Get Single Prodcut (http://localhost:8000/api/products/1) (https://prnt.sc/HVoKEb941FGu)
	6.Update Product (http://localhost:8000/api/products/1?name=Testing Name Update&detail=Testing Details Update&price=500) (https://prnt.sc/YiGpMduTYBKf)
	7.Delete Prodcut (http://localhost:8000/api/products/1) (https://prnt.sc/NNtwsK7WKhCa)