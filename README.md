# Development Workflow
 
* [Technologies](technologies.md)
* [Creating a New Site](creating_a_new_site.md)
* [Development](development.md)
* [Deployment](deployment.md)


## Overview

An optimal workflow using a handful of community projects: Aquifer, Terra CLI, and OpenDevShop (and GitLab maybe?). I started building this GitBook to organize my thoughts. The implementation of these thoughts is still in the works.

For our staging server, [OpenDevShop](http://www.opendevshop.com/) will grant us a lot of [continuous integration functionality out of the box](http://www.thinkdrop.net/blog-entry/may-12-2015-734pm/continuous-deployment-integration-testing-delivery-open-devshop) and is more production ready than Terra at the moment. There is also a lot of momentum picking up around Terra as we speak where the end goal is to replace the hosting components of Aegir and OpenDevShop. Join the [DevShop](https://gitter.im/opendevshop/devshop) and [Terra CLI](https://gitter.im/terra-ops/terra-cli) Glitters to get in on the discussion.

While you could theoretically use any \*AMP stack for local development, this focuses primarily on utilizing Terra CLI because it:
* Has already been thoroughly documented by Heshan
* Is more lightweight than a DevShop VM
* Allows us to contribute to getting DevShop built on Terra
* Is ridiculously easy to run test suites like Behat locally

Bringing us one step closer to DevOps nirvana, making us rockstar contributors along the way.

Lastly, I’m an evangelist of the [drush make workflow](https://www.phase2technology.com/blog/creating-maintainable-sites-with-drush-make/). A recently released project called [Aquifer](http://aquifer.io/) helps in transitioning existing sites while also streamlining new ones. We’re not locked down to using the Drush make workflow as Terra and OpenDevShop support regular site repositories which allows us to transition as we go. Ideally though we should push for all projects to be built with Aquifer. Also, Aegir and OpenDevShop (by inheritance) are more geared towards sites built from make files.

This brings us pretty damn close to DevOps nirvana.

The next level will be to incorporate more automated/manual testing as well, starting with some simple code linting and performing code reviews.