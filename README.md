Welcome to Serendipity
======================

Serendipity is a Python 3 Web Application Framework, including everything you need to quickly build and deploy a Web Application using a well-known Python ORM (SQLAlchemy + SQLasagna Extensions) with support to many relational databases and advanced features like automatic Scaffolding generation, Routing and etc...

By default, Serendipity comes with a simple login and permissions / ACL system. Also it comes with a i18n, very simple translation system integrated with the template engine to generate per-language caches.

In order for Serendipity to work, you must have some Python packages in specific versions (or superior versions). You can check those requirements later in this document in the section **System Requirements**.

We recommend the use of virtualenv and virtualenvwrapper. You can setup your environment quickly using the amazing [virtualenv-burrito](https://github.com/brainsik/virtualenv-burrito). More about the setup in the docs.


Features
========

With Serendipity you can use pure Python 3 and a very nifty templating language to design you entire web application, and even your backend for a web-services in order to support native clients and native mobile apps. We always recommend that you use HTML5, CSS3 and Javascript in your projects but that's entirely up to you.

- Unified Python decorator ( @sdpy ) for exposing methods to the web, process security, override templates and layouts, format a JSON response automatically from a dictionary return, routing aliases and more.
- Completely flexible, you can add new features globally or locally in your controllers.
- MVC approach with RAD / DRY and Convention over Configuration **ALWAYS** on mind. (as learned by the beautiful Zen of Rails)
- A helper script/app called sdpy which allows you to create a new Serendipity app, new controllers, models, views, start and stop the server, check the environment, run tests, update the framework version to the latest stable in this Git official repository and much more.
- Easy to update helper script which not only updates itself but can also update current deployments of the framework core files.
- i18n Translation subsystem with supporting native Python dictionaries for translation.
- Single import on all controllers. We centralize the importing of libraries on the kit.py file which will take all the required libs up to the main memory and serve them to all controllers as needed, keeping the code smaller and memory management centralized and clean.
- There's much more to be written here and to come in the near future... stay tunned on the README file and in the official wiki.

Documentation
=============

For now, the documentation will be published in this project **Github wiki**. This can be changed in the future but it is the way for now.

Requirements
============

Serendipity Framework was built using some Python 3 Libraries for several purposes.
The required ones are listed above, but you can add your own at any time. We recommend that you include this libraries once on the c/kit.py file, so it will be available framework-wide.

- Python 3 (3.2 or higher is highly recommended)
- Tenjin 1.0.1 or higher.
- setproctitle 1.1.2 (If you want a nice process name)
- SQLAlchemy 0.7.2 or higher.
- For MySQL Databases, we are using MyconnPy MySQL Connector under version 0.3.2 or higher.
- For PostgreSQL Databases, we are using the py-postgresql connector.
- For other databases, study the latest version of a connector compatible with Python 3 and SQLAlchemy on SQLAlchemy Website.

Remember to install all those libs for Python 3 as your system probably may have an older 2.x version of Python installed as default.
Generally you do that by running the following inside the library source directory:

        # sudo python3.2 setup.py install

And confirm it is installing by opening python3 and importing the library.
Soon a full environment setup tutorial will be available under the documentation wiki.
Also it is planned for the ./sdpy helper to check the dependencies and their version for you and spawns warning messages if something is wrong with your environment.

We highly recommend that you run Serendipity Framework under Linux, BSD, UNIX or Mac OS X, specially for production environments. This doesn't means however you can't run on Windows environments. It's just not supported now and you might have to change some things manually.


AUTHORS
=======

The Serendipity Framework was developed by **ezVoice Telecom** in Ribeirão Preto - Brazil for use in its own line of appliances and Cloud services. Further the executive council has decided to open the source of the framework to the community in a effort of disseminating the technology and support the development of web-applications in Python 3.

The main engineers involved in the process are:

- Danilo Martins                    < mawkee@gmail.com >
- Evandro Arruda                    < ecarruda@gmail.com >
- Ygor Abreu Lemos                  < ygbr@mac.com >
- Murilo da Silva                   < murilobr@gmail.com >

License and Copyright
=====================

The Copyright of the Framework is property of [ezVoice Telecom - Brazil](http://www.ezvoice.com.br)

Serendipity Framework is licensed under the **GNU LESSER GENERAL PUBLIC LICENSE (LGPL)**.

