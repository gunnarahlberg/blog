---
layout: post
title: How 'Derive scope from Goal' helped my client to choose a non-technical solution
tags:
- agile
- articles
- Sbe
status: publish
type: post
published: true
meta:
  _edit_last: '1'
  _wp_old_slug: how-derive-scope-from-goal-saved-ten-thousand-dollars
---

{{ page.title }}
================

<p class="meta">Published {{ page.date | date : "%Y-%m-%d" }}</span> - Stockholm</p>

As developer, how do you save money for your client and at the same time ensure that you work on interesting and motivating stuff? Here's a tip. Chose to derive scope from a goal. When someone asks you to develop code without reason, say "I see this is important to you. Please, let me know why?"

My responsibility at my current client is to be team leader for a development team of eight developers, two testers, two customer experts. My customer proxy asked me for a new feature. "We have to have another type of user in the system" and the first thing I got was a rough sketch of what the user interface should look like.

<img src="/images/uploads/2011/06/simple_Page_1.png" alt="The sketchup" />

I totally understand why he glossed over the reasons to actually do this piece of software change and new requirement. He had already spent hours and hours with a production problem. It was truly waste and should be eliminated. However, the UI sketch did not transfer this. His sketch was interesting but I didn't get the why it was so important. For me, it transfer the understanding that this would take weeks to implement, would impact the security and permission aspect of the system. We have implemented two user roles with some pain. Another feature request like that was meant icebergs ahead. All manageable but feasible?

So, as this potentially was a mistake to implement without more thought, I asked him, "Could you please explain an example of what this will solve? Just to get my creativity going". What I wanted to know was - what is the Goal or Desired effect. Was every option for a non-technical solution tried? What about the FAQ? What about the customer support first line? Let me see the knowledge base customer service use. Is it updated? Is the knowledge base used? What does the user FAQ look like? Can that be used? Enter the effect map

After some discussion we got a couple of examples

<strong>Example</strong>
"A user may enter foo and the system does blah, which is confusing. A system administrator can view the same foo as the user and support the user same view as the user" - that is the new feature. Most information that the user enters is private to the user and not even the system administrator is allowed to view it by default. Ten minutes of discussion in front of a white board with two pens helped here. We agreed on a couple of examples that are problematic for the user in the current in-production version.

An amazing thing happened here, I asked the customer proxy, "If we look at these examples on the white board, could we agree on a desired effect or goal for the new function?" Another five more minutes and we had one sentence that described the new function. "To be able to understand whether the user acted foolishly in the system or is it a missing function?" That one sentence was written using all kind of trivial words, yet it captured the essence of that new role of the user in the system. Someone that is able to get the same view of the system as the user.

So, I asked, who can fix this? Interestingly, the proxy assumed I was talking about "who" as in what part of the software. So, we used the white board and spelled out "Customer phone support" and "FAQ", "Database administrator" and "third line support" and so on. Some very interesting details showed up here that were not technical, for example, the knowledge is maintained not by the support but by an email to an administrator of the knowledge.

I asked "Who is that administrator? Does she or he get tons of emails? "
and the answer baffled me, "She resigned last week" - wow! We agreed that a replacement should be the first priority if that was the only way to update the knowledge base.
<p style="text-align: center;"><a href="/images/uploads/2011/06/Goal-_Decide_if_user_behave_foolish_or_system_is_wr.gif"><img class="aligncenter size-large wp-image-73" title="Goal-_Decide_if_user_behave_foolish_or_system_is_wr" src="/images/uploads/2011/06/Goal-_Decide_if_user_behave_foolish_or_system_is_wr-1024x291.gif" alt="Effect map" width="1024" height="291" /></a></p>
<p style="text-align: center;">We tried a couple of other non-technical solutions and some possible solutions that wouldn't require software to be developed. Five minutes of more discussion and more people got excited and interested around our white board. It was fruitful, as it was a potential solution and we could review this and be certain it was not an option.</p>
So, this is all interesting, we got other part of the system documentation improved. However, have we addressed the issue and got to the desired goal? Can we decide if the user is behaving foolish or is something wrong? Not really, something is missing. So I said, "What if we ask the user to this and that, that we already have. (I'm not allowed to tell you what). We just leave this note in front of the user of specific things to do so we could help them. " That turned everything upside down. Problem solved, just make a few tests that it does not interfere with existing processes and that the user documentation is updated with a note that "If you get stuck, please follow these simple steps, and we will get back to you".

Some more discussion gave us that, if we just document this, problem solved! WHOA! That saved us so much trouble! I estimate that the initial sketch implementation by the customer proxy would take weeks or months to get right. Money that we saved by some spending half an hour in front of a white board. Simple questions.

Get me right here, I didn't make this saving. I just happened to know how to ask the right questions. The real heroes here is the bright and talented people that really tried hard to find a proper solution to my probes. Was there any non-technical solution available? What is the goal or desired effect? I didn't come up with that. I'm just a random guy who know how to ask questions. I let the customer to reason around these questions.

It is so often a developer team is asked to implement a feature that I made it into a pattern. By merely asking simple things like "Please, let me know why this is important" and then "Let me help you asses that every non-technical solution has been tried" really help. Sometimes you don't get to do mundane stuff. Sometimes you really have to, but then, at least you have a crisp and clear understanding why.

This is of course in itself not new. This is a facet of what is called "Derive Scope from Goal" and came to me by the excellent Gojko Adzic. You should try it too. What I'm seeing though is that it is somewhat delicate to ask the right questions. For example, you may get in a us/them situation or that some domain specific words may get custom without a user to validate them. As always in a creative process, it is a minefield. Carefully questioning can be delicate. I'll gladly help you or your client with that.

Send me an email - agile at gunnarahlberg.com - and let us see what can happen.
