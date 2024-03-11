## LocalGov Drupal Recipe

> [!CAUTION]
> This recipe is experimental and things will break and/or not work from time to time. This should not be installed in production environments.

This recipe is designed to do the following:

- Install core modules that we want
- Set specific core configuration
- Set specific contributed module configuration
- Install and setup base LocalGov Drupal modules and configuration

## Configuring Drupal to Apply Recipes

Follow the [Configuring Drupal to Apply Recipes documentation ](https://git.drupalcode.org/project/distributions_recipes/-/blob/1.0.x/docs/getting_started.md#getting-started-configuring-drupal-to-apply-recipes)

## Installing

- Start with a Drupal 10 site.
- Install the 'Minimal' profile.
- Apply the recipe

The recipe can be applied with PHP. Note that `core/scripts/drupal` must be
executable with `chmod +x`.

```shell
php core/scripts/drupal recipe recipes/contrib/localgovdrupal_recipe
```

If all goes well, you should see the following output:

```shell
 [OK] LocalGov Drupal applied successfully
```

Clear the cache after the recipe is applied. When going back to the site,
all the recipe configuration and customization has been applied.
