# AUTOMATED ALGORITHM FOR DETECTING AND LOCALIZING ENTERIC TUBES TO FACILITATE ACCURATE AND TIMELY RADIOGRAPHIC INTERPRETATION

## Needs Statement

#### Problem
A more time-efficient and accurate means of detecting misplaced and sub-optimal enteric tube placement

#### Population
Intubated patients, especially with altered mental states or an inability to protect their airways

## Background

Misplaced enteric tubes can result in significant morbidity, including pneumothorax, pleural effusion, retropharyngeal abscess and lung abscess. In clinical practice, radiographs are used to confirm position of enteric tubes. These radiographs may be reviewed by the primary team or interpreted by the radiologist prior to starting enteral feeding or medications. Although rare, missed malpositioned enteric tubes can lead to catastrophic consequences including patient death. Mistakes in interpretation can occur due to poor image quality, distracting findings on the radiographs (such as presence of other tubes or pathologies) , or consequence of other human error. An accurate algorithm automatically localizing enteric tubes can help reduce such errors. The algorithm could also flag potential positive studies on reading worklists to facilitate prioritization of interpretation by a radiologist, regardless of length of the reading queue.

![Alt text](images/0331.png)

We will utilize approximately 1000 abdominal radiographs without enteric tubes and about 1000 radiographs with tubes in place, and bounding box information for localization of the tips of the catheter.  Our goal is to create a solution that can reliably identify whether a tube is present and pretty close at deriving bounding boxes that enclose the terminal tip of the tubes. In the final product, the locations of the terminal tips can be used to identify images containing malpositioned tubes, potentially through statistical means or cluster analysis. 

![Alt text](images/Heatmap0331.png)

Team Leads: Travis Browning, MD and Ye Seng Ng, MD, Emergency Medicine, profiles.utsouthwestern.edu/profile/42192/travis-browning.html 

![Alt text](https://images.squarespace-cdn.com/content/v1/5b3ffc3fcef3721bd81d8c60/1559312908014-U0GOGORXOYIS0UJQV43H/ke17ZwdGBToddI8pDm48kLSRW7PLm3WkubOqe1a7DDVZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpyGgy-SgXO0EeFY0JziBd3dD9HtJ7Bi1hLUqRY0vXhnJ17ynhB4yX2qIiJJUVq2E2g/browning1.png?format=1500w)


