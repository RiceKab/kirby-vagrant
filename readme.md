# kirby-vagrant
The kirby starterkit with added vagrantfile to easily setup an isolated environment to test in.

## Important
Debug is enabled out of the box. This can be disabled again in the config by setting `c::set('debug', false);` or just removing out the line entirely.

**This should be disabled before going into production!**

## Setup
* Clone the project
* [Optional] If you already have a `ubuntu/trusty64` box, run `vagrant box update` to get the latest version.
* `vagrant up`

Once the box is setup the website is available on `localhost:8888`. You can login to the control panel at `localhost:8888/panel` with TODOTODOTODO

If you want to SSH into the machine you can do so with the vagrant defaults: username/password `vagrant` (or just `vagrant ssh`)

**See a blank page?** - Kirby's dependencies may not have properly installed. Although this should be done during the provision you can run `composer install` in `/kirby` just to rule that out.

## License
Whilst this box is available under MIT license, you will need a Kirby license once you go live.

See Kirby's EULA at <https://getkirby.com/license> for more details.