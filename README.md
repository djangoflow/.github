# Django + Flutter = Djangoflow


## What is Djangoflow?

[Djangoflow](https://apexive.com) is an open-source framework developed by [Apexive](https://apexive.com), which harnesses the capabilities of [Flutter](https://flutter.dev) and [Django](https://djangoproject.com) to expedite the process of cross-platform application development.

This framework, acting as a crucial component in [Apexive](https://apexive.com) rapid app development, facilitates the construction of production-ready cross-platform applications in a significantly reduced timeframe (sometimes days or weeks instead of months).

Designed with modularity in mind, Djangoflow provides an ecosystem of general-purpose configurable backend and frontend modules, promoting efficient application construction without redundant efforts, thereby adhering to the "Don't Repeat Yourself" (DRY) principle.

The core objective of Djangoflow is to optimize productivity by maintaining a structured codebase, emphasizing a clean architecture, and strictly adhering to DRY principles.

As projects progress to scalability phases, segments with high-performance demands can be replaced with micro-services, employing technologies such as Golang for optimal results.

Djangoflow predominantly employs [Django](https://www.djangoproject.com) as its backend technology, in conjunction with the [django-rest-framework](https://www.django-rest-framework.org/) to devise backend business logic and APIs.

In order to optimize the development process, a systematic code generation procedure is employed to produce the API client and associated documentation, utilizing tools such as [drf-spectacular](https://github.com/tfranzel/drf-spectacular) and [openapi-generator](https://openapi-generator.tech/docs/generators/dart/).

Subsequently, this automatically generated API client is integrated with Djangoflow's Flutter modules, minimizing functional redundancy within the Flutter project. This methodology substantially reduces the time required for coding and debugging APIs and minimizes the potential for human error, adhering to [DRY](https://apexive.com/post/zero-technical-debt) principles.

In summary, Djangoflow represents an integrated ecosystem comprised of Django, Flutter, and Terraform modules. It offers a systematic blueprint detailing the interrelation and functionality of its components.

## Django modules 

A DjangoFLow django module main function is to provide some functionality to the counterpart frontend (flutter) module via REST API (drf).

These modules are therefore very much like regular django packages or apps with a few additions to make the above job easier. You can use djangoflow modules
in your django project without using the djangoflow framework conventions. However, the real magic happens when they are clicked together into a project with minimal configuration.

So what are these small differences between a djangoflow and a django module?

1. DFMeta class in the AppConfig

By configuring the module AppConfig via DFAppConfig you will have an extra app configuration in your django AppConfig, and that extra configuration will
live in the DFMeta class.

It is used for different djangoflow modules to discover each other and automatically configure themselves.

For example, adding https://github.com/djangoflow/django-df-api-drf module to your project will automatically setup the openapi backend for your flutter app.

This module will inspect all other installed apps to see if they provide a djangoflow api settings in their DFMeta class and if so will configure those endpoints without any manual configuration.

2. Django settings shortcuts and defaults

A djangoflow module would have a `df/defaults.py` that can be used for pre-configuring your django project third-party modules in accordance to this djangoflow module needs.

For example, df_auth/defaults.py would give you a number of useful defaults that you can use in your `settings.py` like so:

```
from df_auth.df.defaults import DF_AUTH_APPS, SIMPLEJWT

..
INSTALLED_APPS = [
...
*DF_AUTH_APPS,
...
]

```

This will give you a nice pre-configured set of defaults and the required apps to use the `df_auth` module.

This results in minimal project configuration and glue while re-using the pre-built functionality for things like authentication, notifications, chat, integrations and so on;
and allows bootstrapping a production-ready backend in hours.

What is the left is creating project specific django modules following the same pattern.

Djangoflow modules use `DF_` prefix for configuration.

The best way to discover the ecosystem is by trying out https://github.com/djangoflow/djangoflow-examples

## Flutter modules

Most of the backend djangoflow modules will have one or more flutter counterparts.

TODO(saiful): describe how flutter modules are setup 

## FAQ

1. Why you do not use Go for backend? - Djangoflow is about productivity, not performance which is needed at later stages of a project
2. Why do you use somewhat un-modern REST API. - This allows automatic client generation and keeping business logic on server side.

## History

Having built a lot of software for startups [Apexive](https://apexive.com "Top-notch software development for startups. In weeks, not months.") has accumulated extensive experience and created re-usable libraries ("building blocks") that now enable us to produce high quality code in weeks, not months.

Djangoflow is [Apexive](https://apexive.com "Top-notch software development for startups. In weeks, not months.") effort of open sourcing those libraries and sharing our experience with the open source community.
