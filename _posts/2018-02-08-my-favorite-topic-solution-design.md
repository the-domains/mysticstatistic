---
inFeed: true
description: and the link between data maturity and solution design.
dateModified: '2018-02-11T20:02:37.087Z'
datePublished: '2018-02-11T20:02:37.920Z'
title: Data maturity modelling
author: []
publisher: {}
via: {}
hasPage: true
sourcePath: _posts/2018-02-08-my-favorite-topic-solution-design.md
starred: false
datePublishedOriginal: '2018-02-09T10:54:05.934Z'
url: data-maturity-modelling/index.html
_type: Article

---
<div id="fb-root"></div>
    <script>(function(d, s, id) {
      var js, fjs = d.getElementsByTagName(s)[0];
      if (d.getElementById(id)) return;
      js = d.createElement(s); js.id = id;
      js.src = 'https://connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v2.12&appId=685425478513623&autoLogAppEvents=1';
      fjs.parentNode.insertBefore(js, fjs);
    }(document, 'script', 'facebook-jssdk'));</script>

# Data maturity modelling

and the link between data maturity and solution design.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/666fcd64-d93c-4024-8012-5bf772c290a9.png)

Local government has many verticals, so many it may perhaps be the most diverse organisation you could work within. Even if you compare with some of the giant multi market orgs (for example, Tesco's who in banking, shopping, groceries, property etc). We have so many different types of services that approaching all of them at the same level of depth for a team even our size is a real challenge. It's impractical to take the 'narrow and deep' model, invest in one area and showcase it because the need for data and analytics is across the piece. Having said that, there can be a frustration of the broad and shallow approach doesn't address those services which are a little further up the maturity scale. And then there's the question of investment in time...

---

## What will you learn in this blog

You're going to hear me wax lyrical about aligning your investment in solution architecture to your data maturity model, that big cumbersome models are bad, agile is for the win and Kimball is old news.

The image below or a version of it is in my data strategy. I whap it out every time someone talks about forecasting, or stratification and note that strategic analytics is BUILT UPON advanced reporting, and that there are required foundations that need to be in place. Before we became a big team, there were teams at level 1 and teams that were maybe entering level 2\. Our primary push for the team is to get every service area to level 2, so that we have regular, automated reporting that has an outcomes based focus, delivered to the business to support a retrospective view of where they're going.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/f40e4ef0-2899-49b7-ad20-d5f70a61b876.png)

## Aligning development control to your audiences maturity.

One of the things I believe is that the pace data should be delivered to the business should be proportional to the criticality of the service; I might prioritise the delivery of data to a team responsible for emergency fostering over that of HR for example. At the same time, when a service is at or close to stage 0 on the scale above, there's no point putting rigorous controls on a product they'll consume because it's the first time they'll see it. It's likely the first time that service has been able to gauge the quality of their data, and importantly the gaps where the business process doesn't leave a data footprint. It's more of a "this is what I can see, and it ain't pretty" report. It's to inspire curiosity, to provide insight, and to encourage that service/customer to start to think a little differently about their data.

## The way it goes with Customers at Stage 0 - 1

For services or areas at stage 0 (or between 0 and 1) I'll happy produce 2 or 3 problem focussed PowerBI models; let's pretend we have an admin team responsible for the production of tea for the organisation - we are in Yorkshire and tea is our thing. They've hit me up, the chief exec is kicking off at the amount we're spending on tea and needs some help lickety split.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/6495644d-37a0-4eec-a7b2-b0056be419d9.png)

I like tea, so I prioritise a 2 week sprint window and play fast and loose with the user stories - "as a user I want to be able to see my activity and customer information that represents my service". I'd quite happily give them 3 models, independent of each other as a first pass; one for tea bag procurement, one for distribution activity one for complaints and compliments. They're completely independent, they might want to grow at different speeds; the tea bag procurement model needs more development because the organisation puts more weight on financial based risks. Importantly, the service area doesn't yet have an understanding of half of the data they're seeing on the product... they've been merrily tapping tea bag purchase orders into the finance systems for years but not really taken a whole picture view of their data and understood what they were drawing. At this stage the business are starting to query themselves... how do we define "1 tea bag, is that per 160 that come in a box?" or "it's showing that John Kelly is in a group of 'high tea consumers' at an average of 6 cups per day but that doesn't factor in he works from home 3 days and doesn't drink our tea bags those days". What I'm finding is customers who are seeing **AND ABLE TO INTERACT WITH** data for the first time are

