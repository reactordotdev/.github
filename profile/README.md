# Reactor.dev

Reactor.dev makes it easy for professionals to build a software business by handling the tedium of making good default choices for deploying code into production.

The biggest problem with vibecoding is that it is hard for non-tech practitioners to suffer through the learning curves of the software platforms that are fighting for your business and trying to lock you into their ecosystem. 

Rails is so close to getting you there, but you still need to understand enough about software to get going. You can diligently read the rails guides but in today's world that doesn't win. Why would you suffer through the Rails guides when v0 and lovable and bolt all given you a tantalizing prompt that makes it feel like you have the website pretty much done. They all throw you to the wolves (i.e. all the tools trying to capitalize on the demand that these app generators are creating).

One of the core ideas guiding rails is [Conceptual Compression](https://youtu.be/zKyv-IGvgGE?si=nQgYtWJZ2MFvVVSH&t=1047). Conceptual compression is the idea that we have a lot of concepts that we have to consider when building applications but that we can ignore some of the details by building good abstractions. Those abstractions won't be perfect and you might need to dive in and learn more deeply at a particular point in time when things start to challenge the abstraction (see [leaky abstractions](https://en.wikipedia.org/wiki/Leaky_abstraction)) but you only need to do that when (if ever) your software demands that of you. 

Rails does an exceptional job here for the application development yourself, but in production it leaves you to draw the rest of the owl. Rails has started making this easier by developing kamal, but that misses alerting on errors, product analytics, payments, user management, and more to the developer; which is fantastic for flexibility, but hard for a professional using a vibecoding tool to get a product that someone can pay for online and suppotable. And if they do get a bunch of SaaS tools together they have to manage them all they are all terribly integrated so you can't tell if your most important customer is having a bad user experience or if your product has broken. 

Heroku is still the gold standard for devex but I don't think it should be. We have moved on as an industry and we can have a world class experience from start to end.

To start, reactor.dev makes some opinionated deviations from the rails stack.

For javascript, we use vite and bun instead of importmaps. By using bun, we have a javascript runtime that doesn't need a seperate installer. 

We can make a faster CI/CD pipeline by supporting an opinionated Dockerfile and creating a base-image that already includes the common dependencies and is cached on the build server (or run locally!). 

We can build local-first CI/CD checks so that we're not waiting on github actions to spin up a VM in some cloud somewhere that is trying to any arbitrary task.

We can build an initial data model that is built for AI-first SaaS products so that non-tech professionals can build tools that are secure, scalable and easy to develop on top of.

We can build an rails development environment that includes all the MCP tools that make AI development actually work. 

We can build an application generator that has the context of our opinionated defaults.

But the key is that this should all be vertically integrated so that different parts of the system can build off of each other.

I'm really excited by the democratization of software development and I can't wait to help enable the next generation of entrepreneurs.
