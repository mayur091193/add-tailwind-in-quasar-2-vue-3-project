# Add Tailwind CSS in the Quasar 2 and Vue 3 project - Simple steps


<img src="https://c6c8j7x5.rocketcdn.me/wp-content/uploads/2022/04/Quasar-Framework.png" alt="Reddit">
(Image Source - https://stackdiary.com/vue-ui-components-kits/)

---
[Check out blog](https://medium.com/@mayur091193/add-tailwind-css-in-the-quasar-2-project-simple-steps-339c545dafe0)

Quasar Framework is a great UI framework that provides lots of ready-to-use components which are well tested on the web, iPad, mobile, and all devices.

By adding Tailwind CSS, you can build website UI within minutes. Quasar+Tailwind CSS will definitely help you increase front-end development speed!

In 90% of cases, if you install tailwind using the default command, it won't work, I am sharing steps that worked for me after lots of trial and error.
Create Quasar Project and install Tailwind CSS and it's dependencies:
```
quasar create quasar-tailwind-project

cd quasar-tailwind-project

npm install -D tailwindcss@npm:@tailwindcss/postcss7-compat postcss@^7 autoprefixer@^9
```
Add tailwindcss in the plugins section to .postcssrc.js like below

```
module.exports = {
  plugins: [
    require('tailwindcss')
  ]
}
```

Add tailwindcss imports to **src/css/app.scss

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Now you are ready to use Tailwind CSS in your Quasar Project, just use code from their official documentation.

## Support

- 💖 Sponsor me to support my open source work. https://github.com/sponsors/mayur091193 
- 🙏 Please Support: https://www.buymeacoffee.com/mayur091193
