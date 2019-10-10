<h1 align="center">Techniques</h1>

<div align="center">
  :stars::ship::ship::ship::ship::ship:
</div>
<div align="center">
  <strong>Elements of a software development process,practices</strong>
</div>
<div align="center">
  A <code>4kb</code> framework for creating a tech culture
</div>

<br />

<div align="center">
  <!-- Stability -->
  <a href="https://nodejs.org/api/documentation.html#documentation_stability_index">
    <img src="https://img.shields.io/badge/stability-experimental-orange.svg?style=flat-square"
      alt="API stability" />
  </a>  
  <!-- Build Status -->
  <a href="https://travis-ci.org/choojs/choo">
    <img src="https://img.shields.io/travis/choojs/choo/master.svg?style=flat-square"
      alt="Build Status" />
  </a>
  <!-- Test Coverage -->
  <a href="https://codecov.io/github/choojs/choo">
    <img src="https://img.shields.io/codecov/c/github/choojs/choo/master.svg?style=flat-square"
      alt="Test Coverage" />
  </a>
  <!-- Downloads -->
  <a href="https://npmjs.org/package/choo">
    <img src="https://img.shields.io/npm/dt/choo.svg?style=flat-square"
      alt="Download" />
  </a>
  <!-- Standard -->
  <a href="https://standardjs.com">
    <img src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square"
      alt="Standard" />
  </a>
</div>

<div align="center">
  <h3>
    <a href="https://github.com/AdyKalra/technologyradar/blob/master/Tools.md">
      Tools
    </a>
    <span> | </span>
    <a href="https://github.com/AdyKalra/technologyradar/edit/master/Techniques.md">
      Techniques
    </a>
    <span> | </span>
    <a href="https://github.com/AdyKalra/technologyradar/blob/master/Platforms.md">
      Platforms
    </a>
    <span> | </span>
    <a href="https://github.com/AdyKalra/technologyradar/blob/master/Programming%20Languages%20and%20Frameworks.md">
      Languages and Frameworks
    </a>
    </h3>
</div>

<div align="center">
  <sub>The little framework that could. Built with ❤︎ by
  Ady Kalra</a> and
    inspired by thoughtworks
  </a>
</div>

