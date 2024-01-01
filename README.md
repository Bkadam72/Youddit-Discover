# Youddit-Discover

This research explores the interplay between YouTube's global video content and Reddit's community discussions in today's interconnected digital landscape. 
                    As these platforms significantly impact public discourse, it's vital to understand how content on one affects the other. 
                    Our study investigates the influence of trending YouTube videos on user engagement and sentiment in various Reddit communities. 
                    We use quantitative analysis of YouTube video data and qualitative assessment of Reddit discussions to connect data-driven trends with community reactions. 
                    This investigation into the interactions between these digital giants aims to uncover patterns of digital influence and user behavior. 
                    It provides a thorough insight into the dynamics of cross-platform content in the modern digital ecosystem. 
                    The study also acknowledges challenges like limited data access and rapidly evolving social media policies and privacy issues, offering a realistic perspective on digital media research challenges.

                    We did a strong analysis of the Reddit and Youtube videoes. We extracted most popular music trending videoes and post from the Youtube api and Reddit api. 
                    We alsoo extracted comments on all the trending post and videos from the trending Videos and post we extracted. 
                    This Project involves the collection, analysis and visualization of data using Python programming language. The main aim of this project 
                    
                    Sentiment Analysis of Comments on trending Post and videoes : We investigate the variation in sentiment polarity within comments across different subreddits. 
                    This analysis is aimed at understanding the overarching mood or opinion prevalent in these communities.While for the inpact/sentiment analysis we This code connects to a MongoDB database to analyze the sentiment of YouTube video comments. 
                    It uses the NLTK and TextBlob libraries for sentiment analysis. First, the code connects to a specific collection in the database, then iteratively processes each comment. 
                    For each comment, it calculates sentiment scores using both NLTK's Sentiment Intensity Analyzer and TextBlob's sentiment polarity. 
                    These scores are aggregated and averaged per video. Finally, it categorizes the average sentiment as positive, negative, or neutral based on the score. 
                    This helps in understanding the overall sentiment of the audience for each video in the database.

                    Engagement Trends in YouTube Music Videos: Our research focuses on identifying trends in viewer engagement with trending YouTube music videos. 
                    We look specifically at how this engagement, measured through likes and views, correlates with one another.
                    This Python script leverages Dash to create an interactive web dashboard for analyzing YouTube trending videos and comment toxicity. 
                    It connects to a MongoDB database to fetch data about trending music videos and video comments, processing them into pandas DataFrames. 
                    Key functionalities include calculating engagement rates for videos, generating a word cloud from video titles, and encoding it for display on the dashboard. 
                    The layout integrates HTML and Graph components, featuring a dropdown for metric selection and various interactive graphs, such as bar charts for top videos by selected metrics, average engagement rates by channel, and top channels by video count, along with a correlation heatmap and histograms for comment toxicity. 
                    Here for this dashboard we tried to offer a dynamic and comprehensive visualization of YouTube video engagement and user interactions, providing valuable insights through user-friendly interfaces.

                    Toxicity in YouTube Video Comments: The third aspect of our research involves analyzing the distribution of toxicity in comments on YouTube videos. 
                    We aim to identify and characterize the most toxic comments, looking at patterns and commonalities among them. 
                    Here to achieve the toxicity of the comments we wrote a python code where the script analyzes and updates the toxicity scores of comments in a MongoDB database using the HateModerateSpeech API. 
                    The `get_toxicity_score` function sends each comment to the API and processes the response. 
                    If the API call is successful, it returns the toxicity data; otherwise, it logs an error. 
                    In the `analyze_and_store_comments` function, the script connects to a specific MongoDB collection, retrieves comments, and uses `get_toxicity_score` to assess each one. 
                    The toxicity score is determined based on the API's classification of the comment as 'toxic' or 'non-toxic', and the confidence level provided in the response. 
                    The script then updates the MongoDB collection with these toxicity scores for each comment.
                    Parameters such as database and collection names, API URL, API key, and MongoDB URI are set for execution. 
                    The script demonstrates a practical application of API integration for sentiment analysis in a database context, showcasing automated data processing and storage enhancement techniques. 
                    This approach is beneficial for analyzing large volumes of text data, such as user comments, for sentiment or toxicity.
                    This code snippet is a callback function for a Dash app. It updates a graph to display the top ten most toxic comments, sorted by their toxicity scores. 
                    The graph is a bar chart showing comments on the x-axis and their toxicity levels on the y-axis.

                    This Project aimed to answer the above analysis and. We used Python faktory as backgroud to extract the data from the api. 

How to run code - 
                    1. Login into the vm
                    2. Start the environment by 
                        source myenv/bin/activate 
                        (Note - Run this command in main terminal. Donot try to run in amy folder)
                    3. Run the script by 
                        Pyhton3 app.py 
                        (It will open a web terminal running on port 8707)
