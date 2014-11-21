YoDA
====

The Yo Done Agent. 

Run any command by prepending 'yo' to it and receive a yo whenever the command is done. 

Here is how you can get it:

1. Add the following script in ~/bin
https://github.com/ChrisJamesC/yoda/blob/master/yo
2. Make it executable   

        chmod+x ~/bin/yo

3. Install the yo app on your phone and create an account. 
4. Get/create an API account on http://dev.justyo.co/ (say the created username is EXAMPLE)
5. Send a yo to the API account yo created: EXAMPLE (to register)
6. Add your username and the API token to your .bashrc:

        export YO_USER=*** (should be your yo username here)
        export YO_TOKEN=*** (key corresponding to the yo API account)

7. reload your bashrc:

      source ~/.bashrc

8. In a new shell session, run any command prepending `yo` to it:

      yo sleep 10

__Examples:__

```
yo make check 
yo TRACE=UpdateServer make check TESTS=...
ENV_VAR=1 cd /src/example; yo ENV_VAR=2 make
...
```