## Table of Contents
- [Four Key Metrics](#four-key-metrics)
- [Micro Frontends](#Micro-Frontends)
- [Opinionated and automated code formatting](#Opinionated-and-automated-code-formatting)
- [Secrets as a service](#Secrets-as-a-service)
- [Chaos Engineering](#Chaos-Engineering)
- [Crypto shredding](Crypto-shredding)

## Four Key Metrics

```The thorough ```[State of DevOps](https://cloud.google.com/devops/) ```reports have focused on data-driven and statistical analysis of high-performing organizations. The result of this multiyear research, published in ```[Accelerate](https://itrevolution.com/book/accelerate/)```, demonstrates a direct link between organizational performance and software delivery performance. The researchers have determined that only four key metrics differentiate between low, medium and high performers:``` **lead time, deployment frequency, mean time to restore (MTTR) and change fail percentage.** ``` Indeed, we've found that these four key metrics are a simple and yet powerful tool to help leaders and teams focus on measuring and improving what matters. A good place to start is to instrument the build pipelines so you can capture the four key metrics and make the software delivery value stream visible.``` [GoCD pipelines](https://www.gocd.org/)```, for example, provide the ability to measure these four key metrics as a first-class citizen of the``` [GoCD analytics.](https://www.gocd.org/analytics.html)

```The State of DevOps report, first published in 2014, states that high-performing teams create high-performing organizations. Recently, the team behind the report released Accelerate, which describes the scientific method they've used in the report. A key takeaway of both are the four key metrics to support software delivery performance: lead time, deployment frequency, mean time to restore (MTTR), and change fail percentage. As a consultancy that has helped many organizations transform, these metrics have come up time and time again as a way to help organizations determine whether they're improving the overall performance. Each metric creates a virtuous cycle and focuses the teams on continuous improvement: to reduce lead time, you reduce wasteful activities which, in turn, lets you deploy more frequently; deployment frequency forces your teams to improve their practices and automation; your speed to recover from failure is improved by better practices, automation and monitoring which reduces the frequency of failures.```

## Micro Frontends
```We've seen significant benefits from introducing``` [microservices](https://martinfowler.com/articles/microservices.html)```, which have allowed teams to scale the delivery of independently deployed and maintained services. Unfortunately, we've also seen many teams create a frontend monolith — a large, entangled browser application that sits on top of the backend services — largely neutralizing the benefits of microservices. Since we first described``` **micro frontends** as a technique to address this issue, we've had almost universally positive experiences with the approach and have found a number of patterns to use micro frontends even as more and more code shifts from the server to the web browser. So far,``` [web components](https://www.thoughtworks.com/radar/platforms/web-components-standard) ```have been elusive in this field, though.```

## Opinionated and automated code formatting 
```For as long as we can remember, what style to use for formatting code has been a matter of personal taste, company policy and heated debate. Finally, the industry appears to be tiring of this endless argument and teams are freeing up surprisingly large amounts of time by forgoing these discussions and just adopting``` **opinionated and automated code formatting tools**. ```Even if you don't agree 100% with the opinions of the various tools, the benefits of focusing on what your code does rather than how it looks is something most teams should be able to get behind.``` [Prettier](https://www.thoughtworks.com/radar/tools/prettier) ```has been getting our vote for JavaScript, but similar tools, such as``` [Black](https://github.com/ambv/black) ```for Python, are available for many other languages and are increasingly being built-in as we see with``` [Golang](https://golang.org/cmd/gofmt/) and [Elixir.](https://elixir-lang.org/blog/2018/01/17/elixir-v1-6-0-released/) ```The key here is not to spend hours discussing which rules to enforce, but instead pick a tool that is opinionated, minimally configurable and automated — ideally as a pre-commit hook.```

## Secrets as a service
```Humans and machines use secrets throughout the value stream of building and operating software. The build pipelines need secrets to interface with secure infrastructures such as container registries, the applications use API keys as secrets to get access to business capabilities, and the service-to-service communications are secured using certificates and keys as secrets. You can set and retrieve these secrets in different ways. We've long cautioned developers about using source code management for storing secrets. We've recommended``` [decoupling secret management from source code](https://www.thoughtworks.com/radar/techniques/decoupling-secret-management-from-source-code) ```and using tools such as``` [git-secrets](https://www.thoughtworks.com/radar/tools/git-secrets) ```and``` [Talisman](https://www.thoughtworks.com/radar/tools/talisman) ```to avoid storing secrets in the source code. We've been using``` **secrets as a service** ```as a default technique for storing and accessing secrets. With this technique you can use tools such as``` [Vault](https://www.thoughtworks.com/radar/tools/hashicorp-vault) ```or``` [AWS Key Management Service (KMS)](https://aws.amazon.com/kms/) ```to read/write secrets over an HTTPS endpoint with fine-grained levels of access control. Secrets as a service uses external identity providers such as``` [AWS IAM](https://aws.amazon.com/iam/) ```to identify the actors who request access to secrets. Actors authenticate themselves with the secrets service. For this process to work, it's important to automate bootstrapping the identity of the actors, services and applications. Platforms based on``` [SPIFFE](https://www.thoughtworks.com/radar/platforms/spiffe) ```have improved the automation of assigning identities to services.```

## Chaos Engineering
```accepted, mainstream approach to improving and assuring distributed system resilience. As organizations large and small begin to implement Chaos Engineering as an operational process, we're learning how to apply these techniques safely at scale. The approach is definitely not for everyone, and to be effective and safe, it requires organizational support at scale. Industry acceptance and available expertise will definitely increase with the appearance of commercial services such as```[Gremlin](https://www.thoughtworks.com/radar/tools/gremlin) ```and deployment tools such as``` [Spinnaker](https://www.thoughtworks.com/radar/tools/spinnaker) ``` implementing some Chaos Engineering tools.```

**Chaos Katas** ```is a technique that our teams have developed to train and upskill infrastructure and platform engineers. It combines Chaos Engineering techniques—that is, creating failures and outages in a controlled environment—with the systematic teaching and training approach of Kata. Here,``` [Kata](https://en.wikipedia.org/wiki/Kata) ```refers to code patterns that trigger controlled failures, allowing engineers to discover the problem, recover from the failure, run postmortem and find the root cause. Repeated execution of Katas helps engineers to internalize their new skills.```

## Crypto shredding
```Maintaining proper control over sensitive data is difficult, especially when it's copied outside of a master system of record for backup and recovery purposes. Crypto shredding is the practice of rendering sensitive data unreadable by deliberately overwriting or deleting encryption keys used to secure that data. Considering there are systems, such as audit application or blockchain, that should not or could not delete historical records, this technique is quite useful for privacy protection and``` [GDPR](https://www.thoughtworks.com/insights/blog/gdpr-it-s-time-rethink-your-approach-privacy) ```compliance.```
