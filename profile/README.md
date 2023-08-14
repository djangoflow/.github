<p align="center"><img width=18.5% src="https://github.com/djangoflow/.github/assets/116165418/ddaa2265-af04-4915-8f02-bae1bce43291"></p>
<p align="center"><img width=60% src="https://github.com/djangoflow/.github/assets/116165418/1f3c1c13-a083-46b0-a6b9-38c84a255eef"></p>

<!-- badges -->
<p align="center">
  <!-- Contributions welcome --> 
  <img src='https://img.shields.io/badge/contributions-welcome-orange.svg'>
  <!-- slack -->
  <a href='https://join.slack.com/t/apexiverse/shared_invite/zt-1ols0scna-Pl~WaO2SA3SBTZyuL1vlvg'>
    <img src='https://img.shields.io/badge/Join-Slack-green'>
  </a>
  <!-- twitter -->
  <a href='https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2Fdjangoflow&text=Join%20us%20in%20revolutionizing%20software%20development%20with%20DjangoFlow&hashtags=Django%2CFlutter%2CDjangoFlow' target='_blank'>
    <img src='https://img.shields.io/twitter/url/http/shields.io.svg?style=social'/>
  </a>
 <!-- discord --> 
  <a href='https://discord.gg/2XBSENpEc2'>
     <img src='https://img.shields.io/discord/1093164096419024897?label=Discord&logo=Discord'>
 <!-- Linense --> 
  <a href='https://opensource.org/licenses/MIT'>
    <img src='https://img.shields.io/badge/license-MIT-blue.svg'>
</p>

# 🌟 Django + Flutter = Djangoflow