* Surprised by the level of data quality
* Surprised by how much of their business process isn't recorded / recorded outside of their main technology, usually on spreadsheets. (I keep this spreadsheet because I don't trust that system)
* Surprised at some of the insights (or at least 1 insight) when exploring correlations in their data.

When all this is happening, you already know you haven't got the right amount of metadata to start building a more comprehensive model. The business is asking these models TONS of questions, slicing and dicing with wild abandon to understand any correlates they care about. We're in 'observatory mode' where the service is testing what's possible. This exploration moves us into Stage 1; so now my teabag team know where to get that data from, when asked, and can respond to the chief exec and detail exactly how many tea bags are being bought, and comfort him that he's drinking an average amount of cups of tea. I'm not sure why in this fictitious scenario he cares, but he does.

## Stage 2... that brave world.

> Or really, where everyone expects every organisation should AT LEAST be at.

![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/20a71927-f7cb-4024-b077-83d4e6223c2b.png)

Stage 2 for the customer is about control and confidence. Let's fast forward say, 6 months. The teabag people are now quite happy, they've got a relationship with the chief exec, they give him a discount and learnt how to keep his questions to a minimum. However, they're setting themselves some performance targets... they run their model on volume not service, so they want to charge higher demand customers more. We need to start building a model with more control; we're starting to combine the view of assets driven by the business not just dictated by IT. We'll design a model that allows them to meet their outcomes - I say that a lot, because it's important for the service to be able to articulate and understand the relationship between the outcome they want to achieve and the outputs they need to do that. So, we'll now start to build a tea bag model; it's got data in from finance, we're gluing together customer from the finance system to the corporate complaints data, and activity information. I'll start from scratch using learning from the 3 models before but the result is now definitive. It's a single, one stop shop for tea bag team activity and performance. A T-Stop, if you will.

The specification sitting behind it is now more detailed, and complete. I'm defining measures such as "\# of Customers with an average overhead more than 1 deviation from the norm" instead of "show me the number of customers". Outputs are becoming more defined, not only descriptive in what the field represents, but with more metadata about how that data ends up there, and it's lineage - where that data came from. There's more of an interactive dialogue about presentation; now we want bandings of customer, and trends of the average cost. I want top 25 customers in regard to admin overhead so we can warn them they're going to be charged a premium for being a whinge bag. There's schedules in place to automate output, maybe even some triggers when target thresholds are set. We might even start tickling up the idea of the product being used to underpin tea bag administrator performance; highlighting team members that are slow pourers and those so fast they're a risk of scolding people.

Importantly now this model is locked down. It might still be a powerbi model but it might be a tabular model, it depends on how many users it has, and permissions/security. If others want to see tea bag data in their reports - let's just say a public health paper announced tea drinking had a correlation to productivity - we'd use this model as a source for other models to consume. It's the bonafide tea bag model, there won't be another, it is the source of truth within the organisation. The tea bag team now have adequate data quality controls in place to be confident in this being the single source of truth. The may even have a data steward.

### What's the alternative to this pragmatic delivery approach?

What I've seen in other local authorities and businesses is frankly madness, and in my mind, Kimball has a lot to answer for. IT have taken a lead, they've read Kimball's books, and armed with a waterfall style project management approach they've analysed the hell out of tea bag team at reasonable disruption. They've then built designed and an ETL strategy with often far too many slowly changing dimensions on data attributes that were deemed 'dynamic' - regardless of whether that's operationally important or not. They'll go through a lengthy build process, and then roll out to the business, and step away. The business model might have moved on, their operation has changed - the measures aren't reflective of new targets, and the change process is considerable because IT have moved onto something else.

