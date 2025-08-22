---
layout: post
title: Single responsiblility principle(SRP) is not a good teaching tool
---

Single responsibility principle is not a good teaching tool.
It is vague. It is unfalsifiable. If the class meets this criteria
depends on outside perspectives of what the class does. It can
pass or fail the criteria simply by subtly changing mental models.

For example if a payment object should be responsible for 
all types of payments in a system then it passes even if 
handles every type of payment. You can then a payments should 
be seperate PayPal, Cards etc. Then it no longer does.

You can not objectivly say if passes by simple looking at the
code. It only works if everyone has a shared understanding of
the domain model.


