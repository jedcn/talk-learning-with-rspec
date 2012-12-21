# Talk: Learning With RSpec

## Overview

This talk is part of a series focused on **Learning**.

The two basic ideas behind the **Learning Series** are:

1. As knowledge workers, **Learning** is fundamental to both our day-to-day
   happiness and our long-term happiness with our career. It is enjoyable! And
   it is probably why we're knowledge workers in the first place.

2. The better we get at **Learning** the happier we will become.

The core ideas behind this talk, **Learning ..with RSpec** are:

1. If you look at this 'BDD' tool in the right light, it is something that helps
   us explore new technology and better retain and reference what we've found.

2. RSpec can serve be written to capture well-written, self-executing notes on
   books, podcasts, languages, apis, etc.

3. The R in RSpec is probably linked to Ruby, but any testing framework could
   allow for the same thing. This is not limited to Ruby or RSpec. For example,
   Jasmine and JavaScript.

## Intro to RSpec

For our purposes, the most important aspects of RSpec are:

* It emphasizes the creation of easy-to-read specs

* It emphasizes building specs that produce easy-to-read output

* You can "run" an entire suite of files or just a single pieces of a file.

I am intentionally ignoring the BDD aspect of RSpec. That might be why the tool
was created, but it is not what we're focused on today.

## Metaprogramming Ruby

As I started reading
[this book](http://pragprog.com/book/ppmetr/metaprogramming-ruby), I recall a
footnote indicating that I should exercise and explore the core concepts of the
book via IRB.

I did this, but, when life interrupted, and I couldn't get back to the book for
a week, I found that I had completely lost context.

In searching for something more permanent, I thought about TestUnit and then
ultimately converted to RSpec (for readability).

As I continued on with RSpec, I realized I was writing a group of specs that
were describing not a specific piece of software, but instead, "What Jed knows
about the book Metaprogramming Ruby."

Writing specs definitely slowed down my progress through the book. This isn't
just because it takes longer to write things out, but because it's not always
straight forward *how* to write a spec for some of these concepts.

As an example, consider how self changes throughout this code:

```ruby
# What is self?
module SomeModule
  # What is self?
  class SomeClass
    # What is self?
    def some_method
      # What is self?
    end
  end
end
```

How would you write a spec for that?

It takes some thinking if you're just starting out.

But.. if you can figure it out, you're better off for it.

And if you figure it out in a spec that you commit somewhere, you've got a
easily indexed, self-executing set of notes that can easily be shared with a
friend.

## GIT + GRIT

While I'm still relatively new to git, I've found a great way to "work through"
Git internals is to consider a library like
[Grit](https://github.com/mojombo/grit), which provides Ruby bindings to Git.

As an example, the
[learning-ruby project](https://github.com/jedcn/learning-ruby) has a spec that
uses grit to examine itself. Commits, Trees, Blobs,.. they all come to life when
you sit down and write up a spec for how you think they should work.

This has really made the Git Internals section of Scott Chacon's
[Git Internals](https://peepcode.com/products/git-internals-pdf) or his
[Pro Git](http://git-scm.com/book) much more concrete for me.

## Jasmine and JavaScript

What if you're not a Rubyist? No problem. These concepts apply to any language
that has something similar to RSpec or even TestUnit.

Jasmine's [main page](http://pivotal.github.com/jasmine/) introduces Jasmine
using Jasmine, and that's right along the same lines of capturing notes on
'Metaprogramming Ruby' in RSpec.

## In Closing

If you get comfortable readying RSpec/Jasmine, then it reads almost as well as
regular documentation.

It's not always straight forward to write notes in RSpec, but your effort will
pay off when you can start describing more complex topics.

You can write a spec about almost anything that you could take notes on:

* Reading a book
* New parts of a language
* A podcast
* A conference talk
* An API