Djangoflow is an open source framework created by [Apexive](https://apexive.com "Top-notch software development for startups. In weeks, not months.")
that uses [Flutter](https://flutter.dev) for cross-platform apps and [Django](https://www.djangoproject.com "Django is a high-level Python web framework that encourages rapid development and clean, pragmatic design") for backend.

We also use [openapi-generator](https://openapi-generator.tech/docs/generators/dart/) to automate the api client generation and save time and avoid human errors following [DRY](https://apexive.com/post/zero-technical-debt) principles.

## 📖 History

Having built a lot of software for startups [Apexive](https://apexive.com "Top-notch software development for startups. In weeks, not months.") has accumulated extensive experience and created re-usable libraries ("building blocks") that now enable us to produce high quality code in weeks, not months.

Djangoflow is [Apexive](https://apexive.com "Top-notch software development for startups. In weeks, not months.") effort of open sourcing those libraries and sharing our experience with the open source community.

## 🐍 Django

| Modules                              | Status      | Description                                                                              | Contribute |
|------------------------------------|-------------|------------------------------------------------------------------------------------------|-----------------|
| django-df-chat                     | alpha       | Django-channels based chat backend                                                       | [![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/django-df-chat)](https://github.com/djangoflow/django-df-chat/issues)                |
| django-df-auth                     | production  | Ready to use user authentication with OTP, 2FA & Social integrations                     |[![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/django-df-auth)](https://github.com/djangoflow/django-df-auth/issues)                 |
| django-df-notifications            | production  | Rule based omni-channel notifications (push, email, text, slack, webhook etc)            |[![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/django-df-notifications)](https://github.com/djangoflow/django-df-notifications/issues)                 |
| django-df-portal                   | production  | Web-only admin portal                                                                    |[![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/django-df-portal)](https://github.com/djangoflow/django-df-portal/issues)                 |
| django-df-odoo                     | alpha       | Django Odoo integration                                                                  |[![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/django-df-odoo)](https://github.com/djangoflow/django-df-odoo/issues)                 |
| django-df-gpt                      | alpha       | Integration with GPTs such as chat-gpt                                                   |                 |
| django-df-scheduling               | alpha       | Event and availabilities scheduling                                                      |                 |
| django-df-configurations           | idea        | Remote (and not only) configuration management                                           |                 |
| django-df-model-events             | idea        | Management of model related events, such as food delivery plan or flights times          |                 |

## 🎯Flutter

### Djangoflow 

Contribute: [![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/flutter-djangoflow)](https://github.com/djangoflow/flutter-djangoflow/issues)

| Package | Description | Repository |
|------|-------------|------------|
| djangoflow_auth | Integrate various authentication providers, such as email OTP, magic link, Google, Facebook, Apple Sign-In, Discord, and more. This package provides a comprehensive and easy-to-use solution for managing user authentication. | [Link](https://pub.dev/packages/djangoflow_auth) |
| djangoflow_auth_google | Integrate Google Sign-In with ease using the `GoogleSocialLogin` class. This package allows you to effortlessly handle Google authentication for both web and mobile platforms, enhancing your app's login experience.| [Link](https://pub.dev/packages/djangoflow_auth_google) |
| djangoflow_auth_facebook | Effortlessly handle Facebook login with customizable permissions and login behavior. Use the `FacebookSocialLogin` class to integrate Facebook Sign-In into your app and provide users with the option to sign in using their Facebook accounts. | [Link](https://pub.dev/packages/djangoflow_auth_facebook) |
| djangoflow_auth_apple | Seamlessly integrate Apple authentication for both web and mobile platforms using the `AppleSocialLogin` class. Support customizable scopes, state, nonce, and more. Provide a secure and convenient way for users to sign in with their Apple IDs. | [Link](https://pub.dev/packages/djangoflow_auth_apple) |
| djangoflow_auth_discord | Use the `DiscordSocialLoginProvider` class to handle Discord login with ease. This package provides support for both web and mobile platforms, allowing users to authenticate using their Discord accounts. | [Link](https://pub.dev/packages/djangoflow_auth_discord) |
|  djangoflow_websocket | Easily manage connecting to a WebSocket server, subscribing to messages, handling reconnections etc all at once with djangoflow_websocket | [Link](https://pub.dev/packages/djangoflow_websocket) |
| djangoflow_app | A simple, opinionated, and minimal Flutter application structure for quick start and easy maintenance. | [Link](https://pub.dev/packages/djangoflow_app) |
| djangoflow_app_links | A Djangoflow package that implements deep-link handling via app_links package. | [Link](https://pub.dev/packages/djangoflow_app_links) |
| djangoflow_analytics | A library for tracking analytics with multiple Analytics providers in Flutter applications. | [Link](https://pub.dev/packages/djangoflow_analytics) |
| djangoflow_firebase_analytics | A library provides an easy and organized way to implement Firebase Analytics for your Flutter apps. | [Link](https://pub.dev/packages/djangoflow_firebase_analytics) |
| djangoflow_error_reporter | Djangoflow Error Reporter is a library that provides an easy and flexible way to handle errors in your flutter application. | [Link](https://pub.dev/packages/djangoflow_error_reporter) |
| djangoflow_sentry_reporter | A library that allows you to report errors to `Sentry` using the `djangoflow_error_reporter` pacakge. | [Link](https://pub.dev/packages/djangoflow_sentry_reporter) |
| djangoflow_fcm | A Djangoflow Flutter project to handle notifications using firebase_messaging | [Link](https://pub.dev/packages/djangoflow_fcm) |
| djangoflow_mixpanel_analytics | A library provides an easy and organized way to implement Mixpanel Analytics for your Flutter apps. | [Link](https://pub.dev/packages/djangoflow_mixpanel_analytics) |
| djangoflow_facebook_analytics | A library provides an easy and organized way to implement Facebook Analytics for your Flutter apps. | [Link](https://pub.dev/packages/djangoflow_facebook_analytics) |
| djangoflow_deep_link_interface | A Djangoflow Flutter package to provide abstraction for deep-link extraction. | [Link](https://pub.dev/packages/djangoflow_deep_link_interface) |


### Bloc, openapi & more 
Contribute: [![GitHub issues](https://img.shields.io/github/issues-raw/djangoflow/list_bloc)](https://github.com/djangoflow/list_bloc/issues)
    
| Package | Description | Repository |
|------|-------------|------------|
| openapi_repository | This package generates ListBloc and DataBloc using openapi_repository_annotations. | [Link](https://pub.dev/packages/openapi_repository) |
| flutter_list_bloc | A Flutter package to display the data loaded with list_bloc. | [Link](https://pub.dev/packages/flutter_list_bloc) |
| list_bloc | A BLoC library for loading data from an api end-point with filtering and pagination. | [Link](https://pub.dev/packages/list_bloc) |
| openapi_repository_annotations | Annotation to generate ListBloc and DataBloc. Should be used with openapi_repository package. | [Link](https://pub.dev/packages/openapi_repository_annotations) |
| progress_builder | A simple wrapper for asynchronous actions with progress/loading indicators and error handling. | [Link](https://pub.dev/packages/progress_builder) |

