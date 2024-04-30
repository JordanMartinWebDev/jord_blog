---
thumbnail: 'src/lib/assets/Full Logo.svg'
title: Just Because We Can, Doesn't Mean We Should
description: Just discussion on the ethics of software features.
date: '4/30/2024'
categories:
  - 'programming'
  - 'practical advise'
---

# Just Because We Can, Doesn't Mean We Should

## **We Are Capable**

Much of the world today is run on software. Schools, healthcare, business, etc. all have specialized software that we, as engineers, develop and maintain. However, recent experiences have me wondering if all software features are "good." And I don't mean quality. I mean what is the effect we are having on society with our features that at first seem mundane.

I'd like to discuss 2 examples I witnessed recently, where the features of an application seem harmless and "like a good idea", but end up having effects that could be **dangerous**. Not because of the software itself, but because of the people using the software and the percieved permission we are giving to users of acceptable behavior.

## **The Call Center**

### The Feature

Nothing is more mundane than call center work. Read emails, answer calls, solve some issues, put in tickets. Day in and day out. While we can't change the job itself, as engineers, we can make the software easier for our users.

One day you get a feature request. The call center staff wants a way to message the clients updates on their tickets. That makes sense. So you get to work. Couple of days later, you launch a feature to email the customer through the ticket software, and the customer can easily respond back through email and it logs into the ticket. **Beautiful**. Job well done.

Fast forward a couple weeks and the call center staff are loving the new feature. It's saved them time not having to call customers for every little update, and the customer is happy because they get updated more often. BIG WIN!!!

### The Problem

Uh oh...our main application, for our largest client, is seeing some outage problems. Tickets are rolling into the call center and we need to know exactly what's going on. This is mission critical. Every second we are down is millions lost. We need to know **exactly** what's going on.

You reach out to Tier 1, "Contact the client and see exactly what they are experiencing." While you wait for that info, you go off to check deployments, servers, etc.

...it's been a while. What's taking so long? Why have I not heard back from Tier 1? I need to know exactly what our users are experiencing in detail. "Hey, what did the client say?"

**"Well, they haven't emailed me back yet."**

### What did we do?

One can argue we didn't **do** anything. But I'm here to argue the opposite. By developing this feature for the ticket system, we authorized the call center staff to email customers. It's a valid form of communication...but not during a crisis! Our call staff should have reached out to the client by phone.

You may be thinking. "Well that's obvious! This is a problem with that staff member." First, we know as developers, what's obvious to us isn't always obvious to others. Second, we made the feature. We didn't consider a policy needed for mission critical outages...and now we running at the speed of email.

We did not consider that the ease of sending an email off would change the operating procedure. Why would it? Well because people will often take the path with the least resistance. Do you want to call a customer who's system is out of order and is losing major money in operating costs? Neither does the call center employee. So, they send off an email to avoid confrontation.

It's natural, and we authorized it indirectly.

To add some nuance here, I don't think the feature here is neccessarily the problem. It's how people use the feature that is. But what could we have done to prevent this? Tickets with a priority of high or critical have the "email through ticket" feature disabled. Or upon feature release, a notice sent to the call center supervisor to implement a policy for mission critical moments. There are things we can do to still deliver this feature, but mitigate the damages.

## The Appointment

### The Feature

Hospital and doctor staff have some of the toughest jobs on earth. They are consistently dealing with patients at their worst, they are overworked, and their job is intense. Again, we can't change the job, but we can assist with software.

You get a feature request for a notification system within the hospitals app. They would like the patient to be notified if anything changes with their account. New medicines, new appointments, etc. You get the idea. Great feature. Let's get to it.

Fast forward and it's done. Users now get push notifications from the hospital app when something with their account changes. The hospital is happy and the users of the app are happy too.

## The Problem

In some professions, you don't get many days off, even for a doctor's appointments. But you have to get your eyes looked at. It's getting dangerous to operate the heavy machinery for your job, while you're barely able to see. You schedule a doctor's appointment in advance and plan a day off work that's much needed.

Four days later, you show up to the hospital for your appointment, but you're stopped at the front desk. "We're sorry sir, **we moved your appointment**. You should have been notified via the app two days ago. We scheduled you a new appointment 3 weeks from now."

I would like to say this is a rare occurence...sadly it's not. Now you have missed a days wages, still have poor eyesight, and you have figure out something called an "app" to get an appointment with your doctor.

## What did we do?

In a similar vein as the first story, we have a breakdown in communication. Our nurse or office staff didn't communicate effectively to the patient, and now there is a problem. "Well it's not our fault the office person didn't call." You're correct, but as we discussed hospital staff are often overworked. They could have thought our new notification system would take care of this for them.

We also made an assumption. The assumption was everyone used the hospital app. What about the older population who barely know how to use the internet? What about the blue collar people who prefer to do things the "ole fashion way." What about the people who don't go to the doctor often and weren't even aware of an app or have push notifications off? Do we have a right to force them to use our application or else they don't get informed about things concerning their health?

What could we have done? We can continue with the push notification deployment, but also deploy a text message system and an automated phone call system. We also need to inform the doctor/hospital staff that push notifications are only effective if the person is using the app, and has push notifications on. A phone call will still be nesseccary for important time sensitive changes.

## **Conclusion**

As we make software to improve the lives of our users, something I think we often forget to consider is the human side effects those features can cause. In a world where people would rather text or email than call someone, situations like this can often occur. It's not something we nesseccarily did "wrong", but something we didn't consider when developing the feature. Both features seem harmless at first, until the right situation arrives.

Both my examples revolve around communication with clients, but what other side effects of human nature could we be ignoring? Addiction to apps, like social media? Bullying, enhanced by new anonymous features? Increased social awkwardness, because of through screen communication?

There is an entire world of issues our software can bring to light, and while I'm not argueing we are responsible for all of the world's problems...do we even take them into account? Or are we just being code monkeys who push out features without considering how we as humans might interact with it? I don't have the answer to this, and I need to go...new feature request just came in.
