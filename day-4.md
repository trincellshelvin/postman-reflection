# Git API Request Observations

## Bearer Token
I notice that you have to be very careful with this process and where you store it as it can break or stop working if not set correctly before generating the token. The token is one time view from the GitHub website, however, you do receive an email about the token that has a button to retrieve it should you navigate away from the token page which will refresh losing access from the page. 

There is are specific places to use and store the token for use with all future request within the environment. You have to click the authorization tab to add this token with pick Bearer Token from the drop down. 

## Get Requests
This is a bit temperamental and you seriously must remember to set the variables with the user details in order to retrieve the list of personal repositories. This is done by utilizing your GitHub username and putting that into a variable as well as the baseURL so that you are not having to consistently enter it into the bar. You call it using the wave bracket {} to call it from the list of available variables (self and pre set).

![Token Key1](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetup.github.postman_gjxivm.jpg)
![Token Key2](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetuprepositorypermissions.github.postman_z4jflo.jpg)
![Tokey Key3](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetuptokenexpiration.github.postman_oix8th.jpg)
![Token Key4](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetuprepositoryaccess.github.postman_mzgpbq.jpg)
![Token Key5](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokensetupauthorization.github.postman_ay21ny.jpg)
![GetREPO](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724974207/usertokengetrequest.github.postman_nqiktm.jpg)
![PostREPO1](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724985261/createrepopt2.github.postman_w61m3h.jpg)
![PostREPO2](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724985261/createrepopt2repolistcreatedrepo.github.postman_qcffhd.jpg)
![GetUserREPOS](https://res.cloudinary.com/dgls7u3iq/image/upload/v1725133344/getuserreposapi.github.postman_ydub9r.jpg)
