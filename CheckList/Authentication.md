## Authentication

- Registration
    - Input validation
        - [ ]  Space manipulation & Using Dots & Case sensivity check
        - [ ]  Checking allowed characters (`<> " '`)
        - [ ]  Register using `myemail%00@email.com` or (%0d, %0a)
        - [ ]  Register using `myemail@target.com`
            - Response manipulate from `401 Unauthorized` to `200 Ok` or `302 Found`
    - Analysis
        - [ ]  Check `.js` file on the page, such as `login.js`
        - [ ]  Check the parameters used on the endpoint
            - Might be listed in the `source` or `js`
        - [ ]  Checking the Mobile Endpoint
            - Does it have the same protection as webapp?
            - How does it treat Unicode characters?
        - [ ]  Google Dorks
            - `site:example.com inurl:register inurl:&`
            - `site:example.com inurl:signup inurl:&`
            - `site:example.com inurl:join inurl:&`
    - Misc
        - [ ]  Email Takeover
            - Register an Email, before confirming, change the email. check if the new confirmation email is sent to the first registered email.



### <a name="Authentication">Authentication</a>
- [ ] Test for user enumeration  
- [ ] Test for authentication bypass  
- [ ] Test for bruteforce protection  
- [ ] Test password quality rules  
- [ ] Test remember me functionality  
- [ ] Test for autocomplete on password forms/input  
- [ ] Test password reset and/or recovery  
- [ ] Test password change process  
- [ ] Test CAPTCHA  
- [ ] Test multi factor authentication  
- [ ] Test for logout functionality presence  
- [ ] Test for cache management on HTTP (eg Pragma, Expires, Max-age)  
- [ ] Test for default logins  
- [ ] Test for user-accessible authentication history  
- [ ] Test for out-of channel notification of account lockouts and successful password changes  
- [ ] Test for consistent authentication across applications with shared authentication schema / SSO  


### <a name="Authorization">Authorization</a>
- [ ] Test for path traversal  
- [ ] Test for bypassing authorization schema  
- [ ] Test for vertical Access control problems (a.k.a. Privilege Escalation)  
- [ ] Test for horizontal Access control problems (between two users at the same privilege level)  
- [ ] Test for missing authorization
