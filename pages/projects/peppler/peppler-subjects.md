---
title: Subjects in the Jim Peppler Collection
layout: page
permalink: /jim_peppler_subjects.html
---

## Subjects in the Jim Peppler Collection

### Visualizations

With 199 subjects ranging in content from to Black social life to disc jockeys and funerals, the Jim Peppler _Southern Courier_ Collection provides unique insight into the joy and despair of the 1960s in America.

Click on any of the subject headings to view photos of that subject from the Jim Peppler _Southern Courier_ Collection on the [Alabama Department of Archives and History’s digital collections site](https://digital.archives.alabama.gov/digital/collection/peppler).

<div class='tableauPlaceholder' id='viz1669254970321' style='position: relative'><noscript><a href='#'><img alt='15 Most Used Subject Headings in the Jim Peppler Southern Courier  Collection ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Su&#47;SubjectsInJimPeppler&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='SubjectsInJimPeppler&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Su&#47;SubjectsInJimPeppler&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                

<script type='text/javascript'>                    var divElement = document.getElementById('viz1669254970321');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

The below list contains the names of all 199 subjects tagged in the collection, the associated number of photographs, and the percentage of photos in the whole collection that the subject appears in. Darker colors mean that the subject appears in the collection more frequently.

<div class='tableauPlaceholder' id='viz1669254982017' style='position: relative'><noscript><a href='#'><img alt='All Subjects Used in the Jim Peppler Southern Courier Collection ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Al&#47;AllSubjectsJimPeppler&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='AllSubjectsJimPeppler&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Al&#47;AllSubjectsJimPeppler&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                

<script type='text/javascript'>                    var divElement = document.getElementById('viz1669254982017');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

### Topic Modeling 

While the standardized subject headings for the places, peoples, and subjects represented in the collection tell us a great deal about the materials that are being desribed, they do not fully represent every aspect of the metadata available. The free-text descriptions used in the title and description text fields provide additional information that is not represented in the subject headings. 

I used MALLET and NLTK to identify topics and language that would be necessary to edit or remove to reveal the the topics respectively. But what do I mean by "edit or remove"? Isn't it important to see the data as it exists in its original state?  Well: yes and no! In many cases when analyzing a corpus of text, data has been pre-processed to exclude what are called "stopwords". Stopwords might include the usual subjects such as "a", "an", "the", "was" and similar terms. These are some of the most common words in the English language, so it makes sense to remove them as their frequency will give them undue weight. 

Here is the list of [default MALLET stopwords](https://github.com/elizajames/Stand-Alone-Projects/blob/master/Southern%20Courier/MALLET_default_stopwords). You'll note that some of them are less straightforward and obvious, and it's important to consider that the stopwords we choose to use will impact the final analysis of the metadata. Understanding the natural state of the metadata and the additional stopwords that were required for me to focus in on the metadata that captured the information I found most relevant is critical to fully understanding why I analyzed the metadata I did.

The metadata describing this collection includes language that is highly repetitive and can work similarly to stopwords to mask the data we actually want to look at. To provide transparency for this project, I chose to replace duplicative language with "stub" language to allow the duplicative language to be represented but not have the individual words overrun the resulting topic topic model. I chose to edit the original data with the language I identified in the file available [on the project folder on Github](https://github.com/elizajames/Stand-Alone-Projects/blob/master/Southern%20Courier/additional_stopwords).

[Back to project page](https://elizajames.github.io/jim_peppler.html)