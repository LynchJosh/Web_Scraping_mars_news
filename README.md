# Web_Scraping_mars_news



The purpose of this repository was to utilise web scrapping to grab News headlines and descriptions. Another aspect of this challenge was to gather temperature data from an extensive array of Mars data charts.


# 	Part 1

for element in news_element:
    title_element = element.find('div', class_="content_title") 
    preview_element = element.find('div', class_="article_teaser_body")
    
    news_title_dict = {
        "title": title_element,
        "preview": preview_element
    }
    news_title_list.append(news_title_dict)   




#	Part 2 

min_temp =mars_temp_data.groupby('month').mean().sort_values('month')
min_temp

![part 2 example](https://user-images.githubusercontent.com/112728628/208538780-0fc6ce87-193b-4d93-a5c3-d090ac0dd1e6.PNG)

