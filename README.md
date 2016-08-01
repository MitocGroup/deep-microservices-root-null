deep-microservices-root-vanilla
===============================

[![Build Status](https://travis-ci.org/MitocGroup/deep-microservices-root-vanilla.svg?branch=master)](https://travis-ci.org/MitocGroup/deep-microservices-root-vanilla)
[![Test Coverage](https://codeclimate.com/repos/5789fe0f60cba5007800658b/badges/326a841f5de4a64b9019/coverage.svg)](https://codeclimate.com/repos/5789fe0f60cba5007800658b/coverage)

deep-microservices-root-vanilla is the fundamental building block used by cloud-native web applications
built on top of [DEEP Framework](https://github.com/MitocGroup/deep-framework) and
[Vanilla JS](http://vanilla-js.com). This microservice provides the root structure of the web application 
that is developed in vanilla / plain JavaScript, without using any framework like AngularJS or ReactJS.


## Getting Started

### Step 1. Pre-requisites

- [x] [Create an Amazon Web Services account](https://www.youtube.com/watch?v=WviHsoz8yHk)
- [x] [Configure AWS Command Line Interface](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html)
- [x] [Get Started - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [x] [JDK 8 and JRE 8 Installation Start Here](https://docs.oracle.com/javase/8/docs/technotes/guides/install/install_overview.html)
- [x] [Install nvm](https://github.com/creationix/nvm#install-script) and [use node v4.3+](https://github.com/creationix/nvm#usage)
- [ ] Install DEEP CLI, also known as `deepify`:

```bash
npm install deepify -g
```

> If you want to use `deepify` on Windows, please follow the steps from
[Windows Configuration](https://github.com/MitocGroup/deep-framework/blob/master/docs/windows.md)
before running `npm install deepify -g` and make sure all `npm` and `deepify` commands are executed
inside Git Bash.

### Step 2. Install Microservice(s) Locally

```bash
deepify install github://MitocGroup/deep-microservices-root-vanilla ~/deep-microservices-root-vanilla
```

> Path parameter in all `deepify` commands is optional and if not specified, assumes current
working directory. Therefore you can skip `~/deep-microservices-root-vanilla` by executing
`mkdir ~/deep-microservices-root-vanilla && cd ~/deep-microservices-root-vanilla` before `deepify install`.

### Step 3. Run Microservice(s) in Development

```bash
deepify server ~/deep-microservices-root-vanilla -o
```

> When this step is finished, you can open in your browser the link *http://localhost:8000*
and enjoy the deep-microservices-root-vanilla running locally.

### Step 4. Deploy Microservice(s) to Production

```bash
deepify deploy ~/deep-microservices-root-vanilla
```

> Amazon CloudFront distribution takes up to 20 minutes to provision, therefore don’t worry
if it returns an HTTP error in the first couple of minutes.

### Step 5. Remove Microservice(s) from Production

```bash
deepify undeploy ~/deep-microservices-root-vanilla
```

> Amazon CloudFront distribution takes up to 20 minutes to unprovision. That's why `deepify`
command checks every 30 seconds if it's disabled and when successful, removes it from your account.


## Developer Resources

Having questions related to deep-microservices-root-vanilla?

- Ask questions: https://stackoverflow.com/questions/tagged/deep-framework
- Chat with us: https://mitocgroup.slack.com/messages/general
- Send an email: feedback@deep.mg

Interested in contributing to deep-microservices-root-vanilla?

- Contributing: https://github.com/MitocGroup/deep-microservices-root-vanilla/blob/master/CONTRIBUTING.md
- Issue tracker: https://github.com/MitocGroup/deep-microservices-root-vanilla/issues
- Releases: https://github.com/MitocGroup/deep-microservices-root-vanilla/releases
- Roadmap: https://github.com/MitocGroup/deep-microservices-root-vanilla/blob/master/ROADMAP.md

Looking for web applications that use (or are similar to) deep-microservices-root-vanilla?

- Hello World: https://hello.deep.mg | https://github.com/MitocGroup/deep-microservices-helloworld
- Todo App: https://todo.deep.mg | https://github.com/MitocGroup/deep-microservices-todomvc
- Enterprise Software Marketplace: https://www.deep.mg


## Sponsors

This repository is being sponsored by:
- [Mitoc Group](https://www.mitocgroup.com)
- [DEEP Marketplace](https://www.deep.mg)

This code can be used under MIT license:
> See [LICENSE](https://github.com/MitocGroup/deep-microservices-root-vanilla/blob/master/LICENSE) for more details.
