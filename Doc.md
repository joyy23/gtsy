# Avereage Rating using weighed scoring & Content-based Filtering 
### Jiayi Yang
### Considering that there are 
- new users with no related information
- existed users with some avaliable information
### The code is divided into 2 parts:
- **`Non-personalized recommendation`**
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
 
 The `mean rating method` considers the mean rating of the all questions, which will makes it more universal relatively.
 
- **`Personalized recommendation`**
       In this case, it's actually very hard to use item-based or user-based. 
       
       The reason is still the size of dataset is way too small.
       
       There is very high chance that we can not find any similar user from other two users to one.
       
       20 questions are not so few but there are also a lot of categories, very few useful information can be collected if the questions are deviated.
    - `Content-Based Filtering` 
       
       This enables us to relate the user directly to the question and generate user_profile to see users' interest based on 20 questions' reaction.
     - `IDF`
         
         Actually there is not a big difference in the results of recommended questions between IDF and other two methods.
         But IDF takes the scarcity of some topics into account, and can ensure the data to be in the same scale.
