<!-- 

layout : post
title : Production usage
description : After write the markdown
category : ai
tags : series, fiction
comments : true 
author : Rich Dotcom
thumbnail_image_url: images/img_3.jpg
datetime_str: 23 August 2017
datetime : 2017-08-23
duration: 0:30:20
sound:
  type : simple_url
  value : https://pages.cs.wisc.edu/~cain/mp3/velveteens/bitter.mp3
  language: es        

-->


When running a live site you'll want to set the `PORT` env variable to `80` so you don't need to add `:3000` to the URL.
This requires root privileges and is not recommended.

Instead it is preferred to use a reverse proxy for security reasons.
Heroku and other services handle this aspect for you, but you can implement your own reverse proxy with Nginx or Apache.
**See [Related Projects](%base_url%/related-projects) for deployment scripts to use on your own servers**

## Listening Port
You can change the listening port anytime by setting the environment variable in your shell's profile, or running in-line as below:
`$ PORT=1234 npm start`

## Listening Host Address / IP

### Defaults
podcastjs listens only to localhost (`127.0.0.1`) traffic by default now (v0.17.0).  
This is to prevent unintended exposure and access of your documentation from older versions.  
Previous versions before v0.17.0 would bind to all IP addresses, which could accidentally make documents available on the public internet.  

### Override
To override the default IP host, please look above at an Nginx reverse proxy to access `127.0.0.1` or you can manually set the IP Host (private or public) setting the Environment Variable `HOST` somewhere.  
`$ HOST=192.168.0.10 npm start`
