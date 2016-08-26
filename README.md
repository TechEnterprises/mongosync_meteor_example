# Mongosync + Distill + Meteor (example)
This module demonstrates the capability of the [Mongosync](http://github.com/TechEnterprises/mongosync) module.

It implements into `hook_mongosync_entity_insert_preprocess`, and uses [Distill](http://github.com/TechEnterprises/distill) to process the entities into that Mongodb (compatable with a specific Meteor schema) can consume.

## Purpose
This module is meant to be a demonstration-piece for [a presentation](https://docs.google.com/presentation/d/1eheh9CTxQHnVVOPlP6iYvQMC-kSOA7UC4wl7nWU1kUo/edit?usp=sharing) on Meteor and Drupal integration, and building reactive Drupal applications. It is meant to sync data between a Drupal site, and [this Meteor application](https://github.com/TechEnterprises/meteor-introduction).

Keep in mind that this is purely conceptual. I'm currently working on other projects that implement the ideas demonstrated in this module in a modular way, so stay tuned :)

## Installation
* Install [Mongosync](http://github.com/TechEnterprises/mongosync), and configure it to point to your Meteor app.
* Install [Distill](http://github.com/TechEnterprises/distill).
* Install this module
* Create a content type that you would like to sync with Meteor.
* Configure Mongosync to sync that entity to a sensible collection.
* Create an entity of that content type.
* Ensure that the entity is processed, and sent to Meteor.
