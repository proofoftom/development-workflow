# Development Workflow
 
* [Technologies](technologies.md)
* [Creating a New Site](creating_a_new_site.md)
* [Development](development.md)
* [Deployment](deployment.md)

An optimal workflow using a handful of community projects: Aquifer, Terra CLI, and OpenDevShop (and GitLab maybe?). I’ve started building out this GitBook to organize my thoughts.

For our staging server, [OpenDevShop](http://www.opendevshop.com/) grants us a ton of [continuous integration functionality out of the box](http://www.thinkdrop.net/blog-entry/may-12-2015-734pm/continuous-deployment-integration-testing-delivery-open-devshop) and is way more production ready than Terra at the moment. There is a lot of momentum picking up around Terra as we speak where the end goal is to replace the hosting components of Aegir and OpenDevShop with Terra interfaces. Join the [DevShop](https://gitter.im/opendevshop/devshop) and [Terra CLI](https://gitter.im/terra-ops/terra-cli) Glitters to get in on the discussion.

While you could theoretically use any \*AMP stack for local development, this focuses primarily on utilizing Terra CLI because:
* Heshan has already thoroughly documented its usage
* Is more lightweight than a DevShop VM
* Allows us to contribute to getting DevShop built on Terra
* Ridiculously easy to run test suites like Behat locally

Bringing us one step closer to DevOps nirvana.

Lastly, I’m a huge advocate of the drush make workflow (see: https://www.phase2technology.com/blog/creating-maintainable-sites-with-drush-make/) and a recently released Four Kitchens project http://aquifer.io/ would greatly help in transitioning any existing sites and would also streamline creating new ones. We’re not locked down to using the Drush make workflow though as Terra and OpenDevShop support regular site repositories which would allow us to transition as we go, although ideally we should push for all projects to be structured this way. Also, Aegir and OpenDevShop are more apt at reporting site information such as module/core versions and updates when a site is built with make.

This will bring us pretty damn close to DevOps nirvana. The next level will be to incorporate more automated/manual testing in to our projects as well, starting with implementing some simple linting as well as performing code reviews.