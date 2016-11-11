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
--
Homepage of the UBN

1. Location of all files that are for global reference/use

2. Links to all other biblical book repos on the main readme file.

3. The explanation of the UBN project

4. The volunteer job description

5. A link to this present document


Door43/en-ubn-xxx
--
(where xxx = three-letter code for any biblical book). 

Here is where to locate the working files for the UBN (i.e., the files containing the notes as they are being composed and edited):

- All writers and manager-revisers will do their work online in one of these repositories. Each biblical book repository will contain the working notes created for that book.
- Each chapter of the book will have its own file. For example: Luke 1 will have the following chapter URL: https://git.door43.org/Door43/en-ubn-luk/src/master/content/01.md  

So that the directory tree for any book will look like: 

.. code-block:: none

    en-ubn-xxx/
        |-.github
        |-content/
        |-license
        |-readme.md
  
The directories shown above indicate chapters except for the two reserved folders `front` and `back` which contain, if applicable, the front matter and back matter of the container.

Content
----

The folder structure of the content directory. (Psalms will be 3 digit numbers)

.. code-block:: none

    content/
         |-01.md
         |-02.md
         |-intro.md


Door43/en-ubn-articles
----
In this repo are articles that will be linked from both the UBN and UBC. https://git.door43.org/Door43/en-ubn-articles

- Here is where to locate the working files for the glossary and articles - as they are being composed and edited.
- The ‘rejected’ file with the list of items requested that have been rejected by manager-revisers as necessary. 
- Each glossary and article item will have its own folder in the content folder in the repository. 
  - The Glossary entry will be the 01.md file in the folder. The working glossary entries as they are proposed and then written by the UBN team or others.
  - The Article entry will be the 02.md file in the topic folder. The working articles as they are requested by the UBN team and then written by the UBC team or others.
  So that the directory tree will look like:
  
.. code-block:: none
  
      content/
            |-Topic/
            |   |-01.md
            |   |-02.md
           

REMARK: however, we expect that some articles will not be associated with any glossary term.
