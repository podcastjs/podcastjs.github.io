# Foo Bar Baz Podcast

<p align="center">
  <img src="https://github.com/podcastjs/podcastjs-demo/assets/3322836/bf561775-d960-4763-b0a8-1c3fb8f58d9c" width=150>  
</p>

## Requirements

- Nodejs
- Markdown files
- Mp3 or wav public urls

## Demo

Install the tool

```
npm install -g github:/podcastjs/podcastjs
```

Start as developer

```
podcastjs --start
```

You should see something like this

![](https://github.com/podcastjs/podcastjs-demo/assets/3322836/d8cc4077-c908-478b-bccd-327342a12698)

## Publish

By default, it creates a **site** folder

```
podcastjs --publish
```

If you need a custom folder:

```
podcastjs --publish --output docs
```

This folder will contain your static web site. 
  - You can push host this folder whatever you want.
  - Or you can push to the github to serve it as github site

![image](https://github.com/podcastjs/podcastjs-demo/assets/3322836/c7255e58-4ce8-4df7-b25f-8e41b0d687e6)


## How it works

More details here

https://github.com/podcastjs/podcastjs
