The Following Project aims to demonstrate my understanding of FastApi

This project implement's CRUD  operations

@app.get("/")
def index(): #Displays all the news

@app.get("/get-by-title")
def get_byTitle(title : Optional[str] = None): #Displays News By Title

@app.post("/post-news/{news_id}")
def create_news(news_id : int, n : News):#Used for creating News By Id

@app.post("/post-news")
def create_newsUrl(url : Optional[str] = None):#Used For Creating News by giving url

@app.delete("/delete-News/{news_id}")#Delete by news id
def delete_news(news_id: int)

@app.delete("/delete-News")
def delete_newsTitle(title : Optional[str] = None):#Delete by News Title

@app.put("/update-news/{news_id}")
def update_news(news_id: int, student: UpdateNews):#Update the news