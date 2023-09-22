---
title: Web testing guidelines
description: Practical guidelines for unit, integration, and end-to-end testing on the web.
---

Practical guidelines for unit, integration, and end-to-end testing on the web. {% .lead %}

## Unit and integration testing

When writing unit and integration tests, these are three guidelines that we need to pay attention to:

1. [Query priorities](https://testing-library.com/docs/queries/about#priority)
2. [Testing appearance and disappearance](https://testing-library.com/docs/guide-disappearance/)
3. [Opting in for interactions instead of events](https://testing-library.com/docs/guide-events/#interactions-vs-events)

Please make sure that all questions and assertions in your test files follow those testing guidelines.

## End-to-end testing

Large test suites can be structured to optimize ease of authoring and maintenance. Page object models are one such approach to structure your test suite.

Please read more about how to implement [page object models](https://playwright.dev/docs/pom) in Playwright.
