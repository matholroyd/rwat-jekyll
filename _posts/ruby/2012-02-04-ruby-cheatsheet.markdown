---
categories: ruby
---

## Simple types and constructs
    
    # This is a comment. Comments start with a '#'
    
    # Simple arithmetic - follows BODMAS rules
    3 * (2 + 1) / 4.0 - 1
    
    # Variables and assignment. Variables should start with lower case letter
    x = 10 / 2
    grand_total = 0 
    grand_total += 10
    
    # Constants start with a capital letter
    DomainName = "www.tworgy.com"

    # Symbols. Somewhat unique to Ruby, often used in hashes. Should start
    # with lowercase letter, can contain underscores
    :a_symbol
    :name

    # Strings
    'This is a string'
    "This is also a string"

    # For inline string sustitution, use string with " double quotes and #{ }
    "The total is #{grand_total}"  
    
    # Arrays
    [1, 2, 4, "something different to a number", an_object]
    
    # Hash
    {:name => "Bob", :email => "bob@smith.com", 
      :address => {:street => "1 dobber St", :city => "Melbourne"}
    }
    
    # Comparisons
    1 > 2
    1 >= 2
    2 < 3
    2 <= 3
    1 == 2
    1 != 2
    "quick brown fox" =~ /jumped over/
    

## Methods

    def method_name(variable_one, variable_with_default_param = 10)
      # do something
      result = variable_one + variable_with_default_param
      
      # last line of a method is the return value of the method
      result
    end
    
    # methods end with a ? or a !
    def fire_the_missiles!
    end
    
    def alive?
    end
    
    # Calling the function, passing variables 10 and 2.5
    # Can leave out paratheses
    method_name(10, 2.5)
    method_name 10, 2.5
    method_name 10     # Using the default paramter
    
    # Saving the result of a method
    num = method_name 10, 2.5

## Control structures

    if a == 3
      # do something
    elsif a == 5
      # do something
    else
      # do something
    end
    
    unless b == "cow"
      # do something
    end
    
    launch_missiles if under_attack
    launch_nuclear_missiles unless already_winning
    
## Enumerator methods
  
    # Objects that are lists of items (like Arrays) typically implement the 
    # Enumerator mixin, meaning they have a bunch of methods to help processing 
    # their data. The most commonly used methods are...

    # each
    missles.each {|missle| fire(missle) }

    # collect/map
    names = people.collect {|person| person.name }
    names = people.map     {|person| person.name }  # same as collect
    
    # select/filter, reject
    girls = people.select {|person| person.gender == :female }
    girls = people.filter {|person| person.gender == :female } # same as select
    candidates = people.reject {|person| person.hair_color == :blonde}
    
    # inject - used to aggregate over a list
    total = accounts.inject(0) { |sum, account| sum += account }
    
    # detect/find
    suspects.detect {|person| person.name == "Jack the ripper"} # the first match, or nil
    suspects.find   {|person| person.name == "Jack the ripper"} # same as detect
    

## Classes

    class MyAwesomeClass
      @my_instance_variable = 10
      @@my_class_variable = 20
    
      def regular_instance_method
      end
      
      def self.class_method
      end
    end
    
    MyAwesomeClass.class_method
    obj = MyAwesomeClass.new
    obj.regular_instance_method

## Modules

    module MyModule
      def my_module_function1
        # do something
      end
      
      def my_module_function2
        # do something
      end
    end
    
    # Including the module in a class means the methods are added to the class as
    # instance methods
    class SomeClass
      include MyModule
    end
    
    obj = SomeClass.new
    obj.my_module_function1
      