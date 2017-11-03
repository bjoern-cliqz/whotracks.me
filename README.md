

<img 
alt="whotracks.me"
style="width: 200px"
src="https://raw.githubusercontent.com/cliqz-oss/whotracks.me/master/static/img/who-tracksme-logo.png">

Bringing Transparency to online tracking - built by Cliqz and Ghostery

___
This repository contains:

* data on trackers and websites as shown on [whotracks.me](https://whotracks.me) (`./data`)  
* database mapping tracker domains to companies (`./db`)  
* code to render the [whotracks.me](https://whotracks.me) site


## 1. Building the site
We use python 3.6 for rendering the site.

```bash
$ virtualenv -p <path to python 3> <name>
```

### 1.1 Install Dependencies 
```bash
$ source <name>/bin/activate
$ pip install -r requirements.txt

```
Furthermore you also need to install sass: 
[http://sass-lang.com/install](http://sass-lang.com/install)


### 1.2 Build and Serve Site locally

To build all the site, please run: 
```bash
$ python build.py site
```

Run `python build.py -h` to see how you can build only certain 
parts you may have changed (e.g. blog, tracker pages etc). 
A `_site/` directory will be created with the content of the site.

To serve the site locally, run:

```bash
$ python serve.py
```  
The site should be accessible `localhost:8000`


## 2. Contributing
We are happy to take contributions on:
* guest articles for our blog in the topics of tracking, privacy and security. Feel free to use the data in this repository if you need inspiration.
* Curating our database of tracker profiles.


## 3. License
The content of this project itself is licensed under the [Creative Commons Attribution 4.0 license](https://creativecommons.org/licenses/by/4.0/), and the underlying 
source code used to generate and display that content is licensed under the [MIT license](https://github.com/cliqz-oss/whotracks.me/blob/master/LICENSE.md).
