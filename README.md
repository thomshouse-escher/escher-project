# Escher Project for Git #

Escher is an open-source web application framework written in PHP. This project is a repackaged form of Escher specifically designed for ease of use with the Git version control system.

## Installing from GitHub ##

1. Fork and/or clone the [escher-project][1] repository.
2. In a shell terminal, navigate to your local repository.
3. Run `git submodule init`, then `git submodule update`.
4. Complete `config-sample.php` and rename the file to `config.php`.

### Installing from another source ###

If you do not plan on using Git, you should not create from the escher-project repository.  Please see the main [Escher repository][2] or the [website][3] for other options.

## Creating Your Application in Escher ##

Custom applications in Escher are created as plugins.  Create a short, simply-named folder within the plugins directory and create your application here.

Example:

    /path/to/project# cd plugins/
    /path/to/project/plugins# mkdir myproject
    /path/to/project/plugins# cd myproject
    /path/to/project/plugins/myproject# vim plugin.myproject.php
    ...

Most of your work should occur in this plugin.  Configuration options should be saved in `config.php`.

Remember to add your plugin and commit work to your Git repository as you would with any other project.

## Updating Escher ##

_Note: It is a good idea to merge onto a temporary branch instead of your `master` branch._

1. Make sure your local repository is clean.
2. Run `git fetch escher master` (where "escher" is the name of the `escher-project` remote).
3. Run `git merge escher/master`.
4. If necessary, resolve any merge conflicts and commit.

## License Information ##

Escher is dual-licensed under the MIT and GPL licenses. Please see the [MIT License][4] and [GNU General Public License][5] for details.

[1]: https://github.com/thomshouse/escher-project
[2]: https://github.com/thomshouse/escher
[3]: http://www.escherphp.com
[4]: http://www.opensource.org/licenses/MIT
[5]: http://www.opensource.org/licenses/GPL-3.0
