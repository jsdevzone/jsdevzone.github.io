---
layout: post
title: Packaging Sencha ExtJs Application With Github Electron
comments: true
description: ""
modified: 2015-08-15
tags: [javascript, extjs, nodejs, sencha]
disqus_shortname: "jasimea"
disqus_identifier: "0608201501"
image: "http://4.bp.blogspot.com/-BC7wPNB_8M8/VDbznTaHMyI/AAAAAAAACKU/3mFwF1nCU2c/s770/Untitled-6-800x500.jpg"
---

Github's electron framework lets you write cross-platform desktop application using JavaScript, HTML and CSS. It is based on chromium and io.js. In this blog post we will check how we can package our sencha extjs application into desktop application using electron framework. We will also check how we can automate the packaging by integrating the process into the sencha command.

#### Sencha Desktop Packager
Sencha was providing built in way to package the application into desktop application using desktop packager. Unforutnately they discontinued the project.  Short paragraph about sencha desktop packager.

#### Setting up sencha extjs application.
Sencha provides a cross platform command line application which provides many automated tasks around the full life cycle of your applications from generating a new project to deploying an application to production. Generating a starter extjs application is as simple as follows with sencha command:

-Download and install sencha Cmd.
- Open your terminal and issue the following command

``` 
sencha -sdk	/path/to/extjs/framework generate app AppName /path/to/workspace
cd /path/to/workspace
sencha app watch
```

###Building For Electron.

