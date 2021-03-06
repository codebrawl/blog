---
layout: article
title: "Contest rundown: RSpec formatters"
---

In our [very first contest](http://codebrawl.com/contests/rspec-formatters), we asked the contestants to build a formatter for the [RSpec](http://relishapp.com/rspec) testing library. First of all, congratulations to Iain, Thilko and Chad, for being the first ever to respectively take the first, second and third place! All of you did a great job, so let's go over all five entries for this week.

[Thilko Richter](http://codebrawl.com/users/blackhacker) was the first to get his entry in and he created a nice way to keep you motivated to get your spec suite green again. His [FortuneFormatter](http://codebrawl.com/contests/rspec-formatters#blackhacker) fetches a [fortune](http://brenocon.com/fortune.cgi) and displays it in your terminal window when all of your tests pass.

The [JumbledFormatter](http://codebrawl.com/contests/rspec-formatters#rwtnorton), by [Richard Norton](http://codebrawl.com/users/rwtnorton) jumbles the output of the RSpec's own [documentation formatter](https://github.com/rspec/rspec-core/blob/master/lib/rspec/core/formatters/documentation_formatter.rb), but keeps the first and last letter of every word in its place. It is raelly ssprurinig to see how lbiegle jlmeubd txet lkie this can raelly be!

[Sam Elliott](http://codebrawl.com/users/lenary) did two entries, the [DragonFormatter and the BossFormatter](http://codebrawl.com/contests/rspec-formatters#lenary), both based on the documentation formatter. They're both very simple, but you'll surely find yourself smiling when you see their output. The DragonFormatter notifies you of any &ldquo;dragons&rdquo;, by outputting the &ldquo;HERE BE DRAGONS&rdquo;-message after finding pending specs. The BossFormatter simply adds &ldquo;LIKE A BOSS&rdquo; to any passing spec, adding some assertiveness to running your tests. Both are great and fun alternatives if you're getting bored of RSpec's documentation formatter.

[YELLY!!!](http://codebrawl.com/contests/rspec-formatters#spicycode), by [Chad Humphries](http://codebrawl.com/users/spicycode) does exactly what the name implies and yells &rdquo;yes&ldquo;, &rdquo;no&ldquo; and &rdquo;meh&ldquo; for passing, failing and pending specs. It gets a bit yelly (pun intended) since it starts screaming after every spec, but it's a great way to find out if your specs are passing when you're in the other room to get another cup of coffee.

And last, but certainly not least, [Iain Hecker](http://codebrawl.com/users/iain) took first place with his [SpecCoverage formatter](http://codebrawl.com/contests/rspec-formatters#iain), which allows you to use SimpleCov whenever you want, without having to put it in your `spec_helper.rb` file. It doesn't output anything like you'd expect from a normal formatter, so you're going to have to use another one to see your test output. I've been using this one for a bit and it's great. Iain even turned it into a [RubyGem](https://rubygems.org/gems/spec_coverage) and gave it a proper [repository](https://github.com/iain/spec_coverage) to continue working on it.

Thanks to the contestants for participating and to everyone else for voting. Be sure to check out [this week's open contest](http://codebrawl.com) and if you wanted to join the RSpec formatters contest but weren't on time, keep an eye on our [feed](http://feeds.feedburner.com/codebrawl), since we might just do a round two very soon. Stay tuned!
