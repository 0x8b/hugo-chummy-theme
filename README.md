# Hugo Chummy Theme

**Chummy** is a modern blog theme for Hugo. It contains multiple content types and pages. The theme is **blazing fast** and **fully responsive**.

[Live Demo](#TODO)

## Requirements

- Hugo (installation guide https://gohugo.io/getting-started/installing)

## Features

## Installation

### 1. Install Hugo

To use this theme you will first need to have Hugo installed. Please follow the official installation guide

**Note**: Check your Hugo version - Hugo Extended is required, because this theme uses Hugo Pipes to compile SCSS and minify assets.

To check your version of Hugo, run `hugo version`. Make sure you see **extended** after the version number.

```sh
$ hugo version
hugo v0.105.0+extended linux/amd64 BuildDate=unknown
```

You do not need to use version v0.105.0 specifically, it just needs to have the **extended** part.

### 2. Create new Hugo site

This will create a fresh Hugo site in the folder `your_project`.

```sh
hugo new site your_project
```

### 3. Install Chummy module

Initialize the hugo module system: `hugo mod init github.com/<your_user>/<your_project>`

```sh
cd example-blog
hugo mod init github.com/<your_user>/<your_project>
```

The easiest way to use a Chummy module for a theme is to import it in the config.

#### 3.1 Import the theme in `config.yaml`

```yaml
module:
  imports:
  - path: github.com/0x8b/hugo-chummy-theme
```

#### 3.2 Import the theme in `config.toml`

```toml
[module]
[[module.imports]]
  path = 'github.com/0x8b/hugo-chummy-theme'
```

#### 3.3 Import the theme in `config.json`

```json
{
    "module": {
        "imports": [
            {
                "path": "github.com/0x8b/hugo-chummy-theme"
            }
        ]
    }
}
```

### 4. Copy the example content

Copy the entire contents of the `your_project/themes/hugo-serif-theme/exampleSite/` folder to root folder of your Hugo site, i.e. `your_project/`. To copy the files using terminal, make sure you are still in the project's root, i.e. the `your_project` folder.

```sh
cp -a themes/hugo-serif-theme/exampleSite/. .
```

### 5. Run Hugo

After installing the theme for the first time, generate the Hugo site.

You run this command from the root folder of your Hugo site i.e. `your_project/`

```sh
hugo
```

For local development run Hugo's built-in local server.

```sh
hugo server --buildDrafts --port 46757
```

Now enter [localhost:46757](http://localhost:46757) in the address bar of your browser.

## Update theme

```sh
hugo mod get -u github.com/0x8b/hugo-chummy-theme
```

## Configuration

### Google Tag Manager

### Google Analytics 4

## License

- See [LICENSE](LICENSE)
- Don't create ports of this theme without asking me
- You can't re-distribute or re-sell this theme as your own template

🇵🇱 **Made in Poland** by Mariusz Gumienny