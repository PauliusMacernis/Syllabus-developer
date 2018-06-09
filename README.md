# The Comprehensive Syllabus for Developers

Lets make the comprehensive list of subjects describing what **the developer** must understand nowadays.  
The list is suited for a person who wants to go for any of the following:
- to self-study in order to become **the developer** ([software developer](https://en.wikipedia.org/wiki/Software_developer), [web developer](https://en.wikipedia.org/wiki/Web_developer))
- to self-study in order to pay **the developer**'s [technical debt](https://en.wikipedia.org/wiki/Technical_debt) off
- to teach the course for **the developers** of level junior, mid, and even senior

## General structure

It is quite clear that topics will differ for specific types of syllabus: "Java developer", "PHP developer", "Clojure developer", "Front-end developer", "Back-end developer", "Full stack developer", whatever we put in front of the "developer" makes the final syllabus look differently.  
However, the general stack exists. No matter which high-end (technology stack) the person is choosing, he/she will have to understand things like: encoding (e.g. Unicode, UTF-8, etc.), regural expressions, security (private-public keys, social engineering, etc.), etc.  

## How do I see the compose working? (just some thoughts on the topic)

I personally think that a tool like [Composer](https://getcomposer.org/) may be the tool for managing such syllabus dependencies. It sounds quite weird and funny at the same time but Composer is the dependency manager and may do such thing amaizingly well. The only issue I see is composing the "merged version" of the syllabus.

- Different repositories would exist per topic, for example: PHP - one repository, Symfony - another one, Laravel - one more, Git, Bash, UML, etc.
- Each repository would contain the configuration file like `composer.json` in where all the dependencies are placed. Something similar, I would say:
```
{
    "name": "syllabus/lemp",
    "require": {
        "syllabus/linux": "*",
        "syllabus/nginx": "*",
        "syllabus/mysql": "*",
        "syllabus/php": "*"
    }
}
```
- Then we would simply do `composer install` and it would compose the complete syllabus of the chosen {something} developer.


## How it is actually working now?

At the moment I am working on creating the sylabulus for **PHP web developer** as this is my direct interest of today. Text-only so far... Will see what may be done better later :)
