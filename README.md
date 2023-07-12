# Nissan North America - Capstone Project (Spring 2023)
This is the codebase for the Nissan Capstone Project. 

The project seeks to find what automobile features that customers care about and pain points faced by customers and attempting to understand what features could solve it for them. This is done across both Non-EV and EV vehicles which represent 137 Models and 23 Companies for Non-EV vehicles and 42 models and 23 companies for EV vehicles. Customer Reviews and Comments are scraped from Edmunds.com, Youtube.com, Cars.com and KellyBlueBook(KBB.com) through the use of Open source Web Scraping libraries like beautifulsoup4 and Google's official YoutubeV3API in case of Youtube. The Information Extraction, Semantic Condensation pipeline is performed using OpenAI's ChatGPT API and Prompt Engineering which the Semantic Tagging is performed using the Sentence Transfromers Library.

The whole corpus is "condensed" into a semantic master list of automobile features across Positive, Negative and Wishlist categories and each comment is tagged into one of the same. The resulting analysis supports segmentation across various market cross-sections like Vehicle Make, Model, Year of Production and Model which allows for both broad and granular analyses within a comapany and across competitors while also offering robust insights. 

The Presentation PDF file and the project report provides a detailed overview/flowchart of the pipeline as well as sample results, documentation of challenges, limitations and future work as well as details on alternative approaches attempted. 

In general, these notebooks can be run with API keys being provided by the user. Due to the nature of running certain files in batches across multiple instances, the file names would have to be changed as and when required but the codebase should otherwise be able to run from top to bottom seamlessly. 

EVs - Same file but operation is performed for Provided Electric Vehicles of interest. Otherwise the files correspond to Non-Electric Vehicles

1. Metadata_Cleaning: Cleaning performed on the Original Vehicle Segments to be used further in other notebooks.
2. Metadata_Cleaning_EV: Cleaning performed on the Original Vehicle Segments to be used further in other notebooks. - EVs
3. Cars_CustomerReview_Scrape: WebScraping Customer Comments of Vehicles from VehicleSegments from Cars.com
4. Cars_CustomerReview_Scrape_EV: WebScraping Customer Comments of Vehicles from VehicleSegments from Cars.com - EVs
5. Edmunds_CustomerReview_Scrape: WebScraping Customer Comments of Vehicles from VehicleSegments from Edmunds.com
6. Edmunds_CustomerReview_Scrape_EV: WebScraping Customer Comments of Vehicles from VehicleSegments from Edmunds.com - EVs
7. KBB_CustomerReview_Scrape: WebScraping Customer Comments of Vehicles from VehicleSegments from KBB.com
8. KBB_CustomerReview_Scrape_EV: WebScraping Customer Comments of Vehicles from VehicleSegments from KBB.com - EVs
9. Youtube_Comments_Scraping: WebScraping Customer Comments of Vehicles from VehicleSegments from Youtube's comments section
10. Youtube_Comments_Scraping_EV: WebScraping Customer Comments of Vehicles from VehicleSegments from Youtube's comments section - EVs
11. GPT3.5TurboInformationExtraction: Information Extraction part of the Pipeline using ChatGPT and Prompt Engineering
12. GPT3.5TurboInformationExtraction_EV: Information Extraction part of the Pipeline using ChatGPT and Prompt Engineering - EV Version
13. GPT3.5TurboSemanticCondenser: Semantic Compression part of the pipeline using ChatGPT and Prompt Engineering in a recursive fashion.
14. GPT3.5TurboSemanticCondenser_EV: Semantic Compression part of the pipeline using ChatGPT and Prompt Engineering in a recursive fashion. - EV Version
15. Reddit_Scraping: WebScraping Reddit Threads from the Nissan Sub-Reddit (Unused in the Analyses) 
16. Similarity_Analysis: Sentence Similarity aspect of the pipeline using Sentence Transformers
17. Similarity_Analysis_EV: Sentence Similarity aspect of the pipeline using Sentence Transformers - EV Version
18. LegacyCodeDump: Legacy pieces of code used for testing, debugging and alternative methods tried held as an archive.
19. Nissan_Segment_List: List of Vehicles (Non-EVs) and their associated metadata provided by Nissan which was of interest in this analysis.
20. EV_Model_List: List of Vehicles (EVs) and their associated metadata provided by Nissan which was of interest in this analysis.
21. Nissan_Capstone_Presentation: Capstone Powerpoint Presentation
22. Nissan_Capstone_FinalReport: Capstone Final Report 
