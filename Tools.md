<h1 align="center">Tools</h1>

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
- [Cypress](#Cypress)
- [Jupyter](#Jupyter)
- [LocalStack](#LocalStack)

## Cypress
``` We keep receiving positive feedback on "post-Selenium" web UI testing tools such as``` [Cypress,](http://www.cypress.io/) [TestCafe](https://www.thoughtworks.com/radar/tools/testcafe) ```and``` [Puppeteer.](https://www.thoughtworks.com/radar/languages-and-frameworks/puppeteer) ```Running end-to-end tests can present challenges, such as the long duration of the running process, the flakiness of some tests and the challenges of fixing failures in CI when running tests in headless mode. Our teams have had very good experiences with Cypress by solving common issues such as lack of performance and long wait time for responses and resources to load. Cypress has become the tool of choice for end-to-end testing within our teams```

## Jupyter
``` Over the past couple of years, we've noticed a steady rise in the popularity of``` **analytics notebooks.** ```These are Mathematica-inspired applications that combine text, visualization and code in a living, computational document.``` [Jupyter Notebooks](https://jupyter.org/) ```are widely used by our teams for prototyping and exploration in analytics and machine learning. It has emerged as the current default for Python notebooks. However, we caution to use``` [Jupyter Notebooks in production.](https://www.thoughtworks.com/radar/techniques/productionizing-jupyter-notebooks)

## LocalStack
```One of the challenges of using cloud services is being able to``` **develop and test locally.** [LocalStack](https://github.com/localstack/localstack) ```solves this problem for``` [AWS](https://www.thoughtworks.com/radar/platforms/aws) ```by providing local``` [test double](https://martinfowler.com/bliki/TestDouble.html) ```implementations of a wide range of AWS services,``` **including S3, Kinesis, DynamoDB and Lambda.** ```It builds on top of best-of-breed tools such as``` [Kinesalite,](https://github.com/mhart/kinesalite) [dynalite](https://github.com/mhart/dynalite) ```and``` [Moto](https://github.com/spulec/moto) ```and adds isolated processes and error injection functionality. LocalStack is very easy to use, ships with a simple JUnit runner and a JUnit 5 extension and can also``` **run inside a docker container.** ```For many teams, it has become the default for testing services that are deployed on AWS.```
