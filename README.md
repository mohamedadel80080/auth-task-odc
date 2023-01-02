# ODC-users-project

# API Endpoints
 
## Register endpoint 
  # use this endpoint can register user 
POST  https://djangoodc.pythonanywhere.com/api/register 
   
  required parameters : 
   username,
   password ,
   email  ,

# list user endpoint
  ## can retrive all users 
GET  https://djangoodc.pythonanywhere.com/api/user


# update specfic user 
  ## can update user fields (username,password,email)
PUT https://djangoodc.pythonanywhere.com/api/user/:id

   optional parameters : 
      username ,
      password ,
      email  

# Delete specfic user 
  ## can delete specfic user   
DELETE   https://djangoodc.pythonanywhere.com/api/user/:id

#  login endpoints

POST  https://djangoodc.pythonanywhere.com/api/token/

  required parameters : 
   username,
   password ,

  return refresh , access   token

POST  https://djangoodc.pythonanywhere.com/api/token/refresh/

  required parameters : 
   refresh token

POST  https://djangoodc.pythonanywhere.com/api/token/verify/

  required parameters : 
    token ->(access)
    
