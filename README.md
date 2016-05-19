# Database_Output
#This file defines some SQL querie that can be performed on the database
#Table Manipulation
    CREATE TABLE "Author"
    (Author_ID VarChar,
    Author_Name VarChar,
    Author_Password VarChar,
    Username VarChar);
    
#Data Manipulation
#insert a comment to the comment table 
  INSERT INTO Comment
  VALUES(NULL, 'Saddam', 'sadam@test.com', 'thus the comment', 001);
#deletes a post form the post table
  DELETE FROM Post
  WHERE Post_ID = 003;
  
#Select Statements
#Displays all post with specific conditions
  SELECT Post_Title,Post_Body FROM Post
  WHERE Status = 'published'
      AND Tags_id = 'politics';
#Displays all comment
  SELECT *
  FROM Comment;
  
      
