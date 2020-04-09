#Looping vs Iteration

#looping
#7.times do 
#puts "Stop hitting yourself!"
#end

#Using "while" construct
#input = ""
#while input != "Mommmm!!"
#puts "Stop hitting yourself!"
#input = gets.chomp
#end
  
#brothers = ["Tom", "Tim", "Jim"]
  
#count = 0
#while count <= brothers.length - 1 
#puts "Stop hitting yourself #{brothers[count]}!"
#   count += 1 
#end

#primary_colors = ["Red", "Yellow", "Blue"]

#primary_colors.each do |color|
#  puts "Primary Color #{color} is #{color.length} letters long."
#  end

#primary_colors = ["Red", "Yellow", "Blue"]
#primary_colors.each do |color| # do begins a block
#The lines between the do/end are the block's body
#  puts "Primary Color #{color} is #{color.length} letters long."
#  end # end terminates the block 

#require 'pry'

#def hi_there(name)
#  puts "Hi, #{name}"
#  binding.pry
#end

#hi_there("Sophie") # > "Hi, Sophie"
# => nil

#brothers = ["Tim", "Tom", "Jim"]
#brothers.each do |hippo|
#binding.pry 
#  puts "Stop hitting yourself #{hippo}!"
#end

###all?###The rule for "all" is that every iteration, every loop of the block must return true.

#all_odd =  true 
#[1, 2, 3].each do |number|
#  if number.even? #Will evaluate to false for 1, true for 2, false for 3
#  all_odd = false
#  end
#end
#all_odd #=> false

#all_odd = [1, 3].all? do |number|
#number.odd? #Will evaluate to true for 1, true for 3
#end #=> true
#all_odd #=> true  

#all_odd = [1, 2, 3].all? do |number|
#number.odd? #Will evaluate to true for 1, false for 2, true for 3
#end #=> false
#all_odd #=> false

###none?###Opposite of "all"

#[1, 3].none?{|i| i.even?} #=> true

#none_even = true 
#[1, 3].each do |i|
#  if i.even?
#    none_even = false
#  end
#end #=> [1, 3] because #each always returns the original collection
#none_even #=> true

###any?### 
#[1, 2, 100].any? {|i| i > 99} #=> true 

###include?###
#the_numbers = [4, 8, 15, 16, 23, 42]
#the_numbers.include?(42) #=> true
#the_numbers.include?(6) #=> false

###sort vs sort!###
#require 'pry'
#arr = ["d", "a", "e", "c", "b"]

#arr.sort

#binding.pry

#





  