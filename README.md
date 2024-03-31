# Portfolio Template 🚀

![Vue](https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D) ![Sass](https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white) ![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white) ![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)


# :hammer_and_wrench: Install & Setup

## Get Up & Running :running:

1. Fork the repo
2. Clone the new repo to your machine
3. Run `npm i` to install dependencies
4. Run `npm run serve` to start the development serve
5. View your portfolio at `http://localhost:8080`

## Making It Yours (TLDR;) :sparkles:

1. Update all of the [Images](#content):

- replace `favicon.ico`(or delete)
- replace `header-background.jpg`
- replace `logo.png` (or delete)
- add images to the `potfolio/`directory

2. Update the [Content](#content) from the `.json` file

3. Create a [contact form](#form) using [99inbound](https://app.99inbound.com/)

4. Update the [Styling](#styling) by updating Sass variables

# :pencil: Details for Populating Portfolio

## Meta :gear:

<details>
<summary>Steps</summary>

- In `/public/index.html` you will see `<meta>` properties commented out. Uncomment them and fill them out as apporiate (_optional_)

> Necessary if you plan on making your portfolio searchable in Google and optimizing for SEO.

- Similarly, fill out the `<title>` tags with your name or a title of your choice.
  </details>

## Images :camera:

### Favicon

<details>
<summary>Steps</summary>
- Delete the existing favicon.ico (Note this sometimes takes a while to update on the development server)

- Replace favicon.ico in the `/public` directory with your own favicon (_optional_)

> The Favicon needs to be in a `.ico` format. If you have a `.png` you would like to use you can convert it to `.ico` with an online converter such as this one [here](https://icoconvert.com/).

</details>

### Logo

<details>
<summary>Steps</summary>
- Delete `logo.png` from the assets folder

- Add a new `logo.png` file (_optional_)

> If you do not add another logo.png, you first & last name will display in the 'navbar-brand' area

</details>

### Other Images

**All other images can be found in `src/assets/images`**

> Be sure to keep the same filename and extension for the header-background, profile-pic, & logo.

- In the portfolio folder, add photos to represent your projects

> Naming your files with readable filenames is good practice for SEO.

**Recommended Sizes**

- `header-background.jpg` - A large hero image, at least 1200px wide, but no larger than 1900px.
- `profile-pic.png` - This should be a 1:1 aspect ratio. It will be reduced to 300px.
- `/portfolio` - Recommended aspect ratio of 5:3


# :art: Styling

This project uses SASS / SCSS.

- Easily update basic styling such as colors from `/src/styles/scss/_variables.scss`

- Only update the other partials if you know what you're doing

> In `src/styles/scss`, there are a number of folders and .scss files
>
> All of the files appended with `_` are imported into the `main.scss` file
>
> These get compiled into `src/styles/css/main.css` which is where the site css comes from

- In a terminal instance, run `npm run sass` to watch for changes to scss files and compile them into css

# :bell: Features

- Utilizes typewriter-effect npm package
- Add a list of facts about yourself in your About section
- Specify skills in different categories and your skill level that will fill the bar up the respective amount to your skill level
- Add filters for your portfolio projects
- Animations for each section on scroll

# :star: Credits

- [Bootstrap](https://getbootstrap.com/docs/4.4/getting-started/introduction/)
- [Font Awesome](https://fontawesome.com/)
- [99inbound](https://www.99inbound.com/)
- [Vue.js](https://vuejs.org/v2/guide/)
- [SASS](https://sass-lang.com/)
- [Animate On Scroll Library](https://github.com/michalsnik/aos)
- [This codepen](https://codepen.io/joxmar/pen/NqqMEg) to highlight active navbar items
- [Typewriter effect](https://www.npmjs.com/package/typewriter-effect)
- [Jonas Schmedtmann](https://codingheroes.io/) for teaching me about Sass
- www.bobross.com for the content


# :scroll: License

_This project is licensed under the terms of the MIT license._
