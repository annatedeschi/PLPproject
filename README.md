# PLP Project by Anna Tedeschi
## PLP 1 Assignment
### History Of Perl
PERL is a high-level, general-purpose coding language developed by Larry Wall in 1987. Its original use was for simple text processing but it has developed and is now used for
web development, system administration, and network programming. PERL stands for " Practice Extraction and Reporting Languages" . One of the main draws of PERL is that 
it has a lot of flexibility to do things. In Perl compared to other languages there are multiple ways to fix or solve a problem. 
### Hello World
Hello World is always the first place to start when learning a new language. 

```print "Hello World!\n";```

Here you can see the syntax we start with the command we want to do, which here is print, and then we follow with quotations which is going to encase what we want to say. Then before we 
finish what we want to say we add \n. This just indicates that the line is done, and then we add the end quotations followed by a semi colon which finishes out line.

## PLP Assignment 2
### Naming Conventions

### Keywords 
Yes, Perl has keywords and reserved words. The exact number may vary depending on the version of Perl, but there are a lot of similarities to other languages like python. 
An example of this is if or else
### Naming Variables
When naming variables they have to either start with a letter or an underscore
### Naming conventions
Perl follows some naming conventions, but they are not enforced by the compiler. An example of this is the lowercase and underscore
to name variables
### Type System
Perl is dynamically typed, meaning you do not need to declare what type the variable is explicitly.
However, it's also weakly typed as well
### Mutability
In Perl, most variables are mutable. You can change the value stored in a variable after it has been created, But not a string making it unmutable
### Operators
Perl provides the basic operates (+, -, *, /), linking strings together using periods(.), comparison operators (==, !=, <, >, ), and logical operators to name a few
### Mixed Type Operations
Perl does allows mixed-type operations. For an example it will combine a string and a interger but perl will turn t
he interger into a number so it can form a new string
Binding:
In Perl variable names are bound to their values when the program is run
### Type Binding
Perl is implicitly typed, which means you do not need to specify variable types like you would with Java. This job is done by the compiler and they determine its types
```
my $int= 109;
#this is how you call an interger
my $string = "Hello, World!";
#this is how you call a string

my $float = 3.14;
#this is how you calling a floating varible with a decimal

my $boolean = 0;
#this is how you call a boolean

my @array = (1, 2, 4, 8, 16);
#this is how you create an array in Perl

my %hash = (
    'ans1' => 'value1',
    'ans2' => 'value2',
    'ans3' => 'value3'
);
#this is how you call a dictionary in Perl which is called a hash
```
## PLP Assignment 3
### Calling a Function
```
use strict;
use warnings;
# we use strict and warning to prevent error message
sub numtimesnum {
    my ($num) = @_;
    return $num * $num;
}
my $result = square(5);

# Print the result
print "The square of 5 is: $result\n";
```
### Recursive Functions
```sub factorial {
    my ($n) = @_;
    if ($n <= 1) {
        return 1;
    }
    return $n * factorial($n - 1);
}

my $ans = factorial(5);
print "Factorial of 5: $fact_result\n";

```
### Calling a Function and saving the answer as a vairable 
```sub numtimesnum {
    my ($num) = @_;
    return $num * $num;
}
my $result = square(5);

# Print the result
print "The square of 5 is: $result\n";

```
### Split String Function
```sub splitstrings {
    my ($input) = @_;
    my ($part1, $part2) = split / /, $input, 2;
    return ($part1, $part2);
}

my ($string1, $string2) = splitstring("Hello World");
print "$string1\n";
print "$string2\n";
```
### Function to check pass-by Value
```# this is creating an array of number bewteen 1-10  
@a = (0..10);  
  

print("Values of an array before function call: = @a\n"); 
  
# naming the sub routine 
sample(@a); 
  

print("Values of an array after function call: = @a"); 
  

sub sample 
{  
    $_[0] = "A"; 
  
    $_[1] = "B"; 
}
```
## Else-If statements

### One Condition Else-If Statement
```
my $x = 6;

if ($x == 5) {
    print "x is equal to 5.\n";
} else {
    print "x is not equal to 5.\n";
}
# this program will print " x is not equal to 5"
```

### Multi Condition Else-If Condition
```
my $x = 7;
my $y = 8;

if ($x > 0 && $y < 10) {
    print "both numbers are between 0 and 10.\n";
} else {
    print "at least one number is not between 0 and 10.\n";
}
```
### If-Else-Elif Statment
```
print "What was your grade on the exam? \n";
$grade = <>;

if ($grade >= 90) {
    print "A\n";
} else ($grade >= 80) {
    print "B\n";
} else ($grade >= 70) {
    print "C\n";
} elsif {
    print "D\n";
}
```
