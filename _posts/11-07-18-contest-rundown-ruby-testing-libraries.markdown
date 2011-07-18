---
layout: article
title: "Contest rundown: Ruby testing libraries"
---

After challenging you to create a simple Ruby testing library, we got six very interesting entries. First of all, congratulations to Peter, James and Josep for taking this week's first, second and third place. Because all entries were great this week, we'll briefly go over all of them.

### #1: Peter Cooper

This week's [winning entry](http://codebrawl.com/contests/ruby-testing-libraries#peterc), by [Peter Cooper](http://codebrawl.com/users/peterc), uses a unique way of writing specs. The `README` states "If `=>` in a hash is a "hash rocket", then `+->` and `-->` for tests should be "test rockets"!", which means you write your tests like this:

    +-> { block that should succeed }
    --> { block that should fail }

This makes the specs extremely tiny, allowing you to quickly test small libraries. The library's code fits in a tweet, but Peter also included the extended version -- which is still only seven lines -- to make the code a bit more readable. A very unique entry.

### #2: James Urquhart

[Detective](http://codebrawl.com/contests/ruby-testing-libraries#jamesu), by [James Urquhart](http://codebrawl.com/users/jamesu), took second place this week. Instead of testing code itself, it instructs the user to do things and asks questions. A Detective test can look something like this:

    describe "Cool feature" do
      instruct("We will be testing this cool feature")
      it "should show the correct word" do
        instruct("Go to coolwebapp.com")
        ask("What does it say in the middle of the front page?").expect("Cheezburger")
      end
    end

As you can see, Detective comes with `describe` and `it` blocks, and is a very complete testing library. I love the idea of using human input to do testing. Another idea: hook it up to Amazon's [Mechanical Turk](https://www.mturk.com)!

### #3: Josep Bach

[Josep Bach](http://codebrawl.com/users/txus) took the bronze with his [tiny library named "a"](http://codebrawl.com/contests/ruby-testing-libraries#txus). Inspired by [almost-sinatra](https://github.com/rkh/almost-sinatra), "a" is just 7 lines long (with less than 80 characters per line), but has a lot of great features for its size. For example, it can do setup and teardown, remember at which line failures occur and proper reporting after the suite has finished. The assertions are done -- like you'd expect -- with the `a` method.

Josep already turned his entry into a proper gem (`gem install a-gem`) with a [Github repository](https://github.com/txus/a), which is even shorter than his entry already. With only 6 lines of code, "a"'s long-term purpose is to become the fastest testing framework available.

### #4: Will Leinweber

[Will Leinweber](http://codebrawl.com/users/will) was back again this week, taking fourth place with [Classy](http://codebrawl.com/contests/ruby-testing-libraries#will). "Classy is simple. No setup or descriptions, just equality". Will focussed on having tiny specs, without describe blocks or setups allowing you two write assertions as simple as this:

    str = Classy "ruby string"
    str.size == 11

Again, quite complete for its size, reporting failures and the amount of time it took to run the suite. The library is small and the code is clean. Once again, a solid entry.

### #5: Benedikt Müller

[Benedikt Müller](http://codebrawl.com/users/linopolus) created [SupiSpec](http://codebrawl.com/contests/ruby-testing-libraries#linopolus) and took fifth place. Like Will's entry, it doesn't use assertions as it checks for the return value of the `it` blocks:

    describe 'My Application' do
      describe 'Hello World' do
        it 'should be true' do
          'hello' != 'world'
        end
      end
    end

Complete with `describe` blocks, it prints out the spec descriptions in red or green, giving you instant documentation.

### #6: Viktar Basharymau

[assert_tomorrow](http://codebrawl.com/contests/ruby-testing-libraries#DNNX), by [Viktar Basharymau](http://codebrawl.com/users/DNNX), is a one-line testing "framework" that allows you to test things that should happen tomorrow. Instead of cheating and inventing a time machine, Viktar's entry actually `sleep`s for 24 hours before running the assertion. Awesome entry, it certainly made me laugh.

Special thanks to the contestants and voters, this contest had some great results. I certainly hope these projects stay in development, there are some clever ideas in there. Don't forget to check out our [next contest](http://codebrawl.com/contests/terminal-admin), in which we'll be creating a database admin in the terminal.


