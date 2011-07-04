---
layout: article
title: "Contest Rundown: RSpec formatters"
---

In our [very first contest](http://codebrawl.com/rspec-formatters), we asked the contestants to build a formatter for the [RSpec](http://relishapp.com/rspec) testing library. We had some great entries.

First of all, congratulations to Iain, Thilko and Chad, for being the first ever to respectively take the first, second and third place! All of you did a great job, so let's go over all five entries for this week.

[Thilko Richter](http://codebrawl.com/users/blackhacker) was the first to get his entry in and he created a nice way to keep you motivated to get your spec suite green again. His FortuneFormatter fetches a [fortune](http://brenocon.com/fortune.cgi) and displays it in your terminal window when all of your tests pass.

The JumbledFormatter, by [Richard Norton](http://codebrawl.com/users/rwtnorton) jumbles the output of the documentation formatter, but keeps the first and last letter of every word in its place. It is raelly ssprurinig to see how lbiegle jlmeubd txet lkie this can raelly be!

[Sam Elliott](http://codebrawl.com/users/lenary) did two entries, the DragonFormatter and the BossFormatter, both based on RSpec's own [documentation formatter](http://). They're both very simple, but you'll surely find yourself smiling when you see their output. The DragonFormatter notifies you of any &ldquo;dragons&rdquo;, by outputting the &ldquo;HERE BE DRAGONS&rdquo;-message after finding pending specs. The BossFormatter simply adds &ldquo;LIKE A BOSS&rdquo; to any passing spec, adding some assertiveness to running your tests. Both are great and fun alternatives if you're getting bored of RSpec's documentation formatter.

YELLY!!!, by [Chad Humphries](http://codebrawl.com/users/spicycode) does exactly what the name implies and yells &rdquo;yes&ldquo;, &rdquo;no&ldquo; and &rdquo;meh&ldquo; for passing, failing and pending specs. It gets a bit yelly (pun intended) since it starts screaming after every spec, but it's a great way to find out if your specs are passing when you're in the other room to get another cup of coffee.

And last, but certainly not least, [Iain Hecker](http://codebrawl.com/users/iain) took first place with his SpecCoverage formatter, which allows you to use SimpleCov whenever you want, without having to put it in your `spec_helper.rb` file. It doesn't output anything, like you'd expect from a normal formatter, so you're going to have to use another one to see your test output. I've been using this one for a bit and it's great. I certainly hope Iain turns it into a gem, to make it easier to install.

Thanks to the contestants for participating and to everyone else for voting. Be sure to check out [this week's open contest](http://codebrawl.com) and if you wanted to join the RSpec formatters contest but weren't on time, keep an eye on our [feed](http://feeds.feedburner.com/codebrawl), since we might just do a round two very soon. Stay tuned!
