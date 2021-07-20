# RateMyProfessorScraper

A simple scraper to extract information about a professor off of RateMyProfessors.

To use the scraper:
```py
professor = RateMyProfScraper(schoolId=xxx, firstName="xxx", lastName="xxx")
```

Example:
```py
professor = RateMyProfScraper(schoolId=1258, firstName="Maria", lastName="Aarnio")
print(professor) #{"rating":"4.8", "num_ratings":3, "dept":"Philosophy"}
```

To access a specific part of the returned JSON object:
```py
professor["rating"] #4.8
professor["num_ratings"] #3
professor["dept"] #Philosophy
```

To return a link to the professor's RateMyProfessors page:
```py
professor.professor_link #https://www.ratemyprofessors.com/ShowRatings.jsp?tid=1774527
```
