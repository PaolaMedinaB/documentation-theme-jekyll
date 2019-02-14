---
title: Manual de instalación
tags: [getting_started, troubleshooting]
keywords:
Resumen: "Esta sección describe cómo descargar e instalar Oracle Application Express. La forma de instalar Oracle Application Express depende del tipo de base de datos en la que se esté instalando."
sidebar: mydoc_sidebar
permalink: mydoc_install_jekyll_on_mac.html
folder: mydoc
---


## Arquitectura de APEX 
La arquitectura de APEX es bastante simple. Tienes que tener un navegador que se comunique a través de una aplicación Java de nivel medio (mid-tier) que en nuestro caso es el *Oracle REST Data Service (ORDS)* y que puede ser instalada en Oracle Web Logic Server usando Jetty o Tomcat. Luego esas peticiones se envían a través de la base de datos y todo el procesamiento se realiza en la base de datos Oracle, donde se encuentra el motor apex, y luego envía la petición de vuelta a través del ORDS y de vuelta al navegador.

{% include image.html file="pic3.png" alt="Jekyll" caption="Arquitectura de APEX" %}



## 1. Base de datos Oracle 

Ruby and [RubyGems](https://rubygems.org/pages/download) are usually installed by default on Macs. Open your Terminal and type `which ruby` and  `which gem` to confirm that you have Ruby and Rubygems. You should get a response indicating the location of Ruby and Rubygems.

If you get responses that look like this:

```
/usr/local/bin/ruby
```

and

```
/usr/local/bin/gem
```

Great! Skip down to the [Bundler](#bundler) section.

However, if your location is something like `/Users/MacBookPro/.rvm/rubies/ruby-2.2.1/bin/gem`, which points to your system location of Rubygems, you will likely run into permissions errors when trying to get a gem. A sample permissions error (triggered when you try to install the jekyll gem such as `gem install jekyll`) might look like this for Rubygems:

```
 >ERROR:  While executing gem ... (Gem::FilePermissionError)
  You don't have write permissions for the /Library/Ruby/Gems/2.0.0 directory.
```  

Instead of changing the write permissions on your operating system's version of Ruby and Rubygems (which could pose security issues), you can install another instance of Ruby (one that is writable) to get around this.

## 2. Oracle REST Data Services

Homebrew is a package manager for the Mac, and you can use it to install an alternative instance of Ruby code. To install Homebrew, run this command:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

If you already had Homebrew installed on your computer, be sure to update it:

```
brew update
```

## 3. Navegador web

Now use Homebrew to install Ruby:

```
brew install ruby
```

Log out of terminal, and then then log back in.

When you type `which ruby` and `which gem`, you should get responses like this:

```
/usr/local/bin/ruby
```

And this:

```
/usr/local/bin/gem
```

Now Ruby and Rubygems are installed under your username, so these directories are writeable.

Note that if you don't see these paths, try restarting your computer or try installing rbenv, which is a Ruby version management tool. If you still have issues getting a writeable version of Ruby, you need to resolve them before installing Bundler.

<h2 id="bundler">Install the Jekyll gem</h2>

At this point you should have a writeable version of Ruby and Rubygem on your machine.

Now use `gem` to install Jekyll:

```
gem install jekyll
```

You can now use Jekyll to create new Jekyll sites following the quick-start instructions on [Jekyllrb.com](http://jekyllrb.com).




{% include links.html %}

