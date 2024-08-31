# Git API Request Observations
This is pretty much a straight forward way to manage and review APis. You have to have some details to retrieve them and how to use them according to your project.

## Bearer Token
I notice that you have to be very careful with this process and where you store it as it can break or stop working if not set correctly before generating the token. The token is one time view from the GitHub website, however, you do receive an email about the token that has a button to retrieve it should you navigate away from the token page which will refresh losing access from the page. 

There is are specific places to use and store the token for use with all future request within the environment and also inside of the workspace (your choice). You have to click the authorization tab to add this token with pick Bearer Token from the drop down. 
## Token Setup and Use Screenshots
![Token Key1](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetup.github.postman_gjxivm.jpg)
![Token Key2](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetuprepositorypermissions.github.postman_z4jflo.jpg)
![Tokey Key3](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetuptokenexpiration.github.postman_oix8th.jpg)
![Token Key4](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetuprepositoryaccess.github.postman_mzgpbq.jpg)
![Token Key5](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetupauthorization.github.postman_ay21ny.jpg)
## Get Requests
This is a bit temperamental and you seriously must remember to set the variables with the user details in order to retrieve the list of personal repositories. This is done by utilizing your GitHub username and putting that into a variable as well as the baseURL so that you are not having to consistently enter it into the bar. You call it using the wave bracket {} to call it from the list of available variables (self and pre set). 
## Get Request Screenshot
![GetUserREPOS](https://res.cloudinary.com/dgls7u3iq/image/upload/v1725133344/getuserreposapi.github.postman_ydub9r.jpg)
## Post Request
You must truly know what it is that you want what you are creating to say as a name and description. Much like when sending the get request, variables can and was used in this process. 
## Post Request Screenshots
![PostREPO1](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724985261/createrepopt2.github.postman_w61m3h.jpg)
![PostREPO2](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724985261/createrepopt2repolistcreatedrepo.github.postman_qcffhd.jpg)
# Lets Get Started How To.....
The sections below elaborate on the steps taken by me to get each request.
## Setup the request environment (repetitive information)
I started with creating variables in the environment for the link, user, and bearer tokens as those pieces are information are required for GitHub for every request. That information is setup on the tab when an environment is created by adding them with names for each.
## The Get Request
You will need to use the variables set in a string as follows in order to get the necessary details being requested similar to this {{baseurl}}/user/repos and that string will provide you with a list of all repos owned and created on GitHub by you.
## The Post Request
Requires a little bit more to do besides what the get request requires in the string. The difference is what you put into the body of the request as raw data as follows (one of the two):
{
    "name": "Practice Repo",
    "description": "This is my git postman repo test",
    "private": true,
    "has_issues": false,
    "has_projects": false, 
    "has_wiki": false
}
{
    "name": "Practice Repo",
    "description": "This is my git postman repo test",
   "homepage": "https://github.com", 
   "private": false,  
   "is_template": true
}

