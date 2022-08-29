# Detailed Instructions From Your Instructor Team

The objective of this challenge is for you to scrape high-resolution images of Mars’ hemispheres and titles, update the Mongo database, and modify the `index.html` file so the webpage contains all the information collected in this module as well as the full-resolution images and titles of the four hemispheres.

## Deliverable 1: Scrape Full-Resolution Mars Hemisphere mages and Titles

For the first deliverable, we are asking you to scrape high-resolution images of Mars’ hemispheres and your titles.

you might find the tasks in this challenge to be slightly difficult. There is no one specific method to retrieve the high-resolution image and title of each hemisphere. However, we have provided [starter code](./Resources/Mission_to_Mars_Challenge_starter_code.ipynb) that you should download, copy, and add to your `Mission_to_Mars_Challenge.ipynb` file.

The starter code, has commented steps in the file where you will need to add code to complete this part of the challenge. For Step 3, we have provided a hint of a common approach to retrieve the full-resolution images and titles of each hemisphere.

  * Before the `for` loop, we suggest that you find the HTML tag that holds all the links to the full-resolution images, or find a common CSS element for the full-resolution image.

  * Then, in the `for` loop that should iterate throught the tags or CSS element.

  * Before clicking on each hemisphere link, you should create an empty dictionary. We suggest in the **Hint** to use, `hemispheres = {}`.

  * Next, you should use the `for` loop to click on each hemisphere link and navigate to the full-resolution image page, retrieve the full-resolution image URL string and the title for each hemisphere. **Hint** this step will be similar to scraping the Featured Image and you will need to use the base URL to create the full URL.

  * Inside the `for` loop you should save the full-resolution image URL string as the value for the key, `img_url`, and the title as the value for the key, `title`, in the `hemispheres = {}` dictionary.

  * Before getting the next image URL and title, you'll need to add the `hemispheres = {}` dictionary to the `hemisphere_image_urls` list.

When you print out the list of dictionary items, you should be similar to this image:

![The dictionary that holds the image URL strings and the hemisphere titles for each hemisphere.](./Resources/hemisphere_image_urls.png)


## Deliverable 2: Update the Web App with Mars’s Hemisphere mages and Titles

For the second deliverable, you will need to add the code you created in Deliverable 1 to your `scraping.py` file, update your Mongo database, and modify your `index.html` file so the webpage contains all the information you collected in this module as well as the full-resolution image and title of each hemisphere.

you might find the tasks in this challenge to be more challenging than Deliverable 1. Where you may find the most difficulty, is after you export the `Mission_to_Mars_Challenge.ipynb` file as a Python file and create a new function that scrapes the hemisphere data.

We have provided an updated `index.html` [file](./Resources/index.html) for you to use that will add the hemispehre data to the webpage. However, you may need to modify the HTML code if you have a different database or dictionary name when you loop through the dictionary in the database using, `{% for hemisphere in mars.hemispheres %}`. Finally, you will need to run the `app.py` file, open the `index.html`, and click the "Scrape New Data" button.

The full-resolution images should be rendered on the webpage as shown in the following image.

![The full-resolution images and titles of the four hemispheres of Mars.](./Resources/full_resolution_images.png)

## Deliverable 3: Add Bootstrap 3 Components

For the final delivareable, we are asking you to update your web app to be mobile responsive and add two additional Bootstrap 3 components to make your website standout.

you you should not find the tasks in this deliverable to be difficult. Using the DevTools you will need to make sure that your web app is mobile responsive for all the data on the webpage. If not, you will need to use the [Bootstrap 3 grid system](https://getbootstrap.com/docs/3.3/examples/grid/) to make the web app mobile responsive.

you will also need to apply two additional Bootstrap 3 components to make your webpage standout. We have provided three examples for you, or you can choose other options from this [list](https://getbootstrap.com/docs/3.3/css/).

## Submission

Make sure you upload the following to your GitHub repository:

1. The `Mission_to_Mars_Challenge.ipynb` file with all the code used for scraping.
2. An updated `scraping.py` file.
3. The `app.py` file.
4. The `index.html` file in the template folder and any CSS stylesheets.

## Grading Rubric

The [Misson to Mars Grading Rubric](./Resources/Module_10_Challenge_Grading_Rubric.pdf) is provided for you to use when grading you' submissions.
