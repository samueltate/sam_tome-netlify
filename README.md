# Live Site

https://boring-lumiere-dba43d.netlify.com



# Requirements

- PHP 7+
- [Composer](https://getcomposer.org/)
- [Drush](https://github.com/drush-ops/drush-launcher#installation---phar)
- SQLite and the related PHP extensions

# Docs

https://tome.fyi/docs/getting-started/


# To deploy content to live site  

Fire up local site - open terminal and run following command

```
cd [path to your sam_tome-netify codebase]
drush runserver 127.0.0.1:8888 
```

Open new terminal, cd to codebaase and run 

```
drush uli -l 127.0.0.1:8888
```

Do your drupal work. Add content and modules like any other site. 

When ready to create static file run

drush tome:static

Then git add. git commit -m ... git push origin master. 

Netlify will see change in repo and update static site.



# Local usage

To install Tome locally, run:

```bash
drush tome:install
```

To start a local webserver, run:

```bash
drush runserver
```

When you're ready to build your static site, run:

```bash
drush tome:static
```

## Further reading

This template is largely based on [drupal-composer/drupal-project], so it's
recommended that you consult their [README.md] for more information.

[drupal-composer/drupal-project]: https://github.com/drupal-composer/drupal-project
[README.md]: https://github.com/drupal-composer/drupal-project/blob/8.x/README.md
