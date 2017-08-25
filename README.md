# HW0

This repository contains all the materials required for submission.

# Git Tutorial Screenshot

[This is the screenshot of completed git tutorial](https://github.ncsu.edu/akshetty/HW0/blob/master/Learning%20Git.PNG)

# Screencast on how to use hooks

[Click here to watch the demo](https://youtu.be/zw66U4dyg7g)

# Concepts

**1)** *In your own words, explain the difference between continuous integration, continuous delivery, and continuous deployment.*

Continuous Integration means automatically building and testing, after merging all the changes that have been made to source code.
Continuous Delivery is the process of automatically building, testing, packaging and deploying the code to run in a production-like environment.
Continuous Deployment includes all the process covered by previous two steps, with the addition of automatically deploying the source code to production environment/s. 

CI is a subset of continuous delivery and deployment. It ensures that the modification done on source code are safe to be deployed.
Continuous Delivery automates the process of ensuring that the source code is ready to be deployed in production by an authorized entity.
Continuous Deployment automates the whole process of software lifecycle from integration to deployment.

**2)** *How does DevOps team model (e.g., site reliability engineer) differ than a a NoOps team model (e.g. Netflix team)? What differences in architecture allow for a NoOps model?*

In a DevOps team model, the Dev team is in charge of integrating, building and deploying the code on a production like environment (usually called as staging env.). They ensure that the code is of sufficient quality for actual use by taking care of its lifecycle in staging env. The Operations team is in charge of deploying the code on staging to production env. This means that Ops team take charge of scaling and maintaining the application on production. 

In a NoOPs model, the Dev team need not be concerned of the underlying infrastructure/ operations. Their only concern is with the development and quality of code. The infrastructure or operations is provided to the Dev team, and they can choose to scale or modify it as per their requirement. This is similar to hosting the application in sites like Heroku.

Thus the difference in architecture stems from the fact that in DevOps, a developer has responsibility to develop code as well as manage environment. In NoOps, the developer has to manage code and nothing else.

**3)** *Explain the principle of Every Feature is an Experiment.*

In a traditional development environment, addition of new feature to an application was considered in depth and then developed, with the hope that it will be accepted by the end user and persist.

However, the principle of treating every feature as an experiment, entails that a feature will eventually become obsolete. To track if a feature has become obsolete, data analytics is employed to check how well the feature is being taken by the end-user. If the feature is not being used or its usage has shrunk, it is either modified or removed.

This helps team to introduce new ideas with relative ease, and the data analytics takes care of the longevity/ modifications of the feature.

**4)** *Explain the principle of Be Fast to Deploy, Slow(er) to Release.*

This principle gives a developer power to test a new feature in an actual production environment. Usually this feature (also called as dark release) is hidden from the end-user. Thus, the developer can perform various analysis of the feature, without endangering the user experience. 

If the developer is content, the feature is made available to the public, else it is taken down.This is very helpful in situations where a replica of production is hard or infeasible to make.

However, there can be side effects of this experiment. Introduction of a malformed feature can cause blackouts. It might also be difficult to take down the feature if it is not integrated properly.

