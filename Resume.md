# Resume

Hi there, my name is Pietro and I currently work at the BBC as the technical lead/principal web developer for their responsive news frameworks team. Our goal is to move BBC News (and related products) from their current stack to a cloud based infrastructure. I'm also a published author: [Pro Vim](http://www.amazon.co.uk/Pro-Vim-Mark-McDonnell/dp/1484202511/ref=sr_1_1)

---

You can find me online at the following locations:

- [integralist.co.uk](http://www.integralist.co.uk/)
- [github.com/integralist](https://github.com/integralist)
- [twitter.com/integralist](http://www.twitter.com/integralist)

---

## Table of Contents

- [BBC](#bbc)
- [Career highlights](#career-highlights)
- [Skills](#skills)
- [Published](#published)
- [Open Source Projects](#open-source-projects)
- [Previously](#previously)
- [Summary](#summary)

---

## BBC

I joined the BBC as a client-side specialist, before moving over to work primarily on the server-side. This has given me an understanding, appreciation and knowledge of the "full stack" workflow. My job at the BBC generally involves the following (agile) processes and tools…

### tooling

- [Vagrant](http://www.vagrantup.com/)
- [Docker](http://www.docker.com/)
- Continuous Integration
	- [Travis CI](https://travis-ci.org/)
	- [Jenkins](http://jenkins-ci.org/)
- [Vim](http://www.vim.org/about.php) and [tmux](http://tmux.sourceforge.net/)
	- I wrote a book on the topic called [Pro Vim](http://www.apress.com/9781484202517) (published by [Apress](https://www.apress.com/))
- [GruntJS](http://gruntjs.com/)
- [Tmate](http://tmate.io/) (for remote pair programming)
- [Git](http://git-scm.com/) Version Control System
	- Workflow involves: 
		- Ruthlessly small PRs
		- Rebase/Squash all commits into single commit (use GitHub's `Closes #123` and `Fixes #456` feature)
		- Cherry pick commit into `master` (GitHub will close the PR and any associated Issues automatically)
- [Trello](http://www.trello.com/) for Kanban tasks and workflow
- [Slack](https://slack.com/) for project collaboration

### back-end

- [JRuby](http://jruby.org/)
	- Cloud based applications using the BBC's "Cosmos" service
	- AWS ([CloudFormation](http://aws.amazon.com/cloudformation/), [EC2](http://aws.amazon.com/ec2/), [S3](http://aws.amazon.com/s3/), [DynamoDB](http://aws.amazon.com/dynamodb/), [SQS](http://aws.amazon.com/sqs/))
	- Basic Linux administration (shell scripting)
- [PHP](http://php.net/)
	- Web Application built with [Zend Framework 1](http://framework.zend.com/manual/1.12/en/reference.html)
- TDD (using [RSpec](http://rspec.info/))
- BDD (using [Cucumber](http://cukes.info/) and [Capybara](https://github.com/jnicklas/capybara))

### front-end

- Building interfaces and components that are:
	- [Mobile first](http://www.abookapart.com/products/mobile-first)
	- [Responsive](http://www.abookapart.com/products/responsive-web-design) 
	- Performant ([networking](http://shop.oreilly.com/product/0636920028048.do) and [behaviour](http://shop.oreilly.com/product/9780596802806.do))
	- [Reusable](https://github.com/stubbornella/oocss/wiki)
		- Specifically using [BEM](http://www.integralist.co.uk/posts/bem.html)
		- We also use the [Sass](http://sass-lang.com/) CSS pre-processor
		- Semantic and well structured HTML
	- Simple
		- i.e. code isn't complected
		- e.g. have a [baseline](https://github.com/Integralist/CSS-Baseline), no "kitchen sink" approaches
- Constructing behaviours with:
	- Modular JavaScript
		- [AMD](https://github.com/amdjs/amdjs-api/blob/master/AMD.md)
		- [RequireJS](http://requirejs.org)
	- Patterns: 
		- Mediator (for complex modules that require a mediator to handle interactions)
		- PubSub (for simpler modules to help them stay decoupled)

## Career highlights

### 2015

- Co-authored and designed event archive and automation service utilising AWS Lambda (which at the time supported only NodeJS)
- Worked (both as a developer and technical lead) on BBC service for the May 7th General Election event
- Developed a [Clojure version](https://github.com/Integralist/spurious-clojure-aws-sdk-helper) of the open-source [Spurious Ruby AWS SDK Helper](https://github.com/spurious-io/ruby-awssdk-helper) library, which helps developers to develop locally against a subset of AWS resources
	- Along with a very basic [example Clojure application](https://github.com/Integralist/spurious-clojure-example)
- Supported my team's development of a re-usable monitoring and logging solution
- Co-developed new AWS/Cloud based foundation for BBC Newsbeat
	- Built utilising our open-sourced [BBC Alephant framework](https://github.com/BBC-News/alephant)

### 2014

- Working within a team that challenges itself to investigate and re-evaluate its stance on specific Ruby techniques and principles:
	- AOP, DI Containers, "JRuby native threads vs MRI GIL concurrency"
- Building (soon to be open-source) "Jello" application (integrating Trello with JIRA)
	- BBC utilises JIRA, but my team is more productive using Trello
	- We're required to provide visibility to other managers via JIRA
	- Hence we utilise the Trello API and JIRA REST API to provide synchronisation between the two
- Won two awards at the BBC Web Dev Gathering:
	- Best Public Relations of the Year (for my books [Pro Vim](http://www.apress.com/9781484202517) and [tmux Taster](http://www.apress.com/9781484207765))
	- Most innovative use of Technology (this was a team award for our use of [Docker](https://www.docker.com/) within our CI environment and Sandbox testing platform, and anywhere else we could find a fit for it)
- Co-designed and built the architecture for BBC Newsbeat
	- This architecture was a preface to the next important piece of work, which is to move the BBC Responsive News website from it's "old stack" to an AWS based cloud infrastructure
- Developed the new [Alephant framework information portal repository](https://github.com/BBC-News/alephant)
	- This included building the individual example applications (Sender/Renderer/Broker)
	- Utilising [Spurious](https://github.com/stevenjack/spurious) and [Spurious Browser](https://github.com/stevenjack/spurious-browser) to allow working with AWS resources locally
	- Writing top-level documentation for both the framework and example applications
- Given the opportunity to take on the acting Tech Lead role for the BBC News Frameworks team
- Our team managed to reach a level of Continuous Delivery that was previously not possible
	- This included (amongst other tests and monitoring checks) JSON Schema validation for external APIs
- Was tech lead for the Market Data project (which utilised our Alephant framework)
- Getting to work on solving problems around concurrency and distributed systems
- Enabled more teams to utilise the BBC's custom CLI based Cosmos tool
	- The tool was originally designed around the [CFNDSL](https://github.com/Integralist/cfndsl) Ruby DSL. 
	- The main purpose of the tool was to avoid having to write large JSON CloudFormation documents
	- It also allowed developers to automate the updating of CloudFormation and EC2 config (otherwise developers would have to manually copy and paste CloudFormation into a BBC specific GUI)
	- The issue with the tool was that some teams weren't keen on CFNDSL and so they kept to writing JSON (some used YAML and then converted it into JSON). This meant these teams were unable to take advantage of the tool (as it required CFNDSL)
	- I resolved the issue by updating the CLI tool to allow users to provide data as YAML or JSON thus avoiding the need for CFNDSL and enabling more BBC teams to automate their workflow
- Co-designed and built a CI workflow around static asset compilation
	- [Sequence Diagram](http://cl.ly/image/3W2n4526411n)
	- Used lots of shell scripting to connect each of the nodes together
- Co-designed and built a cloud based distributed load test tool
	- Uses [Apache JMeter](http://jmeter.apache.org/)
	- Utilises AWS [S3](http://aws.amazon.com/s3/), [SQS](http://aws.amazon.com/sqs/), [SNS](http://aws.amazon.com/sns/), [AutoScaling](http://aws.amazon.com/autoscaling/) and [CloudWatch](http://aws.amazon.com/cloudwatch/)
	- Infrastructure constructed using AWS [CloudFormation](http://aws.amazon.com/cloudformation/)
- Arranged [Sandi Metz](http://www.sandimetz.com/) "Object-Oriented Design" presentation
	- Was the first public developer gathering *within* the [BBC Broadcasting House](http://www.bbc.co.uk/broadcastinghouse/)
	- Sandi gave me an honoured mention in the opening of her talk which discussed her own personal journey hoping to one day give a presentation to the BBC (something her parents were happy to finally hear was happening)
- Took initiative to document the BBC Cosmos service
	- The original documentation was very terse and not useful to consumers
	- Any new understanding I accumulated whilst using the service was documented in a GitHub wiki
	- Ensured developers were kept up to date on any changes I was making (asking for feedback and input)
	- The hope was to garner interest in its use (helping us to move off the "old" stack and into cloud development)
- Worked on JRuby based back-end architecture for 2014 elections and Scottish Referendum
	- Utilised AWS ([SQS](http://aws.amazon.com/sqs/), [DynamoDB](http://aws.amazon.com/dynamodb/), [S3](http://aws.amazon.com/s3/)) 

### 2013

- Voted "Developer of the Year 2013"
- Led the development of the redesigned responsive navigation for BBC News
- I was invited to speak at the W3C Responsive Images meet-up
	- The event was hosted by [Mozilla](https://www.mozilla.org/) at their office in Paris
	- Other speakers and participants: [Google](https://www.google.com/), [Apple](https://www.apple.com/), [Microsoft](http://www.microsoft.com/), [Adobe](https://www.adobe.com/), [Opera](http://www.opera.com/), [W3C](https://www.w3.org/) and [Akamai]()
  - [Slides from my talk](https://speakerdeck.com/integralist/bbc-news-responsive-images)
- Selected to become a member of the BBC's [GEL Responsive Working Group](http://www.bbc.co.uk/gel)
- Integrated new BBC UX framework
	- Part of which meant developing a new multi break-point grid system with custom JS overlay (to aid development)
- Open-sourced and rewrote/automated the BBC's core responsive image technique
	- [Imager.js](https://github.com/BBC-News/Imager.js/)
	- Published a [blog post](http://responsivenews.co.uk/post/58244240772/imager-js) on the BBC's "Responsive News" blog about the process
- Developed a [PhantomJS](http://phantomjs.org/) prototype to automate the generation of an Application Cache manifest (for offline support)
	- I wrote a [blog post](http://www.integralist.co.uk/posts/appcache.html) and [open-sourced the project](https://github.com/Integralist/Squirrel). 
	- I've since converted it into a Node based command line tool to make it easier to use. It's available as an NPM module here: [https://npmjs.org/package/squirrel-js](https://npmjs.org/package/squirrel-js)
- Developed a design pattern library for modular/responsive components 
	- This work evolved into my open-source side project: [Stark](https://github.com/Integralist/Stark)
	- I wrote a [blog post](http://www.integralist.co.uk/posts/stark.html) about the process
- Ported JavaScript test suite (resulting in less bugs and allowing developers to be more expressive)
	- Originally used [QUnit](http://qunitjs.com/) 
	- Converted to [Jasmine](http://jasmine.github.io/)
		- Also integrated [Sinon.js](http://sinonjs.org/) and corresponding Jasmine Adapter
- Simplified over-engineered Sass/CSS architecture
- Built a new Sass image function
	- Written in Ruby
	- Takes URL as an argument and returns a Base64 encoded string
	- Code is [open-source](https://github.com/Integralist/Sass-Base64-Extension)
	- Works around IE8 "> 32kb" bug
- Refactored large chunks of code 
	- e.g. ~600 loc Sass mixin to a working 7 loc
- Introduced GruntJS to help different teams automate their processes
	- I open-sourced my findings into a project called [Grunt Boilerplate](https://github.com/Integralist/Grunt-Boilerplate)
- Co-developed the BBC News touch interaction photo gallery feature
- Gave a [presentation](https://slid.es/markmcdonnell/) on existing BBC News strategies and how they might be improved

## Skills

### Primary

- Ruby ([JRuby](http://jruby.org/) and [MRI](https://www.ruby-lang.org/))
- [Object-Oriented Code Design](http://www.integralist.co.uk/posts/ood.html)
	- Here's another of my blog posts, this time on "[message passing](http://www.integralist.co.uk/posts/message-passing.html)"
	- [Other design principles](https://gist.github.com/Integralist/9780188)
	- [Reducing context](https://gist.github.com/Integralist/9791615)
	- Concept of [simplicity](https://gist.github.com/Integralist/c7277cbacd53487b3bb0)
	- [S.O.L.I.D principles](https://gist.github.com/Integralist/9482527)
	- [AOP](https://gist.github.com/Integralist/9887248)
	- [Fun with lambdas](https://gist.github.com/Integralist/9994331)
- [Refactoring](http://www.integralist.co.uk/posts/refactoring-techniques.html)
	- [...and more](http://www.integralist.co.uk/posts/more-refactoring-techniques.html)
	- [Not all conditionals have an obvious refactoring pattern](https://gist.github.com/Integralist/9910271)
	- [Eigenclass](https://gist.github.com/Integralist/bb8760d11a03c88da151)
- Design Patterns
	- [MVCP](https://github.com/Integralist/MVCP)
	- [Ruby implementations](https://github.com/Integralist/Ruby-Design-Patterns)
	- [PHP implementations](https://github.com/Integralist/PHP-Design-Patterns)
- [Regular Expressions](http://www.regular-expressions.info/)
	- Including topics such as understanding "runnaway backtracking"
- Architecture design (e.g. I love drawing diagrams and graphs)
- Test-Driven Development
	- [Principles of good testing](https://gist.github.com/Integralist/7944948) 
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- Client-side performance and optimisation
- [Vim](http://www.vim.org/about.php)
- [tmux](http://tmux.sourceforge.net/)
- [Being a professional](http://www.integralist.co.uk/posts/clean-coder.html)

### Secondary

- [Meta Programming](https://gist.github.com/Integralist/a29212a8eb10bc8154b7)
- [Clojure](http://clojure.org/)
  	- I've started developing more with Clojure (I'm currently working on a an image processing application in my spare time called "Koinonia") as I find the language (and LISP in general) quite a pleasure to work with. My intention is to continue to increase my knowledge so I can push this into being a primarily language.
  	- [Spurious AWS SDK Helper](https://github.com/Integralist/spurious-clojure-aws-sdk-helper)
  	- [Homework from a "Brown Bag" session](https://gist.github.com/Integralist/f82dcb34a431e8fabf56#comment-1299405) 
  	- [Scratch Pad](https://gist.github.com/Integralist/11471364)
  	- [Understanding the power of destructuring](https://gist.github.com/Integralist/11376734)
- [PHP](http://php.net/)
- Shell Scripting
	- I wrote a blog post about [standard unix commands](http://www.integralist.co.uk/posts/unix-commands.html) (such as piping/redirection, `awk`, `sed`, `grep`, `find`, `xargs`, `tr` and others)
- [Data Structures](https://github.com/Integralist/Data-Structures)
- [AWS infrastructure](https://github.com/Integralist/CloudFormation)

### Interested in (but have not built anything substantial, yet)

- [Go](https://golang.org/)
	- I like the CSP (channel based) concurrency model they're using
	- The stripped back syntax, fast compiler, almost C-like speed and compositional code sharing are all nice features
- [Functional Programming](http://en.wikipedia.org/wiki/Functional_programming) (immutable state, referential transparency, currying and partial application etc)
	- I wrote a blog post about [understanding recursion in functional JavaScript programming](http://www.integralist.co.uk/posts/js-recursion.html)
	- Enjoy considering the differences between [OOP and FP](https://gist.github.com/Integralist/a96cf6d6f01d5d0cce0a)
	- I created a scratch pad of [functional concepts in JavaScript](https://gist.github.com/Integralist/b7ed2e337a0b5cbbecce)
- Workflows with Docker
	- I've created a [repository](https://github.com/Integralist/Linux-and-Docker-Development-Environment) 
		- Utilises Ruby within a Docker container
		- I provision the Ubuntu instance with specific developer essentials
		- Part of the the provisioning is ensuring Docker client can be accessed outside the VM
- [Node](http://nodejs.org/)
	- Although I've [built](http://www.integralist.co.uk/posts/appcache.html) some [tools](http://www.integralist.co.uk/posts/squirrel.html) using Node, I'm not necessarily a big fan
	- Would consider using only if it was the appropriate approach for the problem

### Past experiences

> This would be stuff I've used in the past and could probably pick up again if necessary

- JS libraries such as Ender & jQuery, along with the [MVC extension Backbone](http://www.integralist.co.uk/posts/backbone.html)
- ActionScript 3.0
- Classic ASP and an early ASP.NET

### Miscellaneous

> Stuff that just didn't fit anywhere else
 
- Developed my own [style guides](https://github.com/Integralist/Style-Guides) (although admittedly they could do with an update)

---

## Published

### [Apress](http://www.apress.com/)

I authored a printed book called "[Pro Vim](http://www.apress.com/9781484202517)" which was released November 2014.

### [Packt](https://www.packtpub.com/)

I was the technical reviewer for the book [GruntJS Cookbook](https://www.packtpub.com/web-development/gruntjs-cookbook-raw)

### [NET Magazine](http://www.creativebloq.com/net-magazine) (printed publication)

NET magazine asked me to write an article for a new comparison feature they were introducing at the time. This went to print the end of November 2013. You can read the article here: [DalekJS vs CasperJS](https://dl.dropboxusercontent.com/u/3687270/NetMag%20-%20Dalek%20vs%20Casper.pdf)

I also co-wrote an article called [8 ways to improve your grunt set-up](http://www.creativebloq.com/tutorial/8-ways-improve-your-grunt-set-111413407) ([PDF](https://dl.dropboxusercontent.com/u/3687270/NetMag%20-%20Grunt.pdf)) that went to print in the August 2014 edition.

### [Smashing Magazine](http://www.smashingmagazine.com/)

- [My author page](http://coding.smashingmagazine.com/author/mark-mcdonnell/)
- [How To Build A CLI Tool With Node.js And PhantomJS](http://coding.smashingmagazine.com/2014/02/12/build-cli-tool-nodejs-phantomjs/)
- [How To Build A Ruby Gem With Bundler, Test-Driven Development, Travis CI And Coveralls, Oh My!](http://coding.smashingmagazine.com/2014/04/08/how-to-build-ruby-gem-with-bundler-travis-ci-coveralls/)

### [NetTuts](http://net.tutsplus.com/)

- [My author page](http://tutsplus.com/authors/mark-macdonnell)
- [Testing Your Ruby Code With Guard, RSpec & Pry (Part 1 - Ruby/Guard/RSpec)](http://code.tutsplus.com/tutorials/testing-your-ruby-code-with-guard-rspec-pry--cms-19974)
- [Testing Your Ruby Code With Guard, RSpec & Pry (Part 2 - RSpec/Pry/Travis-CI)](http://code.tutsplus.com/tutorials/testing-your-ruby-code-with-guard-rspec-pry-part-2--cms-20290)

---

## Open Source Projects

### Alephant

[https://github.com/BBC-News/alephant](https://github.com/BBC-News/alephant)

> This is the main entry point for the Alephant framework. Which includes: Static publishing to S3 based on SQS messages; Supporting classes for inclusion in other Alephant gems; Using DynamoDB consistent read to enforce message order from SQS; Simple abstraction layer over S3 for get/put; Logger functionality for Alephant; Rendering HTML snippets using Mustache templating engine; Lookup for locations in S3 using DynamoDB; Providing an in-page preview of components during development.

I collaborated with the rest of the BBC News "Core Framework" team to help develop the suite of Alephant Ruby gems.

### Spurious Clojure AWS SDK Helper

[https://github.com/Integralist/spurious-clojure-aws-sdk-helper](https://github.com/Integralist/spurious-clojure-aws-sdk-helper)

> A helper library for configuring the AWS SDK to use Spurious (https://github.com/spurious-io/spurious)

### BBC Imager.js

[https://github.com/BBC-News/Imager.js](https://github.com/BBC-News/Imager.js)  

> Imager.js is an alternative solution to the issue of how to handle responsive image loading, created by developers at BBC News.

### Sinderella

[https://github.com/Integralist/Sinderella](https://github.com/Integralist/Sinderella)

> Ruby gem which will allow authors to pass a code block to transform a data object for a specific period of time

### Squirrel

[https://github.com/Integralist/Squirrel](https://github.com/Integralist/Squirrel)

> Node based cli tool using PhantomJS to automate generation of an Application Cache manifest file for a specified URL

### Grunt Boilerplate

[Grunt Boilerplate](https://github.com/Integralist/Grunt-Boilerplate)

> Boilerplate project structure using Grunt to take care of standard tasks such as: compiling AMD based modules using RequireJS, watching/compiling Sass into CSS, watching/linting JS code, running unit tests and more.

### Stark

[https://github.com/Integralist/Stark](https://github.com/Integralist/Stark)

> Simplified separation of components into decoupled applications. This isn't a framework (or all-encompassing suite of tools). It is a 'strategy', a pattern for handling the architecture of your code. Made possible via an elaborate Node based build script that compiles the components located within a web page.

### DOM Builder

[(https://github.com/Integralist/DOM-Builder](https://github.com/Integralist/DOM-Builder)

> Small utility script for easily generating a DOM structure

### DOMReady

[https://github.com/Integralist/DOMready](https://github.com/Integralist/DOMready)

> A very stable and robust cross browser 'DOM ready' function. Developed with help from @jdalton

### MVCP

[https://github.com/Integralist/MVCP](https://github.com/Integralist/MVCP)

> This is a Sinatra based application which implements the Presenter architectural pattern alongside the industry standard MVC pattern

### Style Guides

[https://github.com/Integralist/Style-Guides](https://github.com/Integralist/Style-Guides)

> My style guides for writing CSS, JavaScript, HTML, PHP, Ruby

### HTML5 Canvas "Image Slider" Game

[https://github.com/Integralist/HTML5-Image-Slider-Game](https://github.com/Integralist/HTML5-Image-Slider-Game)

> Built as part of a Facebook interview test (over the course of three days). Split image into puzzle pieces (and display in random order) and let user move pieces back together again. Works on mobile and desktop devices devices (using mouse and touch events).

---

## Previously

Prior to the BBC I worked for a creative agency called [Storm Creative](http://stormcreative.co.uk) from February 2001 - December 2012.

At Storm I was a technical lead under the role of 'Digital Media Manager' which included the following responsibilities… 

- Programming
	- front-end development
	- prototyping using latest tools and technologies
- Managing 'Digital Media' Department
	- Delegating work to staff (programmers)
	- Ensuring work is done on time
	- Handling staff questions/issues
	- Managing clients
	- Invoicing
	- Server management (Apache)
- Project Manager
	- Meeting with clients and understanding requirements
	- Booking in work with different departments (creative, copy writing)
	- Creating schematics/architecture of applications
	
Storm had carried out a lot of work for the NHS, Art Council, local government as well as local businesses and a two year long project called [LickList](http://www.licklist.co.uk). 

In 2012 Storm started work on a financial business venture called [Money Republic](https://moneyrepublic.com) which I was involved with the stage one build and over saw the project's technical architecture (pushing for the mobile first development process and responsive web design aspects), but it was my team who were responsible for the programming of most of the site with the exception of the home page's core feature which was a loan application widget which was heavily JavaScript based (along with other JavaScript heavy widgets throughout the site). 

Note: since leaving Storm the code base for Money Republic has changed significantly I'm afraid so much of what I had developed is no longer in use.

While managing the Digital Media Department I looked after a team of developers (two back-end and two front-end). After two years one of our front-end devs took the skills I had passed onto him and acquired a role at the London/American agency [Mint](http://mintdigital.com).

---

## Summary

I ideally want to get across two fundamental things about me:

1. I'm very passionate about programming and the openness of the web.
2. I love getting the chance to learn and experience new things.
