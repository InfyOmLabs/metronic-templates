# metronic-templates

Metronic Theme templates for InfyOm Laravel Generator

## Installation

1. Add package to repo:

        "infyomlabs/metronic-templates": "dev-master"
        
2. Run composer update

3. Add service provider to `config/app.php`

        \InfyOm\MetronicTemplates\MetronicTemplatesServiceProvider::class,

4. Edit `config/infyom/laravel_generator.php`

 set `'templates'         => 'metronic-templates'`
 
5. Run Infyom publish layout command
 
        php artisan infyom.publish:layout
