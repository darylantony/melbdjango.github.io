
# MelbDjango

If you're speaking at an upcoming event, you're invited to fork this repo, add your details into index.html, and submit a pull request so we can merge in your changes and publish details of your talk.

Don't worry, we'll review before merging, so there's no need to worry about breaking anything!  Look for the following code, and go to work:

```
<!-- speaking article begins -->
<article class="speaking Grid-cell">

    ...make your changes to the markup in here
    (please follow the form in the template!)

</article>
<!-- speaking article ends -->
```


## Developing Locally

If you need to change any styles, you can do run the site locally to compile the scss and serve the files. Make sure you have the latest version of [nodejs](https://nodejs.org/en/) installed.

```
  npm install
  npm start
```

This will:
  - Watch files in the `styles/` directory for changes
  - Compile `styles.scss` to a `.tmp/` directory
  - Run `autoprefixer` over the compiled temp files
  - Pass the prefixed file through clean-css, resulting in `dist/styles.min.css`
  - Serve the files using `browser-sync`, and refresh on changes
