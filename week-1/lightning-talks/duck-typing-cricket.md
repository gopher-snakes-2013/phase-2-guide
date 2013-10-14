#Duck Typing 

* Facilitates your class to be used in ways you didn't anticipate when you wrote it.

* Limit the dependencies between classes.

*ex: 
```
class HoneyBadger  
  def smack(duck)
     duck.feathers? 
     duck.quacks
     p 'smack!'
  end

end

class Duck
  def feathers?
  end

  def quacks
  end

end

class Squirrel
  def feathers?
  end

  def quacks
  end

end

-----Driver Code-----

h=HoneyBadger.new
d=Duck.new
s=Squirrel.new

h.smack(d)
h.smack(s)

```

* You can call smack on anything that quacks so this reduces dependency. 

* Don't hardcode external classes inside a class that you are writing. 

* Ruby is dynamically typed so it provides Duck Typing 