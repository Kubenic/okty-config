
<h1 align="center">
  <a href="https://okty.io/">
    <img src="https://i.imgur.com/kN8SThu.png" alt="Okty" height="200">
  </a>
  <br>
  Okty - Configuration
  <br>
</h1>

<h4 align="center">The simplest application to create your docker projects.</h4>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Build Status](https://travis-ci.org/lbassin/okty.svg?branch=master)](https://travis-ci.org/lbassin/okty) 
![Dependencies](https://david-dm.org/lbassin/okty.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-lightgrey.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

<p align="center">
  <a href="#what-is-okty">What is Okty ?</a> •
  <a href="#configuration">Configuration</a> •
  <a href="#contribute">Contribute</a> •
  <a href="#license">License</a> •
  <a href="#credits">Credits</a>
</p>

## What is Okty ?

Okty is a simple tool to generate customized docker-compose files.  
This is the configuration repository, you may find more information about this project on the [main repository](https://github.com/lbassin/okty)

## Configuration

Each available container has it own yml configuration file in the "containers" folder  
  
Configuration has simples mandatories fields : 
```yml
name: "The displayed label"
image: "Logo of the container (It has to come from an https source)"
docker: "The name of the image to pull from the docker hub"
version: "The version of of the specified image"
config: []
```

Config entry is a little bit more complicated and will contains all the options to customize your container  

#### Config

In this array, each entry will be considered as a form group.  
In order to make easier setup form for the end user, we recommend to split your configuration by thematics groups.  
  
You need to specify an unique ID for each group and an associated label
```yml
config:
  - 
    id: "Unique_ID"
    label: "Group Label"
    fields: []
```  

### Fields 

// TODO

## Contribute

Okty needs help to stay up to date and improve his features.  
If something is missing or broken, feel free to open an issue or made a pull request.  
  
Maybe the container you want isn't available ? 
Make your own or ask for it on through pull requests or issues !

## License
Okty is made available under the [MIT License](http://www.opensource.org/licenses/mit-license.php).

## Credits
Okty is created and maintained by
[Samuel Alves Antunes](https://github.com/NeverTwice), 
[Laurent Bassin](https://github.com/lbassin),
[Maxime Marquet](https://github.com/x-Raz) &
[Jordan Venant](https://github.com/Kubenic).

*We're open to suggestions, feel free to message us or open an issue.*  
*Pull requests are also welcome!*
