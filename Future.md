Future Technologies
===

Revolutions are going on right now in the IT industry. I feel informing you of this is my responsibility. All of the things I am about to mention have the opportunity to save us time, resources and up-time. Unlike usual, I am going to try and keep this short and sweet in an effort for you to read it.

- Markdown
- Source Control ([Github](http://www.github.com "Github"), [Visual Studio](https://www.visualstudio.com/products/what-is-visual-studio-online-vs "Visual Studio Online"), ...)
- Build Testing ([Appveyor](http://www.appveyor.com/ "Appveyor"), [Visual Studio](https://www.visualstudio.com/products/what-is-visual-studio-online-vs "Visual Studio Online"), [Pester](https://github.com/pester/Pester "Pester (PowerShell Tester)"), ...)
- Configuration Management ([Chef](http://www.chef.io "Chef"), [PuppetLabs](http://www.puppetlabs.com "Puppet"), [PowerShellDSC](https://github.com/PowerShell "PowerShell"), ...)
- Containers (VMWare, Hyper-V, [Docker](http://www.docker.com "Docker"), ...)

# That's it! You can stop reading here #

## If you want to know more about what I am talking about, keep reading ##

# Details #
### Markdown ###
This document is a markdown document. View it raw [here](https://github.com/enu235/enu235.github.io/raw/master/Future.md "Raw"). Markdown is quickly becoming the standard documentation method because it is easily readable, works well in development environments like GIT where built-in version control exists, and is easy to learn.

### Source Control and Build Testing ###
Changes kill. Source control saves. When your environment is controlled by a source engine like Git, all changes are well understood, documented and tested before being committed. Full test environments can be spun up for team approval, comments and more.

Why manually test when you have build engines like Appveyor.com and VisualStudio.com that can run your changes through a series of actions and test before you even have the ability to approve or move forward. One person finds a fix and updates the configurations for resolution. Approval depends on the build engine creating a virtual test and running it through a series of loops to see if all required test are passed. If things fail, either the configuration needs to be dumped/fixed or the build engine needs to be updated to handle the new way things are being done. After all adjustments are made the required individuals can either approve or disapprove of the change. If approved, the changes are committed, but that is not the end. Though everything was done properly, if things still go wrong in production, the change can be rolled back simply and everyone looking at the configuration will naturally see the current version.

### Configuration Management ###
This is the tie that binds everything (Markdown, Source Control and Build Testing) together. Nearly all of our devices, operating systems and services can be managed through these modern configuration engines. Though it is still early, this industry is growing at an extreme pace. It works by allowing the administrator to create a configuration document that would be in source control that defines the configuration of the managed item. When the managed item needs to change, the configuration document changes. This at first makes complete since when thinking about servers and applications, but it does completely apply to things like VMWare, Network devices and so on. In VMWare, the configuration document would be processed on something like the VCenter server, network devices would be controlled by dedicated server/container processing through the document and directly interacting with the device(s). Using this method is also a great benefit when automation starts to kick in. Since the configuration is merely a text document, the automation engine does not need to understand the logic/technology it is controlling. The automation engine just adds a text block for a new item or modifies an existing text block to update a managed item or series of items.

### Containers ###
Today we use virtualization to isolate workload. This virtualization has allowed us to make great strides forward and it is time to keep moving on to containers that do much the same thing in a much more effective and controllable way. A good example of this is a SMTP (Simple Mail Transport Protocol) server, which we run as an independent virtual machine today that takes up 20 GB of hard drive space and GBs of memory. Though the hard drive space and memory is deduped, the SMTP service only takes a few MB of disk and memory. When it all boils down, we are doing a lot more work than we should, and adding more points of failure. We need to start preparing for this future today. Technologies like DNS and DHCP have to be ready for this so why wait to start making preparations.
