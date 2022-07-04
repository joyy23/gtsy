# Avereage Rating using weighed scoring & Content-based Filtering 
### Jiayi Yang
### Considering that there are 
- new users with no related information
- existed users with some avaliable information
### The code is divided into 2 parts:
- Non-personalized recommendation
   - Editorial Content 
     
     This should work, but it's should be done by editors, not programmers
   - Top N
     
     This could work as well, the ranking can be based on the number of answers or the the click rate
   - Average Ratings
   
     This could work if we regard the person who give feedback to this question as the degree of interes in this question. 
     Since we have no information about new users at all, the formula should not require any related information. 
     Thus, Avereage Rating using weighed scoring is the best choice. 
     
   - Product Associations
   
     This could help to find out similar questions (under similar topics) but the problem is that we don't know what to recommend to users since we know nothing about new users
     
 The reason that why I chose Average ratings instead of Top N is the data is way too little. Apart from User4(new user), we only have 3 other users.
 There is no way to make a Top N ranking based on Feedback dataset for only three data, since there will be a high deviation value and it is not universal.
 The mean rating method    
- Personalized recommendation

### The dataset is with binary result 