The model is big, and cumbersome, and lumbering. It's technical... it expects too much of the customer and doesn't encourage or support that cultural journey that you need to bring your customers on to. It's usually 5-10 times longer than an agile delivery of a model, and despite being comprehensively documented and tested, its ability to flex is a con that negates the pro's. What's criminal is I still hear of these being the first step for providing intelligence to a customer.

## Agile or Waterfall

Ok so I guess I am really replaying the difference between agile and waterfall, but it's more than that really, it's the implication of agile in solution design. You could take an agile approach to a more traditional Data warehousing solution (Stage \> ETL \> DW \> OLAP Model \> Reports), but I don't think that responsive to customer maturity and I don't think that's responsible in terms of development pace. Your customers might already have a good view of data, and be starting from a more mature position but often they're not. And let's be honest, technology, disparate data sources and converging solutions all play a role. I provided an example of the tea bag company understanding where it's data was coming from, but often in a more complex business area, business process can be spread across 10 or more core technologies, with gaps being filled with ad-hoc excel, access and lord knows what cloud based joys.

## Stage 3 - Dare we dream?

We dare! We're planning for it mass market too. For me though stage 3 demands some givens. That we know completely our current state of data quality, and that we have proper and robust mechanisms for controlling quality - for example Master Data Management processes. We're currently designing a Single View of a Child and this is going to form a central way or demonstrating who a child is, and what event's we know about. For that, we're going full fat, traditional source to stage, shape, then through an ETL and MDM process, land in a DW as a record of fact. Everything is properly defined, processed, and rule based. Lineage and audit are baked in, it's all contained. And that design is the product of a process with the business, that they've engaged with, that they recognise the value of.

## Stage 4 - Predictive Analytics

This is stage is a misnomer in that it doesn't really follow the architecture model... you can absolutely perform predictive analytics to varying degrees of success at any stage of the maturity model, but obviously it works best if you have cleaned and described data. If for example, you want to predict the likely growth of blue badge applications, or you want to design a machine learning process that can be used as a decision support system, it needs clean data to run that from. It's unlikely but entirely possible that the tea bag company, having sat using spreadsheets and never really understanding their business are going to knock on the door and ask for a customer demand risk stratification model that they might consider when accepting new subscriptions - because it requires a level of maturity that you really need to grow. Similarly, you might get Bill Buzzword who has read an internet article and wants to start using these techniques to better anticipate where potholes are going to be. I mean, that's admirable, and actually very exciting - but if we've got huge gaps in accuracy around road condition, then our working data is flawed and our model is going to be flawed too.

We're starting to dabble here, we've run a few experiments and had some successes, we've got some interesting case study material too.

## Stage 5 - Prescriptive

I think if you're able to do stage 4, then stage 5 isn't a data gap it's a skills gap, and maybe some other non technology gaps (ethical, legislative, political). If you're data is mature to the point you can use it to confidently predict with... you're able to prescribe. There's work on the cards to be in here, and to pilot some prescriptive decision support work that uses history to better recommend next actions. Will our organisation get to the point where we can automate these decisions? I hope so... but I recognise the need to more thoroughly work through some of the softer barriers.

## Data Architecture

There's questions that need to be answered in another blog, this is big enough - around the way we grow up models from a ten minute "something I crapped up for you" to a solid, load balanced 26gb tabular model. There are decisions we make about the levels we'll aggregate smaller models into bigger ones as a service matures. We do have an approach, it's not super rigid but it's worth discussing perhaps in a future blog.

## What have you learned

Hopefully that you should never go big bang, and that your solution design and investment in approach should align to the risk of your customers' needs changing - something that's absolutely impacted by their maturity. That building production ready, mass consumption mini models is completely appropriate, as is cross referencing those - and that your design methodology should become more robust alongside the needs of the business. Agility is key - if you can't deliver at the speed of the demand your customers will go elsewhere, presume it can't be done and create something themselves which is uncontrolled and on unknown technology. A worse risk, you'll build something that is unable to flex at the pace of the business and ultimately turn off the business and represent a waste of development.

PEACE!

    <div class="fb-comments" data-href="http://mysticstatistic.com/" data-numposts="5"></div>