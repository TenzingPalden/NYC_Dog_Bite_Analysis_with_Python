# NYC_Dog_bites_Python_analysis
Welcome to the NYC Dog Bite Data Analysis project! This project aims to investigate the statistics and trends related to dog bites in New York City from 2015 to 2021. Utilizing Python, particularly the Plotly package, I generated visually compelling interactive graphs to gain insights into this humorous yet concerning public health issue. The primary goal of this project is to analyze the NYC Dog Bite dataset and address key questions surrounding incidents of dog bites during the specified time frame. 

Plotly Express is a high-level data visualization library in Python that provides an easy-to-use interface for creating a wide range of interactive plots. 
```Python
import plotly.express as px

df = pd.read_csv("DOHMH_Dog_Bite_Data.csv")
dog_breeds=dog_breeds.drop("UNKNOWN")
```

# Bar Chart of the Top 20 Dog bite Breed occurrences in NYC
```Python
fig = px.bar(dog_breeds[:20], text_auto=True, title="Top 20 Dog Breeds that Bit Humans in NYC")
fig.show()
```
<img src="https://github.com/TenzingPalden/NYC_Dog_bites_Python_analysis/assets/85039775/6a3d6466-a3ce-4125-8d6a-cc1737fadd01" alt="Image Description" width="1200"/>

# Pie chart of the Top 20 Dog bite Breed occurrences in NYC

```Python
fig2= px.pie(dog_percent[:20], values="Breed", names=dog_percent.index[:20])
fig2.show()
```
<img src="https://github.com/TenzingPalden/NYC_Dog_bites_Python_analysis/assets/85039775/c93018b3-6187-4bd0-a121-4330e7387110" alt="Image Description" width="800"/>

#  Pie chart of the Dog Bite occurrences by borough

```Python
fig2= px.pie(dog_percent[:20], values="Breed", names=dog_percent.index[:20])
fig2.show()
```
<img src="https://github.com/TenzingPalden/NYC_Dog_bites_Python_analysis/assets/85039775/abbf636a-fda9-4b3e-b068-0acfaed7ffca" alt="Image Description" width="800"/>

# Bar Chart of Dog Bite Count from 2015 to 2021
```Python
fig2= px.pie(dog_percent[:20], values="Breed", names=dog_percent.index[:20])
fig2.show()
```
<img src="https://github.com/TenzingPalden/NYC_Dog_bites_Python_analysis/assets/85039775/0ca7008a-1633-4c84-bfb4-8465d8d52d9f" alt="Image Description" width="800"/>

# Conclusion
The analysis of dog bite data in NYC from 2015 to 2021 has revealed valuable insights into the prevalence and nature of dog bite incidents in the city as well as serving as a great way for me to practice and hone my Python and Pyplot skills. Through a thorough examination of the dataset, it has become evident that pit bulls emerged as the most common aggressors in dog bite attacks during this period. This finding underscores the importance of awareness and responsible ownership practices to mitigate the risks of dog bites.

# Future Thoughts

 For the future of this project, I think investigation into factors contributing to dog bite incidents, such as breed-specific behaviors and age of the animal, and external characteristics, can provide a more nuanced understanding of the issue. Additionally, implementing targeted educational initiatives and policies to promote responsible pet ownership and canine behavior training can play a pivotal role in reducing dog bite incidents in NYC and beyond.
