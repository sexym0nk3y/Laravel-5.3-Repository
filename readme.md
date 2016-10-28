# Laravel 5.3 Repositories

Simple repository setup for Laravel 5.3

## Installation

1. Copy `BaseRepository.php` into `App/Repositories`
2. Copy `repository.stub` into `App/Console/Commands/stubs`
3. Copy `MakeRepositoryCommand.php` into `App/Console/Commands`
4. Add `MakeRepositoryCommand:class` into the `App/Console/Kernel.php`

```php
class Kernel extends ConsoleKernel
{
    /**
     * The Artisan commands provided by your application.
     *
     * @var array
     */
    protected $commands = [
        Commands\MakeRepositoryCommand::class,
    ];

```

## Usage
The `make:repository` command automatically creates a new Repository into `App\Repositories`

```terminal
php artisan make:repository NameRepo
```