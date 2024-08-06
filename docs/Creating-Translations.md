<h1 style="text-align:center">
    Creating Translations
</h1>

## Introduction

This document will guide you through the process of creating translations for the VtubersTV project.

## Prerequisites

Before you start creating translations, you need to have the following:

- A GitHub account.
- A text editor.
- A web browser.
- A basic understanding of [JSON](https://www.json.org/json-en.html).
- [Git](https://git-scm.com/) installed on your computer.

## Steps

1. Make a new fork of the repository by clicking on the "Fork" button on the top right corner of the repository page.

    <img src="https://docs.github.com/assets/images/help/repository/fork-button.png" alt="Fork button" width="500">

2. Clone the forked repository to your local machine using Git:

    ```bash
    git clone https://github.com/{YOUR_USERNAME}/localization.git
    ```

    <h5 style="text-align:center">
        Replace {YOUR_USERNAME} with your GitHub username.
    </h5>

3. Navigate to the localization directory to access the localization files for different languages. This directory contains all the files in the repository.

    ```bash
    cd localization
    ```

4. Navigate to the translations directory to access the translation files for different services.

    ```bash
    cd translations
    ```

5. Choose a service you want to translate, and open the corresponding directory to access the translation files.

    For example, to translate the VtubersTV Dashboard (https://dashboard.vtubers.tv), navigate to the dashboard directory:

    ```bash
    cd dashboard
    ```

    <!-- The locale is like this: en-us -->

6. Make a copy of the en-us.json file and rename it to the appropriate locale code for your language. For example, if you are translating to Spanish, the file should be named es-es.json. This follows the [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) standard for language codes.

7. Open the translation files in your preferred text editor and translate the content into your desired language. For this example, we will be using [Visual Studio Code](https://code.visualstudio.com/) as the text editor.

    ```bash
    code {LOCALE}.json
    ```

8. Translate the content in the file to your desired language. Make sure to maintain the JSON structure and formatting while translating the content.

9. Once you have completed the translation, save the file and commit your changes to your forked repository.

    ```bash
    cd ../..
    git add .
    git commit -m "Add {LANGUAGE} translations for {SERVICE}"
    git push
    ```

    <h5 style="text-align:center">
        Replace {LANGUAGE} with the language you translated the content to and {SERVICE} with the name of the service you translated.
    </h5>

10. Create a pull request to merge your changes into the main repository. Go to the main repository page and click on the "New pull request" button.

    <img src="https://docs.github.com/assets/images/help/pull_requests/choose-base-fork-and-branch.png" alt="Create pull request button" width="500">

11. Select your forked repository as the base repository and the main repository as the head repository. Click on "Create pull request" to submit your changes for review.
