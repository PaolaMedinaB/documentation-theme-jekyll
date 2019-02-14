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

La base de datos de Oracle está disponible en cinco ediciones, cada una adecuada para diferentes escenarios de desarrollo e implementación. Éstas son:

*  <b> Oracle Database Standard Edition One </b>for small business and highly distributed branch environments.

* <b> Oracle Database Standard Edition </b> for larger machines and clustering of services with Oracle Real Application Clusters (Oracle RAC). 

* <b> Oracle Database Enterprise Edition </b> for  high-volume online transaction processing (OLTP) applications, query-intensive data warehouses, and demanding Internet applications. 

* <b> Oracle Database Express Edition (Oracle Database XE) </b> is an entry-level edition of Oracle Database that is free.

* <b> Oracle Database Personal Edition </b> supports single-user development and deployment environments that require full compatibility with Oracle Database Standard Edition One, Oracle Database Standard Edition, and Oracle Database Enterprise Edition.


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

