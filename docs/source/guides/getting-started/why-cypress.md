---
title: Why Cypress?
comments: false
---

{% note info %}
# {% fa fa-graduation-cap %} What You'll Learn

- What Cypress is, and why you should use it
- Who Cypress is built for
- Key Cypress features
- Our mission, and what we believe in
{% endnote %}

# In a Nutshell

Cypress is a next generation front end testing tool built for the modern web. We address the key pain points developers and QA engineers face when testing modern applications.

We make it simple to:

- {% urlHash 'Setup tests' Setup-Tests %}
- {% urlHash 'Write tests' Write-Tests %}
- {% urlHash 'Maintain tests' Maintain-Tests %}

Cypress is most often compared to Selenium; however Cypress is both fundamentally and architecturally different. Cypress is not  constrained by the same restrictions as Selenium.

This enables you to **write faster**, **easier** and **more reliable** tests.

# Who Uses Cypress?

Our users are typically developers or QA engineers building web applications using modern JavaScript frameworks.

Cypress enables you to write all types of tests:

- End to end tests
- Integration tests
- Unit tests

Cypress can test anything that runs in a browser.

# Cypress Ecosystem

Cypress is a free, open source, {% url "locally installed" installing-cypress %} testing tool **and** a service for {% url 'recording your tests' features %}.

- ***First:*** Cypress makes it easy to setup and start writing tests every day while you build your application locally. *TDD at its best!*
- ***Later:*** After building up a suite of tests and {% url "integrating Cypress" continuous-integration %} with your CI Provider, our  {% url 'Dashboard' features %} can record your test runs. You'll never have to wonder: *Why did this fail?*

# Our Mission

Our mission is to build a thriving, open source ecosystem that enhances productivity, makes testing an enjoyable experience, and generates developer happiness. We hold ourselves accountable to champion a testing process **that actually works**. We believe our documentation should be simple and approachable. This means  enabling ours readers to fully understand not just the **what** but **why**.

We want to help developers build a new generation of modern applications faster, better, and without the stress and anxiety associated with managing tests and their eventual, inevitable failures.

We know that in order for us to be successful we must enable, nurture, and foster an ecosystem that thrives on open source. Every line of test code is an investment in **your codebase**, it will never be coupled to us as a paid service, or company. Tests will be able to run and work independently, *always*.

We believe testing needs a lot of love, and we are here to build a tool, a service, and a community that everyone can learn and benefit from. We're solving the hardest pain points shared by every developer working on the web. We believe in this mission and hope that you will join us to make Cypress a lasting ecosystem that helps everyone win.

# Features

Cypress comes fully baked, batteries included.

## Setup Tests

- **Get Started in Minutes.** Don't spend days setting up a test environment. Just {% url "install our desktop app" installing-cypress %}, {% url "add your project" testing-your-app#Adding-Your-Project %} and {% url "start testing" writing-your-first-test %}!
- **No Changes to your Code.** You don't need to change your code and Cypress doesn't need to modify your code.
- **No Dependencies.** There's no need to download Selenium, Webdriver, Node, or any other code dependencies to get your tests up and running.
- **ES2015 Friendly:** Write modern code with zero configuration.
- **Launch Browsers.** Cypress can automatically launch your locally installed `Chrome` browsers, but also comes baked with the ability to run headlessly using `Electron`.

{% img /img/guides/setup-tests.gif %}

## Write Tests

- **Time Travel Snapshots:** {% url "Step back through" overview-of-the-gui %} every command issued during a test.
- **Easily Debug.** Use [Chrome DevTools](https://developer.chrome.com/devtools) while tests run. We even support {% url `debugger` debugging %} in both your test code and your application code.
- **Real-time Updates.** Cypress automatically re-runs whenever you make changes.
- **Automatic Waiting.** Never add waits or sleeps to your tests. {% url 'Cypress intelligently waits' introduction-to-cypress#Default-Assertions %} for commands to resolve before moving on.
- **Control Network Traffic.** Easily {% url 'control, stub, and test edge cases' network-requests %} without involving your server. You can modify network traffic however you like.
- **Simple API.** {% url "Every command" api %} uses a simple, readable, and familiar API to locate and verify elements on a page.

{% img /img/guides/write-tests.gif %}

## Maintain Tests

- **Consistent Results.** Our architecture doesn't use Selenium or Webdriver. Say goodbye to slow, brittle, and flaky tests.
- **Continuous Integration.** Cypress supports {% url "TravisCI" https://travis-ci.org/ %}, {% url "Jenkins" https://jenkins.io/ %}, {% url "CircleCI" https://circleci.com/ %}, {% url "Codeship" https://codeship.com/ %}, or any service running {% url 'Docker' images %}.
- **Screenshots & Videos:** Cypress automatically takes {% url 'screenshots' screenshots-and-videos %} on failed tests and records a {% url 'video' screenshots-and-videos %} of headless runs.
- **Understand Failures:** Our {% url 'Dashboard Service' features %} can record all of your tests and help you pinpoint and understand failures.
- **Excellent Support.** Get stuck? We're here to help you. {% open_an_issue "Open an issue" %}, join us in {% url "our Gitter chat" https://gitter.im/cypress-io/cypress %}, [email us](mailto:support@cypress.io), or {% url "ask a question on Stackoverflow" https://stackoverflow.com/search?q=cypress.io %}.

{% img /img/guides/maintain-tests.gif %}