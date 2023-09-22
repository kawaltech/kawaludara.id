---
title: Core principles
description: We value best user experience over feature completeness.
---

We value best user experience over feature completeness. {% .lead %}

## What we strive for

### ✅ Performance

Our applications must be high-performant because our audience is spread across Indonesia with varying types of devices and network speed. For instance, a good measurement of web application performance is Google's [Core Web Vitals](https://web.dev/vitals/).

### ✅ Accessibility

Our applications must be accessible so that we can reach more users and help more people.

### ✅ Eventual consistency

Any information presented on our applications must be up-to-date to the latest version that we can provide. We can tolerate delays to a certain degree for the sake of application performance, but it should be limited to less than an hour.

### ✅ Iterative, incremental changes

Software development is **complex, cognitive work**. The simpler we can make something, then generally the easier it is to do. Similarly, the less amount of moving parts a software component has, the less prone it is to errors, and the less maintenance burden it gives us.

One of the simplest ways to reduce complexity is to reduce the scope. We can often postpone the less valuable parts of a large issue and do them later in order to get the most valuable parts into our user's hands faster.

## What we're going against

### ❌ Counter-productive cosmetics

We can't afford to hurt applications performance or to provide outdated information just for the sake of the beauty of the applications.

### ❌ Expensive functionalities

We must carefully consider any additional dependencies overhead on the website/applications. Unless its benefits outweigh the trade-off that we have to pay, we should avoid adding the functionality. Even if it is proven to be beneficial, we should strive to implement it in the best possible way. An excellent example of it is [Google Analytics](https://github.com/kawalcovid19/wargabantuwarga.com/issues/18).

### ❌ Unmeasured improvements

For any improvements on the applications, we should continuously measure its impact, for instance, using the [Core Web Vitals](https://web.dev/vitals/). If proven to hurt the metrics, we should revert the changes and find another way to implement them without degrading the performance.
