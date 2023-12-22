[[HTML]]
# Fix mailto not working in HTML
#resource 

1. Go to Settings, Apps, Default Apps, and under Email, select Google Chrome.
    - This step alone, does not necessarily work, I had to set the _handler_, as shown in the following steps, because Gmail was blocked.
    - [![enter image description here](https://i.stack.imgur.com/uDhpJ.png)](https://i.stack.imgur.com/uDhpJ.png)
2. In Chrome, go to Settings by selecting [![enter image description here](https://i.stack.imgur.com/5k926.png)](https://i.stack.imgur.com/5k926.png)
3. Select Privacy and security on the left side of the screen
4. Select Site Settings
5. Scroll down to Permissions and select Additional permissions
6. Select Handlers
7. Select Allow sites to ask to become default handlers for protocols
    - If a site (e.g. Gmail) is blocked, remove the block
8. Open Gmail in a new tab and sign in
    - In the address bar, select the [![enter image description here](https://i.stack.imgur.com/gqcLR.png)](https://i.stack.imgur.com/gqcLR.png)
        - [![enter image description here](https://i.stack.imgur.com/6K0sb.png)](https://i.stack.imgur.com/6K0sb.png)
        - _This page wants to install a service handler._
    - Select Allow, and then Done
9. Return to the Settings tab, and `mail.google.com` will be the email handler.
    - [![enter image description here](https://i.stack.imgur.com/A4gqX.png)](https://i.stack.imgur.com/A4gqX.png)

[Reference](https://stackoverflow.com/a/66319770)
