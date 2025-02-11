**Table of contents**
* [Installation](#installation)
* [Usage](#usage)
  * [Prerequisites](#prerequisites)
  * [Job offer analysis](#job-offer-analysis)
  * [The main panel](#the-main-panel)

# Why Job Analysis Chrome Extension
This Chrome Extension is meant to:
* Help you analyze the Job Market 
* Simplify the job searching process

You could figure our for example that:
* Berlin offers more full-remote jobs than Munich
* 24% of Job offers on Upwork are for Website and CMS developers
* 4.5% of Job Offers on LinkedIn come from the Finance & Insurance sector
* ... and much more

<div style="background-color: #f0f0f0; display: inline-block; padding: 0.5rem;">
    <img src="img/example-charts.jpeg" alt="Description of image">
    <p style="font-size: 0.8rem; text-align: center; margin-top: 0.5rem;">Example analysis results</p>
</div>

When you have this information you can focus your energies on the right platform 
(maybe on Stepstone there are more job offers for your desired role),
refine your research filters, and refine your CV to target your ideal clients 
(Berliner Startup in the Finance sector? SMB part-time DevOps engineer? SAP consultant for corporates in the Manufacturing field?)

When you have chosen your target client, refined you CV, found the best Job Platforms, and refined your filters,
this extension will help you track down and identify the best offers for you. *

\* 🚧 This feature is under construction.

## Installation
Follow these easy steps.

1. Download the zip file
2. Move it to a folder where you can keep the extracted files (see recommended folders below)
3. Extract the zip inside the dedicated new folder
4. Open your Chrome browser
5. Follow [Load an unpacked extension instructions](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world#load-unpacked)
   * Navigate to **chrome://extensions**
   * Enable Developer Mode by clicking the toggle switch next to **Developer mode**
   * Click the **Load unpacked** button and select the extension directory *
6. The extension is now installed

<div style="background-color: #f0f0f0; display: inline-block; padding: 0.5rem;">
    <img src="img/install-steps.png" alt="Description of image">
    <p style="font-size: 0.8rem; text-align: center; margin-top: 0.5rem;">How to enable and load unpacked extensions</p>
</div>

**\* Please Note**: the extension directory is the one that contains the **manifest.json** file.

Recommended folders:
* Linux: /home/your-username/Documents/ja-chrome-extension
* Windows: C:\Users\YourUsername\Documents\ja-chrome-extension
* macOS: /Users/YourUsername/Documents/ja-chrome-extension

## Usage

### Prerequisites
The first thing to do once installed the extension is to set the API Key.

To do that, right-click on the extension icon (or open the extensions' menu and then click on the three dots), and then click Options.

![pin-it.png](img/pin-it.png)

![open-options-2.png](img/open-options-2.png)

![open-options-1.png](img/open-options-1.png)

Enter your API Key and click Save. A success message should appear.

![options-page.png](img/options-page.png)

Now you are ready to use the extension.

### Job offer analysis
The first thing you can do is to analyze a job posting page.\
Open the page with your browser, **right-click** on the page, hover over the **Job Analysis** menu item and then select one of:
1. Analyze job
2. Analyze and save job

![context-menu-items.png](img/context-menu-items.png)

**Analyze job** will perform the analysis for the current job posting page and show the results table.

![analysis-result-1.png](img/analysis-result-1.png)

![analysis-result-2.png](img/analysis-result-2.png)

You can choose to save the results in the current project (called "default" if you haven't configured it yet. More details later.)

**Analyze and save job** will perform the same operation and automatically save the result.

### The main panel
The main panel is the most important part of the extension.\
From here you can manage all the aspects of the plugin (except for the api key).

To open the main control panel click on the plugin icon.
A new panel should open on the right side of your screen.

![open-panel.png](img/open-panel.png)

From this panel you can:
* **Configure the "Current project"**. It acts as a folder for your data, you can create multiple projects.
* **Manage the "Link Grabber"**. It grabs job posting links from the page while you navigate (it is available only on certain websites, the list of supported websites is growing).
* **Manage the "Link Scraper"**. It opens in a new tab the grabbed links and extracts the job posting info for the next step: the analysis.
* **Manage the "Job Analyzer"**. It processes the job postings info collected in the previous step.
* **Download the analysis results**. Clicking the Download CSV button you will be able to export a CSV containing all the job posting analysis results. You can then import the file into your preferred CSV reader (Google Sheets, Excel, Open Office, ...)