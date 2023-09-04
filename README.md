# Features

* Simple, easy to use, single or multi page, A4-sized Curriculim Vitae generator.
* Print friendly, just use your browser or save as PDF.
* Write your resume in yaml. All content stored in data files.
* Add/Remove sections order change section orders by editing `config.yaml`.
* Section names are configurable in `config.yaml`. So, you can write in any language you want.

This theme is based on the resume-A4 theme by [Mert Bakır](https://gitlab.com/mertbakir/resume-a4). I just added some features and changed the style a bit to fit my tastes, and I'm sharing it here in case someone else finds it useful.

# How To Use

## Download

1. Create a [hugo](https://gohugo.io/) project.
2. Go to themes folder.
3. Clone this theme.

```
cd themes
git clone https://github.com/jacopouggeri/cv.git
```

or add as a submodule

```
git submodule add https://github.com/jacopouggeri/cv.git themes/a4cv
```

## Start

1. Open `config.yaml` and add your relevant information.
2. Modify the `data` folder in the root directory. All you need is that folder.
3. Test locally running `hugo server`. (If you don't have hugo installed, check [here](https://gohugo.io/getting-started/).)

## Config File

* You can add/remove sections.
* Add multiple pages as many as you like.
* The order of "features" is important in the config file. 

### Custom CSS

Copy the ```\assets``` folder in the root directory if you want to make simple modifications, or make your own theme by editing the theme directly from themes/a4cv/assets.
### Avatar

Set the avatar link in `config.yaml`. Keep your image in the `static` folder. You can set `avatar` as ```false``` if you don't want to add a picture.

### Publications

You can change `style` of the `publications` feature in the config file. There are options for APA and IEEE standards. As always, if you don't like them, you can make your own ;)

## Print | Save As PDF

If you don't like the result of "save as pdf" in Mozilla Firefox, try Chrome or a Chromium-based browser. Probably, because Firefox doesn't support [this](https://developer.mozilla.org/en-US/docs/Web/CSS/%40page/size).

# License

This project is open-sourced and licensed under the terms of the MIT license. I would be happy though, if you give attribution.

> _I'm open to suggestions and contributions._

# My Work Flow

1. Make changes.
2. Delete `resources` folder in main project.
2. Build your hugo site using the theme. `hugo server`
3. Copy `resources` folder from main project to theme folder `themes\a4cv\resources`
4. `git commit` and `git push`.
