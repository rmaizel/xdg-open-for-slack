# xdg-open-for-slack
Quick fix for authenticating to Slack on OpenSUSE linux

## Background
After installing Slack Desktop on openSUSE Tumbleweed, I found I couldn't authenticate. Something about the app and KDE was broken, and wouldn't let me log in. So, like any good techie I searched online for an answer, and landed on StackOverflow. Lots of suggestions, but the only answer I found that worked referenced the code in this repo. 

**I TAKE NO CREDIT FOR THIS CODE**

I have to thank [ϹοδεMεδιϲ](https://stackoverflow.com/users/83005/%cf%b9%ce%bf%ce%b4%ce%b5m%ce%b5%ce%b4%ce%b9%cf%b2) for their answer - not even the top one! - to the question in this thread: [Signing into slack-desktop not working on 4.23.0 64-bit (Ubuntu)](https://stackoverflow.com/questions/70867064/signing-into-slack-desktop-not-working-on-4-23-0-64-bit-ubuntu). The answer permalink is here: https://stackoverflow.com/a/71579300 

## Instructions
1. Download the latest Slack for Linux client here: https://slack.com/downloads/linux; Install it, *BUT DO NOT RUN IT YET*
1. Download the file `xdg-open` from this repo, or copy the content and create your own. 
1. From a terminal, in the folder where you downloaded `xdg-open` Run the following commands:
    ```
    sudo cp xdg-open /usr/local/bin   
    sudo chmod +x /usr/local/bin/xdg-open
    ```
4. Now, launch Slack, and log in normally.
