<h1 align = center> Know Your Audience Better </h1>
<h3 align = center> Tailor strategies by unleasing the power of localized trends and sentiments </h3>
<h1> </h1>  
<h4>Can we help a politician tailor their speech for the next campaign visit to Minnesota? </h5>

Here, I present an approach to utilize the trending topics (searches made on Google, for example) for customizing and tailoring a campaign speech, such that it targets the right audience and creates the desired impact. 

<h3> <u>Steps </u> </h3>
    
**1. Hot Searches on Google Trends**    
  
For a geography on interest, extract the top trending topics through the searches made on Google. This can be fetched by using the Google Trends API (pyTrends) by using a search keyword of interest. The API allows to filter for the Geography as well as the time span you want to search for.

<img src = "/images/topic-pop.png" style="zoom:15%">  <img src = "/images/topic-senti.png" style="zoom:35%">

<h1> </h1> 
**2. Extract Local Sentiments on Popular political topics**  
   
Obtain tweets containing the keywords for these trending searches and extra voter sentiment. This makes use of the Twitter API connenction established using any local or cloud Python installation. A common way to extract tweets from Twitter is using the tweepy library. Here, this API gives access to select the location as well as the time span of tweets made. In the output, we can also extract the person's original location, tweet location, other post and profile attributes, like likes, comments and RTs for better understanding of the tweet's reach and performance. Finally, the user ID obtained from the tweet let's us understand whether the user is popular on Twitter and the popularity could be influential in getting the tweet's performance.
    
<img src = "/images/senti.png">    
    
<h1> </h1>     
**3. Dashboarding the collected tweets/sentiments**  
  
I then look at the extracted data to understand some patterns and hidden trends in the data. This can be achieved in two ways: Using the Data Studio present in the GCP suite, Using a tableau dashboard connected to the data for live refresh. Although I created the pipeline in the GCP environment, I make use of Tableau to visualize the results, simply because it allows to more variety in visuals and more comfort in designing viwes. The above screenshots represent both Tableau and Data Studio views.  

<h1> </h1> 
**4. Customization for Maximizing the Opportunity**  
  
Through the above analysis, any one can understand the voter's sentiments and views on specific topics and tune the speech as well as campaign to better suit a target geography.
  
  
<br>

<h3> Artchitecture at a Glance </h3>


<br>
The whole architecture is part of the GCP framework, starting from the combinaton of Google Trends and  Twitter APIs using Google Cloud's AI Notebooks (which serve as an interface for running Python notebooks). Google Cloud Storage is then used to store the final datasets with sentiments. These can be visualized using a Data Studio visual or can be linked to the Tableau desktop or server service using the API connection to Google account. The below image shows the same visually.  
  <br>
<img src = "/images/architecture.png">
<br>
  
<h2>How does it help other businesses?</h2>
  
  This analysis is transferable for all the businesses and use cases, where knowing your audience's (dynamic) preference and customers is crucial for extracting the best gains. Below are some of the use cases where this can be applied directly:   
   
<img src = "/images/usecase-retail.png" style="zoom:35%"> <h6 align = right>Retail chains can better plan and manage inventory of stores based on locally trending products and customers’ sentiments to minimize inventory loss.  </h6>
  
  <br><br><br>
<img src = "/images/usecase-music.png" style="zoom:35%"> <h6 align = right> Bands can narrow down on potential locations for concert that resonate with their genre of music to maximize footfall.  </h6>
  
  <br><br><br>
<img src = "/images/usecase-rest.png" style="zoom:35%"> <h6 align = right> Fast food restaurant chains can identify popular products at a localized level and customize menus for stores to match customer preferences and gauge user sentiments to further improve their offerings.  </h6>
  
<br>

##### Contributors:   

Aditya Agrawal   <agraw205@umn.edu>  
Anirudh Srikant  <srika028@umn.edu>  
Brady Engelke    <engel746@umn.edu>  
Karthik Ravishankar <ravis038@umn.edu>  
Sudhir Vinjamuri <vinja024@umn.edu>  
  
