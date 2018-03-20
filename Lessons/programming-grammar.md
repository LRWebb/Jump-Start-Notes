# Lesson 9: Programming Grammar

[Link to Ada Academy lesson 9](https://github.com/Ada-Developers-Academy/jump-start/tree/master/learning-to-code/grammar)

Text in bold from lesson plan 

## Activities:
:heavy_check_mark: Review notes within this section  
:heavy_check_mark: Watch [Video: Values, Variables, Commands and Comments](https://vimeo.com/channels/1001988)  
:heavy_check_mark: Complete the [practice problems](./practice-problems.md) and then check your answers using `irb`  
:heavy_check_mark:  Write a madlibs program  
  :heavy_check_mark: First play a few on [eduplace](https://www.eduplace.com/tales/) to become familiar with the game  
  :heavy_check_mark: Create a MadLib program that accepts input from the user and outputs a completed MadLib  
  :heavy_check_mark: Use up to ten different parts of speech in order to fill in your MadLib  
  :heavy_check_mark: Output should consist of a paragraph of output that has the user’s input substituted into the MadLib, we have provided an example run, but your madlib program should be unique to you  

## Notes:
Gist using Atom and Linux:  
Experimenting and reading online, I found that Ctrl+Alt+G is what makes a Gist in Atom on Linux. Did that to start the Gist of essay answers.   
Ctrl+Shift+G in Atom brings up the style guide!  
Also learned I need to have a file open in Atom with text before a Gist can be made of it  

https://gist.github.com/730fe708fbdea083056267ac877876ab

New to me- float, symbol, hash  

There is an order of operations in Ruby  

Assignment statements are read from right-to-left, not from left-to-right. Use phrases like assigns, or stores the value, instead of equals, or equal to.  

Compound assignment statements look very cool- also potentially confusing, but cool that actions can be combined  

Chomp!  

I’m going to have to read this more than once  

Slice sounds cool  

Video- instructor recommends we watch this twice  

## Practice Problems:  
### Variables and assignment practice:  
Complete each section by hand, then check your answers using irb  

x = 5  
what value does x now hold?  
5  
irb says 5!  
  
z = "Hello"  
what value does z now hold?  
Hello  
irb says Hello!  
  
a = 5  
b = 3.2  
c = a + b  
what values does c now hold?  
8.2  
irb says 8.2!  

var1 = "lawl"  
var2 = "brb"  
what value does var2 now hold?  
brb  
irb says brb!  

e = 6 + 3  
what values does e now hold?  
9  
irb says 9!  
  
f = 3.5  
f = f + 2  
what value does f now hold?  
5.5  
irb says 5.5!  

poodle = 4  
pitbull = 3  
what value does boxer now hold?  
nil  
irb says NameError!  
  
h = 5  
h = h + h  
what values does h now hold?  
10  
irb says 10!  

j = 1  
k = 2  
m = 3  
n = j + k + m  
what value does n now hold?  
6  
irb says 6!  
  
p = "moo"  
q = "quack"  
p  = q  
what value does p now hold?  
quack  
irb says quack!  
  
r = "moo"  
s = "quack"  
t = "woof"  
r = t  
what value does r now hold?  
woof    
irb says woof!  
  
u = 5  
u = u * 2  
u = u * 2  
u = u * 2  
what value does u now hold?  
40  
irb says 40!  
  
v = "b"  
z = "a"  
what value does v now hold?  
b  
irb says b!  
  
aa = 3234  
bb = 2398  
cc = 0  
dd = (aa + bb) / cc  
what value does d now hold?  
0  
irb says ZeroDivisionError!  
  
yy = 7  
zz = yy % 2  
what value does zz now hold?  
3.5  
irb says 1 :(  
  
ee = 12  
ff = ee % 4  
what value does ff now hold?  
1  
irb says 0 :(  
  
zz = 17  
hh = zz % 3  
what value does hh now hold?  
6  
 irb says 2 :(  
  
### Operators practice:  
Consider the following variable assignments and then fill in the tables  
d = 10  
e = 5.0  
f = 2  
g = 11.0  
h = 3  
i = 1.5  
  
| Operation | Result | Data type of result | Ran in Ruby, am I right? |
| :--- | :--- | :--- | :--- |
| d + e | 15.0 | Float | Yep! |
| f + h | 5 | Integer | Yep! |
| g + h | 14.0 | Float | Yep! |
| d - f | 8 | Integer | Yep! |
| g - e | 6.0 | Float | Yep! |
| (h + i) - f | 2.5 | Float | Yep! |
| (d - f) + e | 13.0 | Float | Yep! |
| d * f | 20 | Integer | Yep! |
| g * i | 16.5 | Float | Yep! |
| f * g | 22 | Integer | no I missed the float 22.0 |
| d / f | 5 | Integer | Yep! |
| d / e | 2 | Integer | no I missed the float 2.0 |
| e / f | 2.5 | Float | Yep! |
| (g * f) / f | 11 | Integer | no I missed the float 11.0 |
| (d / f) * e | 25 | Integer | no I missed the float 25.0 |
| 21 / 5 | 4.2 | Float | no float was wrong 4 |
| 14 / 5 | 2.8 | Float | no float was wrong 2 |
| 10 % 3 | 3.33 | Float | no it's 1? |
| 20 % 2 | 10 | Integer | no it's 0?? |
| 4 % 5 | .08 | Float | no it's 4? |
| 8 % 1 | 8 | Integer | no it's 0?? |

Need to learn more about modulus  

### String practice:  
Determine the output of slice on your own and then check your answer using irb  

problem 1
my_string = "I love Seattle"
my_string.slice(7) 
I think the output is:
S
Checking in irb it's:
Correct!

problem 2
my_string = "I love Seattle"
my_string.slice(2, 4)
I think the output is:
l v
Checking in irb it's:
love- does the range

problem 3
my_string = "I love Seattle"
my_string.slice("Seattle")
I think the output is:
Seattle
Checking in irb it's:
Correct!

problem 4
my_string = "Ada"
my_string + " Lovelace"
I think the output is:
Ada Lovelace
Checking in irb it's:
Correct!

problem 5
my_string = "Ada"
my_string << " codes" << " it!"
I think the output is:
Ada codes it!
Checking in irb it's:
Correct!

problem 6
my_string = "Ada"
my_string.concat(" likes to code").slice(4...9)
I think the output is:
likes
Checking in irb it's:
Correct!

problem 7
my_string = "Hello world"
"Goodbye " + my_string.slice(6, 5) << "!"
I think the output is:
Goodbye w !
Checking in irb it's:
Goodbyew! -- I added too many spaces to my answer

problem 8
my_string = "Hello world!"
my_string.slice(0...5).concat(", goodbye!")
I think the output is:
Hello, goodbye!
Checking in irb it's:
Correct!

problem 9
my_string = "Hello world!"
my_string.slice(0) << "i" + "!"
I think the output is:
Hi!
Checking in irb it's:
Correct!

problem 10
my_string = "I love ruby"
my_string.slice(7, 4).concat(my_string.slice(2...6)) + my_string.slice(0)
I think the output is:
Rvlove I
Checking in irb it's:
No, it's RubyloveI
looking back at the code…. I get the last part, I don't get the Ruby part

problem 11
my_string = "I love ruby"
"R".concat(my_string.slice(8, 3) + " rocks!")
I think the output is:
Ruo rocks!
Checking in irb it's:
Rubyrocks!
Hm got this wrong too- looking back at the code it's similar to the last one I missed- cutting backwards but spelling forwards

problem 12
my_string = "I love ruby"
my_string.slice(2, 4) << my_string.slice(7...11).concat(my_string.slice(2...6))
I think the output is:
lvrubylove 
Checking in irb it's:
loverubylove
well I was close- I missed the range part but now I know it

## MadLibs!

For the next part, I looked at the titles of the EDUPLACE Wacky Adlibs list- I didn't read the copy, just used the titles as inspiration. I picked "Why I love Fall"

Final:
NAME I just grabbed my favorite scarf, it's officially Fall! My favorite season :) There are many reasons to love Fall. First, you have the ADJECTIVE weather. Neither too hot nor too cold, it's perfect for going for a OUTDOOR ACTIVITY, reading at home, or anything in between, especially with SINGULAR NOUN. 
I believe all PLURAL NOUN ANIMAL are better in the fall- they're so fun to watch! At night the COLOR sky just sparkles with stars, and all around you can hear the ADVERB sound of peaceful nature. 
Don't even get me started on the ADJECTIVE food! All season long, you have at least NUMBER options for yummy things. From BREAKFAST FOOD to DESSERT, hearty, flavorful, and filling foods are the name of the game. Hot apple cider isn't too bad either!
No year is complete without a soothing, restful, reenergizing, and delicious Fall season. Don't you agree, NAME? It's okay to agree or disagree, you can have your own opinion. Why is FAVORITE SEASON your favorite season? What do you like to do with FRIEND during that time? 

Asking for:
1. ADJECTIVE
2. OUTDOOR ACTIVITY
3. SINGULAR NOUN
4. PLURAL NOUN ANIMAL
5. COLOR
6. ADVERB
7. SECOND ADJECTIVE
8. NUMBER
9. BREAKFAST FOOD 
10. DESSERT
11. NAME
12. FAVORITE SEASON
13. FRIEND

I have a Ruby file open in Atom. 
Taking a break to rewatch the video, then going back to this. 

Here's what I have in my Ruby file so far:
these are the variables:
1. ADJECTIVE:
2. OUTDOOR ACTIVITY:
3. SINGULAR NOUN:
4. PLURAL NOUN ANIMAL:
5. COLOR:
6. ADVERB:
7. SECOND ADJECTIVE:
8. NUMBER:
9. BREAKFAST FOOD:
10. DESSERT:
11. NAME:
12. FAVORITE SEASON:
13. FRIEND:

this is the start where I ask for the words
Print "It's MadLib season! I need your help finishing this bit of writing. I'm going to ask you 13 questions and each answer should be only one word. Ready? Here's the first one:
Adjective"
Adjective = gets.chomp

Here's the final paragraph and where the outputs should go:
puts "NAME I just grabbed my favorite scarf, it's officially Fall! My favorite season :) There are many reasons to love Fall. First, you have the " Adjective " weather. Neither too hot nor too cold, it's perfect for going for a OUTDOOR ACTIVITY, reading at home, or anything in between, especially with SINGULAR NOUN.
I believe all PLURAL NOUN ANIMAL are better in the fall- they're so fun to watch! At night the COLOR sky just sparkles with stars, and all around you can hear the ADVERB sound of peaceful nature.
Don't even get me started on the ADJECTIVE food! All season long, you have at least NUMBER options for yummy things. From BREAKFAST FOOD to DESSERT, hearty, flavorful, and filling foods are the name of the game. Hot apple cider isn't too bad either!
No year is complete without a soothing, restful, reenergizing, and delicious Fall season. Don't you agree, NAME? It's okay to agree or disagree, you can have your own opinion. Why is FAVORITE SEASON your favorite season? What do you like to do with FRIEND during that time?""


Okay I'm made some changes. Now I'm at:
this is the start where I ask for the words
print "It's MadLib season! I need your help finishing this bit of writing. I'm going to ask you 13 questions and each answer should be only one word. Ready? Here's the first one:
ADJECTIVE"
Adjective = gets.chomp

print "Here's the next one! 
OUTDOOR ACTIVITY: "
OUTDOOR_ACTIVITY: = gets.chomp

print "Here's the next one! 
SINGULAR NOUN: "
SINGULAR_NOUN = gets.chomp

print "Here's the next one! 
PLURAL NOUN ANIMAL: "
PLURAL_NOUN_ANIMAL = gets.chomp

print "Here's the next one! 
COLOR: "
COLOR = gets.chomp

print "Here's the next one! 
ADVERB: "
ADVERB = gets.chomp

print "More than halfway there you're awesome! How about a: 
SECOND ADJECTIVE: "
SECOND_ADJECTIVE = gets.chomp

print "Here's the next one! 
NUMBER: "
NUMBER = gets.chomp

print "Here's the next one! 
BREAKFAST FOOD: "
BREAKFAST_FOOD = gets.chomp

print "Here's the next one! 
DESSERT: "
DESSERT = gets.chomp

print "Here's the next one! 
YOUR NAME: "
YOUR_NAME = gets.chomp

print "Here's the next one! 
FAVORITE SEASON: "
FAVORITE_SEASON = gets.chomp

print "Last one! You rock :) 
FRIEND'S NAME: "
FRIENDS_NAME = gets.chomp


Here's the final paragraph and where the outputs should go:
puts "Guess what, #{YOUR_NAME}? I just grabbed my favorite scarf, it's officially Fall! My favorite season :) There are many reasons to love Fall. First, you have the #{ADJECTIVE} weather. Neither too hot nor too cold, it's perfect for going for a #{OUTDOOR_ACTIVITY}, reading at home, or anything in between, especially with #{SINGULAR_NOUN}.
I believe all #{PLURAL_NOUN_ANIMAL} are better in the fall- they're so fun to watch! At night the #{COLOR} sky just sparkles with stars, and all around you can hear the #{ADVERB} sound of peaceful nature.
Don't even get me started on the #{ADJECTIVE}, #{SECOND_ADJECTIVE} food! All season long, you have at least #{NUMBER} options for yummy things. From #{BREAKFAST_FOOD} to #{DESSERT}, hearty, flavorful, and filling foods are the name of the game. Hot apple cider isn't too bad either!
No year is complete without a soothing, restful, reenergizing, and delicious Fall season. Don't you agree, #{YOUR_NAME}? It's okay to agree or disagree, you can have your own opinion. Why is #{FAVORITE SEASON} your favorite season? What do you like to do with #{FRIENDS_NAME} during that time?"

whomp whomp syntax error:
(repl):8: syntax error, unexpected ':', expecting end-of-input
OUTDOOR_ACTIVITY: = gets.chomp
Gotta get that : out of there

Oops my adjective variable was off-
uninitialized constant ADJECTIVE
Did you mean?  Adjective
changing that.

uninitialized constant SEASON
(repl):59:in `<main>'
annnnd season is missing a _- fixed now!

All good :)

Curious about "[Optional] Explore Ruby's built in methods for String like capitalize, downcase, upcase"

Added ""FRIENDS_NAME".capitalize" to program
that didn't work.
Googled- ended up on StackOverflow
This works! FRIENDS_NAME.capitalize!

Added it to file :)





