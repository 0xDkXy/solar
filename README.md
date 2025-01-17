# Solar Theme for Zola

Port of [Solar theme for Hugo](https://github.com/bake/solar-theme-hugo) to Zola.

![screenshot](./screenshot.png)

## Installation


First download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/hulufei/solar-theme-zola.git
```
and then enable it in your `config.toml`:

```toml
theme = "solar-theme-zola"
```

Add `title` and `description`:

```toml
title = "Your Blog Title"
description = "Your blog description"
```

## Options

### Color schemes

Set color scheme to (Solarized) `dark` or (Solarized) `light` with `solar_theme` option in `extra`:

```toml
[extra]
...
solar_theme = "dark"
```


### Sidebar menu

Set a field in `extra` with a key of `site_menus`:

```toml
site_menus = [
  { type = "title", name = "More About Me" },
  { type = "url", url = "https://github/hulufei.com/solar-theme-zola", name = "Repository" },
  { type = "url", url = "rss.xml", name = "RSS" },
  { type = "title", name = "Friends" },
  { type = "url", url = "https://github.com/0xdkxy/", name = "0xDkXy" },
]
```
Each link needs to have a `url` and a `name`.  
If type is `title`, it will be the title of following urls.  
Otherwise it will be a hyperlink.
