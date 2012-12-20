Symfony2 XHR Error Handling - Demo Application
===============

This is a demo app that accompanies [this blog post](http://marvelley.com/2012/12/20/symfony2-json-responses-for-xhr-errors-and-authentication-failures/).

#Installation

  1. Clone the repository:

        $ git clone git://github.com/craigmarvelley/symfony2-xhr-error-handling.git

  2. Ensure you have [Composer](http://getcomposer.org) available, either on the path or as a [standalone PHAR archive](http://symfony.com/doc/current/book/installation.html#option-1-composer). We'll assume the former, so 

        $ composer help
    
    should print out Composer's help screen.
  
  3. Configure permissions according to the [Symfony manual](http://symfony.com/doc/current/book/installation.html#configuration-and-setup)
        
  4. Copy app/config/parameters.yml.dist to app/config/parameters.yml... 

        $ cp app/config/parameters.yml.dist app/config/parameters.yml
  
     and configure with values correct for your environment.

  5. Complete app installation by running Composer's install command:

        $ composer install

  6. Create the database schema for the app:

        $ app/console doctrine:schema:update --force        
        $ app/console cw:setup:admin

  7. Create a user:
  
        $ app/console fos:user:create
        
  8. Navigate to the app, log in and you're done :)
