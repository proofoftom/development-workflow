# Development Workflow
 
* [Technologies](technologies.md)
  * [Aquifer](aquifer.md)
  * [Terra CLI](terra.md)
  * Drupal VM
  * [DevShop](devshop.md)
* [Creating a New Site](creating_a_new_site.md)
  * [From Scratch](from_scratch.md)
  * [From Existing Files](from_existing_files.md)
* [Development](development.md)
* [Deployment](deployment.md)

## Overview

This is the collaborative concept of an ideal workflow. It leverages a handful of community projects as well as their respective philosophies. Projects include Aquifer, Terra CLI and DevShop, but others could prove useful as well. I started this documentation to organize my own thoughts. The instantiation of these thoughts is still in the works.

### Staging Server

For our staging server, [DevShop](http://getdevshop.com/) will grant us a lot of [continuous integration functionality out of the box](http://www.thinkdrop.net/blog-entry/may-12-2015-734pm/continuous-deployment-integration-testing-delivery-open-devshop) and is more production ready than Terra at the moment. There is a good amount of momentum picking up around Terra as we speak where the end goal is to replace the hosting components of Aegir and DevShop. Join the [DevShop](https://gitter.im/opendevshop/devshop) and [Terra CLI](https://gitter.im/terra-ops/terra-cli) Gitters to get in on the discussion.

### Local Development

While you could theoretically use any \*AMP stack for local development, this focuses primarily on utilizing Terra CLI because it:
* Has already been thoroughly internally documented by Heshan
* Is more lightweight than a DevShop VM
* Allows us to contribute to a DevShop built on Terra
* Is ridiculously easy to run test suites like Behat locally

Bringing us one step closer to DevOps nirvana, making us rockstar contributors along the way.

### Drush Make

Lastly, I’m an evangelist of the [drush make workflow](https://www.phase2technology.com/blog/creating-maintainable-sites-with-drush-make/). A recently released project called [Aquifer](http://aquifer.io/) helps in transitioning existing sites while also streamlining new ones. We’re not locked down to using the Drush make workflow as Terra and DevShop support regular site repositories which allows us to transition as we go. Ideally though we should push for all projects to be built with Aquifer. Also, Aegir and DevShop (by inheritance) are more geared towards sites built from make files.

This brings us pretty damn close to DevOps nirvana.

### Further Enlightenment

The next level will be to incorporate more automated/manual testing starting with some simple code linting along with performing code reviews.