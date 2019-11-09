# Automated X-ray NG Tube identification

### Authors
Nimesh Chudasama  
nimeshchudasama1@gmail.com  
Author affiliation, including full address with zip code

Kevin Nguyen  
Author email address  
Author affiliation, including full address with zip code

Cooper Mellema  
Author email address  
Author affiliation, including full address with zip code

Jeon Lee  
Author email address  
Author affiliation, including full address with zip code

Anindita Palit  
axp172130@utdallas.edu  
Author affiliation, including full address with zip code

Yee Seng Ng  
Author email address  
Author affiliation, including full address with zip code

Julian Narvaez  
jmn112@case.edu  
Author affiliation, including full address with zip code

### Abstract
Misplaced enteric tubes can result in significant morbidity, including pneumothorax, pleural effusion, retropharyngeal abscess and lung abscess. In clinical practice, radiographs are used to confirm position of enteric tubes. These radiographs may be reviewed by the primary team or interpreted by the radiologist prior to starting enteral feeding or medications. Although rare, missed malpositioned enteric tubes can lead to catastrophic consequences including patient death. Mistakes in interpretation can occur due to poor image quality, distracting findings on the radiographs (such as presence of other tubes or pathologies) , or consequence of other human error. An accurate algorithm automatically localizing enteric tubes can help reduce such errors. The algorithm could also flag potential positive studies on reading worklists to facilitate prioritization of interpretation by a radiologist, regardless of the length of the reading queue.

We will utilize approximately 1000 abdominal radiographs without enteric tubes and about 1000 radiographs with tubes in place, and bounding box information for localization of the tips of the catheter.  Our goal is to create a solution that can reliably identify whether a tube is present and pretty close at deriving bounding boxes that enclose the terminal tip of the tubes. In the final product, the locations of the terminal tips can be used to identify images containing malpositioned tubes, potentially through statistical means or cluster analysis.

### Keywords
CNN, Radiograph, X-ray, Enteric-tube, Position, Bounding-box, Clinical, Interpretation, Machine Learning

### Introduction
Signicant morbidity, including pneumothorax, pleural effusion, retropharyngeal abscess and lung abscess are all direct results of misplaced enteric tubes. Complications with enteric tubes arise in diverse ways with one such case study showing a "scan of the head revealed that the small-bore feeding tube had violated the cranial base repair and entered the brain stem and spinal cord" (Hanna et al. 2011). 

Clinical impact remains significant. A study of 39 children with inserted tubes showed, "Tube placement error occurred in 43.5% of tubes at least once during the observation period" (Ellett et al. 2005). Another study conducted of 2000 enteric tube insertions showed "13 complications (26% of malpositions), including 2 deaths, which were directly attributed to the feeding-tube malposition" (Sorokin et al. 2006). Complications of misplaced enteric tubes occur across patient populations and result in severe complications.

Detected misplaced enteric tubes can be done with multiple methods however, "[r]adiography remains the gold standard for determining
feeding tube location" (Metheny et al. 2007). Even with the gold standard of enteric tube localization, accurate and timely detection remains an issue. The following image is an example of the radiological images that are reviewed for enteric tube placement:

![](/Users/juliannarvaez/Desktop/EntericTubeExample.png)

These enteric tubes can be difficult to see and radiologists faced with time constraints can easily make mistakes when localizing and reporting these enteric tubes. Reporting information back to the physicans and clinical workers requesting the radiological scan must be completed within an hour. This lack of immediate feedback places time constraints on both the radiologists and clinical workers requesting the radiological scans. In addition, sub-optimal placement is not readily reported and may cause discomfort for patients. 

Having a tool to assist radiologists in reviewing enteric tube scans would decrease incidents of misplaced enteric tubes and increase the efficiency of the scan review process.

### Methods
Insert methods here, with the two required subsections as described below:
Implementation
This section describes how the tool works and relevant technical details for implementation.

### Operation
This section should include the minimal system requirements needed to run the software and an overview of the workflow

### Results
Include if the paper includes novel data or analyses; should be written as a traditional results section (otherwise, include a Use Cases section).

### Use Cases
If not including a Results section, include this section. Examples of input and output files should be provided with some explanatory context. Any novel or complex variable parameters should be explained in sufficient detail to enable users to understand and use the tool's functionality. 

