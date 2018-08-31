# striped - WIP
striped is a brazen two-column [Gutenberg](https://github.com/Keats/gutenberg) based on the Jekyll theme of the same name that pairs a prominent sidebar with uncomplicated content.

![striped screenshot](https://github.com/zoosky/striped/blob/master/screenshot.png)


## Contents

- [Installation](#installation)
- [Options](#options)
  - [Sidebar menu](#sidebar-menu)
  - [Sticky sidebar content](#sticky-sidebar-content)
  - [Themes](#themes)
  - [Reverse layout](#reverse-layout)

## Installation
First download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/zoosky/striped.git
```
and then enable it in your `config.toml`:

```toml
theme = "striped"
```

## Options

### Sidebar menu
Set a field in `extra` with a key of `striped_links`:
```toml
[extra]
striped_links = [
    {url = "https://google.com", name = "Google.com"},
    {url = "https://google.fr", name = "Google.fr"},
]
```
Each link needs to have a `url` and a `name`.

### Sticky sidebar content
By default striped ships with a sidebar that affixes it's content to the bottom of the sidebar. You can optionally disable this by setting `striped_sticky` to false in your `config.toml`.

### Themes
striped ships with eight optional themes based on the [base16 color scheme](https://github.com/chriskempson/base16). Apply a theme to change the color scheme (mostly applies to sidebar and links).

![striped in red](https://f.cloud.github.com/assets/98681/1831229/42b0b354-7384-11e3-8462-31b8df193fe5.png)

There are eight themes available at this time.

![striped theme classes](https://f.cloud.github.com/assets/98681/1817044/e5b0ec06-6f68-11e3-83d7-acd1942797a1.png)

To use a theme, set the `striped_theme` field in `config.toml` to any of the themes name:

```toml
[extra]
striped_theme = "theme-base-08"
```

To create your own theme, look to the Themes section of [included CSS file](https://github.com/poole/striped/blob/master/public/css/striped.css). Copy any existing theme (they're only a few lines of CSS), rename it, and change the provided colors.

### Reverse layout

![striped with reverse layout](https://f.cloud.github.com/assets/98681/1831230/42b0d3ac-7384-11e3-8d54-2065afd03f9e.png)

striped's page orientation can be reversed by setting `striped_reverse` to `true` in the `config.toml`.
