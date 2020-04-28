# GA-access-token-using-sign-in

Setting up authentication.

1. Go to the APIs & Services page in the GCP Console using below link.
https://cloud.google.com/console/google/maps-apis/overview

2. Click the project drop-down and select or create the project for which you want to add an API key.
3. Click the menu button  and select **APIs & Services > Credentials**.
4. On the Credentials page, click Create **credentials > OAuth client ID**.
5. Then it will show many options for selection. Select **Other** options. Then provide **name** and click on create button.Then you OAuth client ID generated.
6. Then Click on the **name** which you provided for OAuth client ID under OAuth 2.0 Client IDs
7. After clicking on name, you we are seeing multiple options like **DOWNLOAD JSON**, **Reset Secret** and **Delete**.
   
   Click on **DOWNLOAD JSON** button. It will download that json key file then rename that file to **oauth_file.json**

# Generating access token

1. Open terminal to install requirements. Install requirements using below command:
    
    **pip3 install -r requirements.txt**
    
2. Run python file

    **python3 ga_connection.py**
    
3. After running python file, it will generate **authentication link** for granting GA access with scopes. Open that link complete flow as per process.
4. After completing of authentication, it will generate **ga_credentials.dat** file which contain token.


**Notes**: I have added ga_credentials.dat and oauth_file.json for sample reference.