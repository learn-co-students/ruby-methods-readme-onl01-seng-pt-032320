Let's try making a method we can use over and over. Make a new file called
`greeting.rb` (you can use: `touch greeting.rb` from your terminal). Put the
following code in it:

File: `greeting.rb`

```ruby
def greeting
  puts "Hello World"
end
```

Save your file and run it with `ruby greeting.rb`. You'll see:

```bash
$ ruby greeting.rb
$
```

You'll notice that when you run your program, nothing happens. Your program
successfully defined the method but it never executed it. Just because you built
a machine doesn't mean that you turned it on. Update your `greeting.rb` to
entirely read:

File: `greeting.rb`

```ruby
def greeting
  puts "Hello World"
end

greeting
```

Save your file and run it with `ruby greeting.rb`. You'll see:

```bash
$ ruby greeting.rb
Hello World
$
```

Now your program actually executed the program. Update the code again to
entirely read:

File: `greeting.rb`

```ruby
def greeting
  puts "Hello World"
end

greeting
greeting
greeting
greeting
greeting
```

Save your file and run it with `ruby greeting.rb`. You'll see:

```bash
$ ruby greeting.rb
Hello World
Hello World
Hello World
Hello World
Hello World
$
```

The bareword `greeting` will execute the body of the defined method.

#### Writing Code vs Reading About Code

Programmers love conventions, or agreed upon rules that help them talk to each
other about code. A common syntax convention for Ruby methods is to preface them
with a `#`, and in subsequent lessons, you might see methods written with a `#`
in front of the method name. For example, if a method is named 'greeting',
rubyists will often refer to it as `#greeting`. This is so that other rubyists
can instantly recognize it as a method, as opposed to a variable or a bareword
or a class.  But remember that when you write it in your code, it should be
`greeting` and not `#greeting`.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/ruby-methods-readme' title='Methods in Ruby'>Methods in Ruby</a> on Learn.co and start learning to code for free.</p>