### Conclusion and next steps
This section should include a brief discussion of allowances made (if any) for controlling bias or unwanted sources of variability, and the limitations of any novel datasets. Also, include any next steps for future development (whether your group actually plans to do this or these steps are just included a guidance for potential future development).

### Data and software availability
Source code for new software must be made openly, and permanently available in a structured repository such as Zenodo (the F1000Research team can assist with deposition), as well as uploaded to a Version Control System (VCS) such as GitHub, BitBucket or SourceForge. Please provide details in a section entitled “Software availability”, listing the repository and the license under which the software can be used in the article. Source code must be assigned an open license. 

### Author contributions
F1000R uses the CRediT Taxonomy for author contributions.  For each author, list their contribution(s) from the list below.  Anyone who contributed in another capacity or otherwise does not meet the criteria for authorship (e.g. they did not review the final manuscript) should be included in the acknowledgements.



Contributor Name | Contributor Role |
-----------------|------------------|
Conceptualization | Ideas; formulation or evolution of overarching research goals and aims.|
Data Curation | Management activities to annotate (produce metadata), scrub data and maintain research data (including software code, where it is necessary for interpreting the data itself) for initial use and later reuse. |
Formal Analysis | Application of statistical, mathematical, computational, or other formal techniques to analyze or synthesize study data. |
Funding Acquisition | Acquisition of the financial support for the project leading to this publication. |
Investigation | Conducting a research and investigation process, specifically performing the experiments, or data/evidence collection. |
Methodology | Development or design of methodology; creation of models. |
Project Administration | Management and coordination responsibility for the research activity planning and execution. |
Resources | Provision of study materials, reagents, materials, patients, laboratory samples, animals, instrumentation, computing resources, or other analysis tools.         |
Software | Programming, software development; designing computer programs; implementation of the computer code  and supporting algorithms; testing of existing code components. |
Supervision | Oversight and leadership responsibility for the research activity planning and execution, including mentorship external to the core team. |
Validation | Verification, whether as a part of the activity or separate, of the overall replication/reproducibility of results/experiments and other research outputs. |
Visualization | Preparation, creation and/or presentation of the published work, specifically visualization/data presentation. |
Writing – Original Draft Preparation | Creation and/or presentation of the published work, specifically writing the initial draft (including substantive translation). |
Writing – Review & Editing | Preparation, creation and/or presentation of the published work by those from the original research group, specifically critical review, commentary or revision – including pre- or post-publication stages. |

### Competing interests
Note any financial, personal, or professional competing interests for any of the authors that could be construed to unduly influence the content of the article. If none, include the text ‘No competing interests were disclosed.’

### Grant information
Include funding if relevant (including funding from authors’ employers if relevant, and any relevant grant funding).  If none, include the text ‘The author(s) declared that no grants were involved in supporting this work’. 

###Acknowledgements
This  section should acknowledge anyone who contributed to the research or the writing of the article but who does not qualify as an author; please clearly state how they contributed. Authors should obtain permission to include the name and affiliation, from all those mentioned in the Acknowledgments section.

### References
Instructions on using the F1000R Google docs plug in for reference management: http://f1000.com/work/faq/google-docs-add-on/1

Instructions on using the F1000R Word plug in for reference management: http://f1000.com/work/faq/word-plugin 

### Figures and Tables
All figures and tables should be cited and discussed in the article text. Figure legends and tables should be added at the end of the manuscript. Tables should be formatted using the ‘insert table’ function in Word, or provided as an Excel file. Files for figures should be uploaded as separate files through the submission system. Each figure or table should have a concise title of no more than 15 words. A legend for each figure and table should also be provided that briefly describes the key points and explains any symbols and abbreviations used. The legend should be sufficiently detailed so that the figure or table can stand alone from the main text. 
Images (not necessary, but why not)
Photographs and microscopy images: Photographs and microscopy images should be submitted as uncompressed TIFFs with a resolution of at least 300dpi at the size they are likely to be displayed (see above).

Mixed images: Images that are a mix of half-tone images and line art (e.g. annotated gels or images with scale bars) should be submitted as TIFF files at a resolution of 500dpi or vector files (e.g. EPS or Adobe Illustrator files). Please ensure that the text size is at least 8pt and lines are thick enough to be clearly visible at the size the image will be displayed.

Images to be used as data: If you are submitting photographic images as part of your raw dataset, please submit them as uncompressed TIFF files.

