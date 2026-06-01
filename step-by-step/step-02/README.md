# Step 02 - Add Some CSS

I generated some starting CSS from the Notenik defaults. 

From within Notenik, I used *Collection -> Sample Display Template*.

This created two files within my initial content folder. 

- `display.html` was then discarded
- `display.css` was then renamed `styles.css` and moved to a new `css` folder within the `web` folder. 

Next I needed to add something like the following line to the HTML template file, at the bottom of the `<head>` section. 

```
<link rel="stylesheet" href="css/styles.css" />
```

I added a couple of Notenik wrinkles to this standard line, though. 

First, I added the `=$relative$=` merge template variable before the `css` folder name. This tells Notenik to automatically climb to the top of the `web` folder structure for files generated within subfolders. 

```
<link rel="stylesheet" href="=$relative$=css/styles.css" />
```

And then, instead of putting this line directly into the template file, I created a file named `head-links.html` within the `factory/includes` folder, and placed inside of that file. 

The HTML template file then had the following line added, to pull in the include file we just created. 

```
<?include "../includes/head-links.html" ?>
```

So now, at the conclusion of this step, we have a starting `css` file that is linked into the HTML template. 

So if you now rerun the script file we created in Step 01, it should generate web pages that now have some starting style to them. 

The CSS file will be modified in later steps, but at least now we have some basic styling, including light and dark modes. 
