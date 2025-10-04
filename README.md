# 生日快乐

<p>
<img src="https://img.shields.io/github/stars/abandon888/HappyBirthday" alt="stars" />
<img src="https://img.shields.io/github/issues/abandon888/HappyBirthday" alt="issues" />
<img src="https://img.shields.io/github/forks/abandon888/HappyBirthday" alt="forks" />
<img src="https://img.shields.io/github/license/abandon888/HappyBirthday" alt="license" />
<a href="https://app.netlify.com/sites/friendly-paprenjak-ad64b7/deploys"><img src="https://api.netlify.com/api/v1/badges/39d29171-f3b1-4172-932e-1f657058303a/deploy-status" alt="Netlify Status" /></a>
</p>

Wish someone a happy birthday in a special way.

This project preview page：<https://friendly-paprenjak-ad64b7.netlify.app/>

**Project Highlights**

1. Carefully designed text animations and romantic balloon animations
2. Customize all text, images, background music, and font styles by simply editing the `customize.json` file
3. Click anywhere on the page to create a dazzling fireworks effect
4. Automatically play beautiful background music to create a warm and romantic atmosphere
5. Built with the modern rspack framework for improved performance

## Some project background you may want to know

Used to wish special people or lovers a happy birthday and create a romantic atmosphere. For the story behind the project, you can read my Zhihu blog post: [Thoughts from celebrating birthdays - website background music playing]

## How to use

Fork this project, modify the customize.json file, replace the content with your own content, and then deploy it on github pages or some other hosting website (such as netlify).
- Vercel deploy

   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fabandon888%2FHappyBirthday&project-name=happy-birthday)

- Netlify Deployment (recommended for domestic users, not blocked)

   [![Deploy with NEtlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/abandon888/HappyBirthday)

> You don't need to initiate PR

You can modify text, images, background music, fonts, and more, but there are some caveats:

1. Only modify the customize.json file; do not modify other files, as this may cause the page to display incorrectly.

2. When replacing music, be sure to rename it to the same name or modify the path in the json file, for example, `bgMusic.mp3` in my case.

3. The birthday hat may appear misaligned when replacing images, so it's recommended to trim the image to the same size as the original to ensure optimal viewing.

4. When replacing fonts, simply modify the font configuration in the json file. You can use local fonts or online fonts (such as Google Fonts). The `LXGW WenKai` font file is already included in the project and can be used directly. Also, `font` only supports one font configuration.

Usage Example

  ```json
    "fonts": [
      {
        "name": "Yuvraj"
      },
    //Or use local fonts, but only one font can be used at a time
    // {
    //     "name": "LXGW WenKai",
    //     "path":"./fonts/LXGWWenKai-Regular.ttf"
    //   } 
    ]
  ```

## Local Development/Preview

The project uses npm as the package manager. Please ensure that the node environment has been configured locally. Otherwise, please install it yourself. The node environment verification is as follows:

```
$ node -v
v22.2.1
```

Then install the dependencies:

```
npm install
```

run:

```
npm run start
```

## Other

This project uses pure HTML, CSS, and JavaScript, along with GSAP for animations.

Thanks to the original author for open-sourcing the project. This project is based on [happy-birthday](https://github.com/faahim/happy-birthday) with modifications.

If you like this project, please give it a star ⭐ to encourage me. Thank you!

## Changelog

### v2.0 (February 3, 2025)

1. Build the project using rspack
2. Add font configuration support
3. Add fireworks effects
4. Optimize music playback interaction
5. More configurable options

### v1.0

1. Added music playback effects
2. Added a guide page
3. Localized into Chinese
4. Optimized some details
