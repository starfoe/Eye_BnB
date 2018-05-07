
Eye BnB

Business Understanding

•	This project will help users find their favorite lodging during their travel, based on images or some descriptions that the users upload

•	It will provide value to:
  o	People who are looking for adding more fun, passion and excitement to their travel 
  o	Apartment owners who want to know how many apartments in the same city looks like theirs so that they can make their apartments   either discriminative or closer to the apartments which are already popular. 

Data Understanding

•	Airbnb publicized their own datasets from which I can get a list of all the apartments in certain cities in the U.S. and collect basic information of the apartments
•	With the list above, I can scrape images and highlight tags of each apartment with BeautifulSoup and Request

Data Preparation

•	Online collection
  o	Raw data is the basic information of Airbnb apartment (location, descriptions, price range, webpage URL) which can be found in the datasets publicated by Airbnb. It will be saved in MongoDB on AWS
  o	With the webpage URL gotten from above, images of each apartment will be scraped by BeautifulSoup and Request
  o	Highlight tags and some reviews will also be scraped and saved
  o	All the data will be saved to MongoDB on AWS

•	Offline processing:

  o	For each apartment in the DB, extract certain features from its images and save to an excel spreadsheet (with its ID) 
  o	Put highlight reviews to the excel spreadsheet for further uses
  
Modeling

•	Similarities calculation
  o	Eculidean Distance
  o	Cosine Distance
  
•	Image feature extraction
  o	Color：RGB
  o	Fourier transform based features
  o	others

Evaluation

•	Visualization: look at all the recommendations and conceptually check if they make sense

Deployment

•	Step1: given a picture, the system can return places looks similar (of the same style)
•	Step2: users can add some word descriptions to what they dream of going ( industrial style, splendid..) to make the searching more precise


favorite
61
I've been using Markdown for class notes, and it's great. I even do some preprocessing on the Markdown so I can do things like tables. But this term I'm teaching a class with a lot of math, and I'd love to be able to put LaTeX formulas with Markdown, something like this:
The refinement relation is written $a \sqsubseteq b$, which can be 
pronounced "$a$ approximates $b$" or "$b$ is at least as defined as $a$".

