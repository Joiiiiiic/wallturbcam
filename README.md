# Basic tutorial

The website is built using Hugo, it may look a bit scary but it's not I promise. Essentially what Hugo does is convert the files we write into HTML so they can be uploaded to the the website. 

This tutorial will teach you how to update the contents but if you need to change other things like theme and layout, contact Joy (jc2392). If she doesn't do it, annoy her until she does. 

For details about the Youtube channel where the videos are uploaded, contact Joy directly. 

The first part of the tutorial will teach you how to add contents to the website, but you will not be able to view it until Joy (hopefully) updates it. If you wish to view it or do the updating yourself, instructions can be found in the second part of this document, otherwise feel free to skip it. 

If you have any suggestions/advice for the aesthetics, structure or anything else about the website, feel free to contact Joy. She will be eternally grateful for you help. (She is fully aware of how bad it currently looks so will not take any offence in your comments.)

## Basics

### Folder structure

The two main folders you need to know are `content` and `static`. 

The content folder includes the content of most pages of the website (not the layout, just the text and other relevant things eg. directory of images), each one in a separate `.md` file. The subfolders are 
reasonably intuitive, so find the corresponding page you want to edit. This tutorial will go into more detail about how to edit each of the main pages. 

The static folder includes all the files that stay as it is when Hugo converts others into HTML, in our case this is mainly images. All new images should be added here. 

If there is anything you need to do that might involve changing any other folder (apart from those mentioned below), contact Joy. 

## Changing specific contents

### logo & favicon

The current placeholder image can be found in the `static` folder, replace them then you are good to go. It is recommended that the logo has a transparent background. Also, ensure that the favicon is 32px*32px. 

### Slides on the home page

The file that controls it can be found in `data/slide.json`. It is very intuitive, add & delete slides as you wish. 

### Text on the home page

File found in `content/_index.md`. 

### Edit pages & create new pages in "project"

The files for corresponding pages can be found in `content/project/`. Edit the corresponding file. Add a new file by duplicating an existing one then edit. 

For content in the front matter (the one at the top between two lines of `---`), description refers to the text that shows on the main project page, weight is the order each page is arranged on the main page (1 being the one highest up). Image refers to the background image displayed in the main "research" page. 

The page is in markdown format, see files in `content/random_pages` for reference on how to display different fonts, tables etc.

### Edit "people" page

File found in `content/people/_index.md`. The structure is (hopefully) very intuitive, add/delete/edit entries as required. Images should ideally be of the aspect ratio 3/4, otherwise it will be cropped

### Edit "publication" page

File found in `content/publication/_index.md`. 

## View and update edits to the website yourself

### Installation

If you wish to preview and/or upload the website yourself, you will need to install a few things: **!!!! need to check !!!!!!!**

- Hugo
- Go (the language)
- CSS

There are plenty of websites that tell you how to do it. 

### Testing and uploading the website

To test the site, run the following code in the root directory of the website: 

```bash
hugo server
```

You can then view the website at `http://localhost:1313/`. I would recommend turning on autosave on your text editor (eg. VS code), the website will update automatically whenever you change anything. Otherwise, it will update when you save a file. If anything weird appears, try rerunning the code. 

Once the website is ready to be published, run the following code: 

```bash
hugo
```
This generates HTML (and other relevant) files in the `public` directory. It is recommended that you delete everything that is in the folder first before running the code. 

Once it is done (should be very very quick - one of the benefits of using Hugo and those alike), copy everything in the folder to `wallturbcam/public_html` on the SRCF server and the website should show in a few minutes. 

Note: running `hugo server` also generates things in the `public` directory, but do not upload that to the website. 


## The tutorial ends here

---

---

## Checklists

### A list of things that might be needed:
- something smart to say on the home page, maybe an introduction of the group?
- project page: some more description for each of the cases might be useful
- publication: would this be required? - happy to do it, shouldn't be too hard, but could just link to google scholar?
- people: picture + short bio?
- logo or whatever that could go on the top left corner & favicon (which is a smiley face currently...)
- add copyright at the bottom of the site
- stupid question - what is the name of the group? Wall turbulence, I assume from the name of the website? 
- Is there anything else that is needed?
- Check youtube channel, change channel name, video name etc. Videos are currently unlisted ie. cannot be found through search, can only access with link
