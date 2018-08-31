# striped - WIP
striped is a brazen two-column [Gutenberg](https://github.com/Keats/gutenberg) based on the HTML5UP theme striped.

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
