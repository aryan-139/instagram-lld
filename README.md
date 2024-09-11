# instagram-lld
This is a repository containing the low level design for instagram. 

## key features of instagram

### Authentication and Authorization Service
- signup of a new user
- creation of usernames 
- login using username-password/ previous logged in the device/ single sign-on using mail or socials 

### Content Feed Generation
- Showing the most relevant posts/ reels above 
- Filtering of the feed based on different selections (General Feed, Close Friends Only, Image Only, Reel Only)
- How long should the feed be? 
- What happens when someone hits refresh?

### Feed Content Interactions
- Likes, Comments, Shares, Bookmark
- How does the comments viewing happen? Do you hit the RDB or just keep it cached somehow. 
- Managing comments when there is high influx of comments? 
- If someone makes a new comment and you are reading the comments, does it dynamically show that there is a new comment? 
- How does like get stored, does every like is made to be read in a DB one by one? 
- Shares and Bookmarks data saving

### Story Generation And Prioritization Consumption Only
- Which stories to rank higher? 
- How many stories to load at a time? 
- What happens when I click on a story? 

### Search and Discovery 
- Search Page content prioritization
- Recent searches made, how many to show? 
- Trending Searches
- What to search recommendations? 
- When a search param is made, what can the search be, username, song, post, hashtags
- How to rank the search results? (Hashtags, Likeability, other parameters)
- How to make that search happen? How can it be optimised? Hitting a table/ data warehouse? How does it function? 
- Storing of recent searches data 

### Content Creation (Post, Story, Reel, Live)

- Story Creation
- Post Creation 
- Reel Creation 
- Live 
- How does media get stored, and how does it get stored, as per the colour template if text?
- How does media modifications work? 
- What is used for live? 
- What interactions are stored when someone goes live? 
- How to store the live? Do you prioritize the quality of storage for live? 
- How to stream data well? 
- Reel Modifications, how does that work? 
- What are the KPIs that are tracked per media item that qualifies as a post? 
- How does tagging in post work? 
- Adding location

### Reel Consumption Service 
- Algorithm to rank the reels higher 
- What are the KPI's tracked 
- How is the Reel labeled? 

### Suggested For You 
- Closest Follower Recommendation Engine to find the closest friends 

### Messaging Service 
- How are messages saved? 
- How do you spam/ protect nudity from the incoming messages? 
- Categorizing messages as normal messages and message requests
- Recent Chats
- Searching through a bunch of messages 

