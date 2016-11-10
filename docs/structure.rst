The IT Architecture of the UBN Project
======================================

General Architecture
--------------------

- Door43/en-ubn - the UBN home page that contains information pertinent and links to all the other UBN repos
- Door43/en-ubn-articles - the repo that contains the articles that will be linked from both the UBN notes and UBC
- Door43/en-ubn-xxx - each biblical book has its own repo

Specific Architecture
---------------------

Door43/en-ubn 
-----
Homepage of the UBN
1. Location of all files that are for global reference/use

2. Links to all other biblical book repos on the main readme file.

3. The explanation of the UBN project

4. The volunteer job description

5. A link to this present document


Door43/en-ubn-xxx, 
----
(where xxx = three-letter code for any biblical book). 

Here is where to locate the working files for the UBN (i.e., the files containing the notes as they are being composed and edited):

- All writers and manager-revisers will do their work online in one of these repositories. Each biblical book repository will contain the working notes created for that book.
- Each chapter of the book will have its own file. For example: Luke 1 will have the following chapter URL: https://git.door43.org/Door43/en-ubn-luk/src/master/content/01.md  

So that the directory tree for any book will look like: (Psalms will be 3 digit numbers)Content		01.md		02.md		intro.md

Directory Structure
-------------------




Content
-------

The folder structure of the content directory in resource containers are mostly the same. Differences between resource types may include the absense of some files or the inclusion of others.

Note: that where a .txt extension is shown below, the proper extension should be used according to the content_mime_type indicated in the package.json. For example .usfm or .md.

.. code-block:: none

    content/
        |-config.yml
        |-toc.yml
        |-01/
        |    |-title.txt
        |    |-sub-title.txt
        |    |-intro.txt
        |    |-reference.txt
        |    |-summary.txt
        |    |-01.txt
        |    |-02.txt
        |    ...
        ...
        |-front/
        |-back/
        ...

The directories shown above indicate chapters except for the two reserved folders `front` and `back` which contain, if applicable, the front matter and back matter of the container.

The files within each chapter represents the chunks of the chapter. Within each folder are additional reserved files:

- title
- sub-title
- intro
- reference
- summary



