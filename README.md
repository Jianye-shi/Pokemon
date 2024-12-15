# GROUP_L: A Fantastic Adventure: Pokémon  

## Overview
This project presents a comprehensive analysis of virtual creatures from various gaming universes, including Pokémon, Palworld, Roco Kingdom, and SEER. The study employs data science methods, including data mining, deep learning models (ResNet and U-Net), and image processing techniques, to scrutinize these creatures and investigate the nuances and distinctions between them. The objective is to shed light on the ongoing debate about game design and intellectual property, and to offer insights that can guide the creation of future games that respect creativity and legal standards.

## Dataset 
The Dataset of this project contains 2 parts: pictures and info of pets in different games. All the data is stored in the file '/data', and because of the limitation of the git platform, we couldn't upload so such pictures, so all the pictures are stored in .rar files.
## Methodology

### Data Collection
- **Pokémon**: Data was collected using the PokéAPI, retrieving essential details such as names, types, and image links, which were stored in JSON format. Images were archived in a dedicated folder.
- **Palworld**: Data was extracted from the Palworld wiki using web scraping techniques, with creature names and elements organized into a DataFrame and saved as a CSV file. Images were scraped and stored using Beautiful Soup.
- **Roco Kingdom**: Data was collected by automating interactions with the Roco Kingdom wiki using selenium, navigating through categorized pages to gather pet information from 2010 to 2014. Images were retrieved using urllib.request due to server restrictions.
- **SEER**: Data was scraped from both the official SEER website and its wiki page. Textual information was saved to CSV files, and images were downloaded using urllib.request.

### Models and Techniques
- **U-Net**: Employed for image segmentation tasks due to its ability to maintain high-resolution features throughout the network, making it suitable for comparing fine-grained details and contours of creatures.
- **ResNet**: Used for image classification tasks and feature extraction, recognized for its robustness in handling deep networks and its efficiency in recognizing attributes and similarities across a diverse set of creatures.

## Experiments

### Task1: Data Mining
- Collected and organized data from Pokémon, Palworld, Roco Kingdom, and SEER, including creature names, types, elements, and images.
- Encountered issues with image retrieval due to server restrictions and website protection systems, resulting in partial data collection for SEER.

### Task2: Training of Pokémon Type
- Used a specialized dataset of Pokémon images linked to their types (e.g., grass, fire, water).
- Trained a pre-trained ResNet18 model to predict Pokémon types.
- Achieved good generalization capability with a final test loss close to the validation loss.

### Task3: Analysis of Types from Other Games
- Applied the trained ResNet model to predict the top three attributes for images with the Dark attribute from other games.
- Visualized the distribution of predicted attributes using bar charts and histograms.
- Analyzed the model's confidence levels for each attribute rank.

### Task4: Most Similar Pokémon
- Used ResNet18 for pet attribute recognition and similarity comparison across different games.
- Explored U-Net for image segmentation tasks but found it did not outperform ResNet in this specific task.
- Evaluated various similarity calculation methods, including cosine similarity and hashing.

## Conclusion
The study has provided valuable insights into the complex interplay between game design, intellectual property, and data science. The U-Net and ResNet models were instrumental in illuminating the unique characteristics of virtual creatures from different gaming platforms. ResNet's efficiency and robust feature extraction capabilities made it particularly suited for comparative analysis. The study demonstrates the potential of data science to enrich the gaming industry and society at large, contributing to a more nuanced appreciation of virtual creatures in our digital culture and the need for responsible game design.

## References
The report cites various references, including academic articles, online sources, and technical papers, to support its findings and methodology. These references are listed at the end of the report and can be accessed for further reading.
