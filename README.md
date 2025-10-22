<!--
title: "Liascript Presentations"

import: https://raw.githubusercontent.com/LiaScript/CodeRunner/master/README.md
        https://raw.githubusercontent.com/LiaTemplates/BeforeAndAfter/0.0.1/README.md

icon:   https://styleguide.ugent.be/files/uploads/logo_UGent_EN_RGB_2400_kleur_witbg.png

link:   https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
        https://fonts.googleapis.com/css?family=Lato:400,400italic,700
        style.css

@runR: @LIA.eval(`["main.R"]`, `none`, `Rscript main.R`)

@JSONLD
<script run-once>
  let json = @0 

  const script = document.createElement('script');
  script.type = 'application/ld+json';
  script.text = JSON.stringify(json);

  document.head.appendChild(script);

  // this is only needed to prevent and output,
  // as long as the result of a script is undefined,
  // it is not shown or rendered within LiaScript
  console.debug("added json to head")
</script>
@end

@style
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 10px;
}

.flex-child,
.flex-child-1 { flex: 1; }
.flex-child-2 { flex: 2; }
.flex-child-3 { flex: 3; }
.flex-child-4 { flex: 4; }
.flex-child-5 { flex: 5; }
.flex-child-6 { flex: 6; }
.flex-child-7 { flex: 7; }
.flex-child-8 { flex: 8; }

@media (max-width: 500px) {
    .flex-child,
    .flex-child-1,
    .flex-child-2,
    .flex-child-3,
    .flex-child-4,
    .flex-child-5,
    .flex-child-6,
    .flex-child-7,
    .flex-child-8 {
        flex: 100%; /* Makes the child divs take up the full width on slim devices */
        margin-right: 0; /* Removes the right margin */
    }
}
@end

link:   https://unpkg.com/leaflet@1.9.4/dist/leaflet.css
script: https://unpkg.com/leaflet@1.9.4/dist/leaflet.js

-->

# Preserving data at UGent
![img1](https://images.pexels.com/photos/158827/field-corn-air-frisch-158827.jpeg "Corn Fields Under White Clouds With Blue Sky during Daytime, by Pixabay from Pexels https://www.pexels.com/photo/corn-fields-under-white-clouds-with-blue-sky-during-daytime-158827/, CC0") This course shortly explains the role of data preservation in research verification and reuse, the main steps to preserve data and helps researchers decide which location is most suitable to preserve their data.

- Contact: (Name), Data Steward, Team Open Science, University Library. rdm.support@ugent.be
- Learning outcomes:
  • Describe the reasons why data should be preserved
  • Outline the basic steps of preservation, including data appraisal/selection
  • Choose a suitable preservation medium for their data
- Eligibility for participation: Any researcher can watch their video at their own pace. Familiarity with Ghent University ICT/storage infrastructure is recommended. 

## Data preservation in a nutshell

<iframe 
  width="800" 
  height="450" 
  src="https://www.youtube.com/embed/UaiRAI-fwmw" 
  title="Knowledge clip: Preserving Data" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

## What do we mean by preservation

Preserving means more that simply not deleting data. **Preservation means**:

> Actions to prevent data from becoming unavailable and unusable over time, for example because of: 

* ‘Owners’ leaving
* Outdated software or hardware
* Storage media degradation
* A lack of sufficient descriptive and contextual information to keep data understandable

## Why preserve data?

> Why is it important to preserve data? (Select **all** that apply.)

<!-- data-randomize -->
[[X]] To ensure future access and reuse of valuable information  
[[X]] To enable verification and reproducibility of research results  
[[ ]] To reduce the total amount of stored information in the world  
[[X]] To protect cultural and historical heritage  
[[ ]] Because data automatically preserves itself over time  
[[X]] To comply with legal and ethical requirements  

---
<!-- data-randomize -->
> What are some risks of **not** preserving data properly? (Select **all** that apply.)

[[X]] Loss of irreplaceable research results  
[[X]] Inability to reproduce experiments or findings  
[[ ]] Increased innovation through data loss  
[[X]] Damage to institutional or scientific credibility  
[[ ]] Improved security through deletion of all old data  

---

## Preserving data in practice


<iframe
  src="https://ugent.h5p.com/content/1291866917768823107/embed"
  aria-label="Data preservation in steps"
  width="800"
  height="600"
  frameborder="0"
  allowfullscreen="allowfullscreen"
  allow="autoplay *; geolocation *; microphone *; camera *; midi *; encrypted-media *">
</iframe>
<script src="https://ugent.h5p.com/js/h5p-resizer.js" charset="UTF-8"></script>

## License and citation

This course is licensed under a [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.en). Please cite it as:

> Oset, Paula. Blablablaba.... [![DOI](https://sandbox.zenodo.org/badge/1080457223.svg)](https://handle.test.datacite.org/10.5072/zenodo.389626)
 

```json   @JSONLD
{
  "@context": "https://schema.org/",
  "@type": "LearningResource",
  "@id": "https://elixir-europe-training.github.io/ELIXIR-TrP-TeSS/",
  "http://purl.org/dc/terms/conformsTo": {
    "@type": "CreativeWork",
    "@id": "https://bioschemas.org/profiles/TrainingMaterial/1.0-RELEASE"
  },
  "description": "TeSS, how can I help you? This is our interactive hands-on course about efficient use of the ELIXIR TeSS platform.",
  "keywords": "FAIR, OPEN, Bioinformatics, Teaching, TeSS",
  "name": "TeSS, how can I help you?",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "educationalLevel": "beginner",
  "competencyRequired": "none",
  "teaches": [
    "search events and material in TeSS via direct and faceted search",
    "add manually and automatically events and material to TeSS",
    "extract events and material from TeSS by using TeSS widgets"
  ],
  "audience": "training providers",
  "inLanguage": "en-US",
  "learningResourceType": [
    "tutorial"
  ],
  "author": [
    {
      "@type": "Person",
      "name": "Bruna Piereck"
    },
    {
      "@type": "Person",
      "name": "Olivier Sand"
    },
    {
      "@type": "Person",
      "name": "Alexander Botzki"
    }
  ],
  "contributor": [
    {
      "@type": "Person",
      "name": "Yasmine Maes"
    },
    {
      "@type": "Person",
      "name": "Finn Bacall"
    },
    {
      "@type": "Person",
      "name": "Munazah Andrabi"
    }
  ]
}
```
