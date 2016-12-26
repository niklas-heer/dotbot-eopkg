# Dotbot eopkg Plugin

**WIP - needs more testing**

For use with [dotbot](https://github.com/anishathalye/dotbot),
this plugin allows one to easily install or upgrade a list of eopkg packages.

This plugin is heavily inspired by the [apt-get](https://github.com/rubenvereecken/dotbot-apt-get) plugin.

## Usage

It's easiest to track this plugin in your dotfiles repo:

```bash
git submodule add https://github.com/niklas-heer/dotbot-eopkg
```

I also recommend having your eopkg list in a separate file
since dotbot will need root privileges in order to use the plugin.
Using the plugin will look something like this:

```bash
./install -p dotbot-eopkg/eopkg.py -c packages.conf.yaml
```

Example for `packages.conf.yaml`:

```yaml
- eopkg:
  - vim
```
