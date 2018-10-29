# Scrape Google Maps by Octoparse

Just download the `GoogleMaps_Copy.otd` file provided, and import it into [Octoparse](https://www.octoparse.com) - a free automatic web scraping tool. You can get Google Maps data including the name of restaurants, rating, category, location, description, and hours. The following tutorial shows detailed steps of creating this task.

See more [here](https://www.octoparse.com/tutorial-7/scrape-data-in-google-maps)

To be specific, we enter "Orange CA" on [Google Maps website](https://www.google.com/maps) and enter "restaurants" and copy the [URL](https://www.google.com/maps/search/restaurants/@33.7726566,-117.8522727,13z/data=!3m1!4b1) (https://www.google.com/maps/search/restaurants/@33.7726566,-117.8522727,13z/data=!3m1!4b1) for scraping.

---

## Catalog

1. [Go to web page](#go-to-web-page---to-open-the-target-web-page)
2. [Create a pagination loop](#create-a-pagination-loop---to-scrape-all-items-from-multiple-pages)
3. [Build a loop item](#build-a-loop-item---to-scrape-all-the-items-on-current-page)
4. [Extract data](#extract-data---to-select-the-data-to-extract)
5. [Start extraction](#start-extraction---to-run-your-task-and-get-data)

---

## Go to web page - to open the target web page
In this tutorial, the first step is a little different. We should set "Browser" in "Settings" in order to open Google Maps correctly in Octoparse since default browser cannot open Google Maps correctly.

* Create a task with "Advanced Mode" in "Home" page.
* Enter [Google website](https://www.google.com) into the "Extraction URL" box and click "Save URL" to move on.
* Open "Workflow" in the top-right corner in Octoparse.
We strongly suggest turn on "Workflow" mode to get a better review of what you are doing with your task just in case you mess up with the steps.
* Click "Save" to save your task.
* Click "Settings" and change your browser to "Firefox 45.0" and click "Save".
* Change your "Page URL" in "Go To Web Page" step in workflow to the [URL](https://https://www.google.com/maps/search/restaurants/@33.7726566,-117.8522727,13z/data=!3m1!4b1) (https://www.google.com/maps/search/restaurants/@33.7726566,-117.8522727,13z/data=!3m1!4b1) or any other website containing location information you want in Google Maps.

![GoogleMaps_gif_1](https://raw.githubusercontent.com/octoparse/Scrape-Google-Maps-by-Octoparse/master/GoogleMaps_gif_1.gif)

<br><br>

## Create a pagination loop - to scrape all items from multiple pages

* Click on `>` button (which means next) for pagination.
* Click "Loop click Single Button" in "Action Tips" panel.
* Uncheck the box for "Retry when page remains unchanged (use discreetly for AJAX loading)"
* Check the box for "AJAX Load" box and set "AJAX Timeout" as 15 seconds.
* Click "OK" to save.

![GoogleMaps_gif_2](https://github.com/octoparse/Scrape-Google-Maps-by-Octoparse/blob/master/GoogleMaps_gif_2.gif?raw=true)

| Tips: |
| :------ |
| If you want to learn more about AJAX, check this [AJAX Tutorial](https://www.octoparse.com/tutorial-7/ajax) out! |

<br><br>

## Build a loop item - to scrape all the items on current page

* Select the first and the second block of restaurant information in the current page.
* Click "Extract data in the loop" in "Action Tips" panel.
Octoparse will automatically select all similar elements (blocks of restaurant information) and extract data on current page.

![GoogleMaps_gif_3](https://github.com/octoparse/Scrape-Google-Maps-by-Octoparse/blob/master/GoogleMaps_gif_3.gif?raw=true)

<br><br>

## Extract data - to select the data to extract
* Customize fields and delete useless fields.
* Click "OK" to save.
We will select name of restaurants, rating, category, location, description, and hours to remain in fields.

![GoogleMaps_gif_4](https://github.com/octoparse/Scrape-Google-Maps-by-Octoparse/blob/master/GoogleMaps_gif_4.gif?raw=true)

* Edit the field name (e.g. name and rating)

![GoogleMaps_gif_5](https://github.com/octoparse/Scrape-Google-Maps-by-Octoparse/blob/master/GoogleMaps_gif_5.gif?raw=true)

<br><br>

## Start extraction - to run your task and get data

* Click "Save" to save your task.
* Click "Start Extraction" and "Local Extraction" to start local extraction task. 

![GoogleMaps_gif_6](https://github.com/octoparse/Scrape-Google-Maps-by-Octoparse/blob/master/GoogleMaps_gif_6.gif?raw=true)

* Click "Export" button to export data after extraction. 

After the executing above steps, details of restaurants information on Google Maps will be collected automatically by Octoparse. Feel free to let us know if you have any question or need our assistance. Contact us [here](https://www.octoparse.com/contact)!
