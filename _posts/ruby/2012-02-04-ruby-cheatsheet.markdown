---
categories: ruby
---

## Simple types and constructs
    
    # This is a comment. Comments start with a '#'
    
    # Simple arithmetic - follows BODMAS rules
    3 * (2 + 1) / 4.0 - 1
    
    # Variables and assignment
    x = 10 / 2
    variables_must_start_with_lowercase_letter = "a"
    aVariableWithUpperCase = 100
    
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
    "The total is #{calculated_grand_total}"  
    
    # Arrays
    [1, 2, 4, "something different to a number", an_object]
    
    # Hash
    {:name => "Bob", :email => "bob@smith.com", 
      :address => {:street => "1 dobber St", :city => "Melbourne"}
    }
    

## Methods

    def method_name(variable_one, variable_with_default_param = 10)
      # do something
      result = variable_one + variable_with_default_param
      
      # last line of a method is the return value of the method
      result
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
    launch_missiles unless already_winning
    

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
    
    # Including the module in a class means the methods are added to the class
    class SomeClass
      include MyModule
    end
    
    obj = SomeClass.new
    obj.my_module_function1
      