# Learn-YAML By Anand 🥷
> YAML stands for “YAML Ain't Markup Language”
> YAML files are created with extensions “.yaml” or “.yml”. we can use any IDE or text editor to open/create YAML files. 
> > YAML is a light-weight, human-readable data-serialization language. It is primarily designed to make the format easy to read while including advanced features. It is similar to XML and JSON files but uses a more minimalist syntax even while maintaining similar capabilities.
> > It is very easy and simple to represent complex mapping. Due to this, it is heavily used in configuration settings.

## XML vs JSON vs YMAL 🤖
> <img width="605" alt="image" src="https://github.com/Akashay-Anand/Learn-YAML/assets/82114930/2993f3c4-f7ba-4a09-836b-6f25a93fbed3">
> <img width="612" alt="image" src="https://github.com/Akashay-Anand/Learn-YAML/assets/82114930/4c3bb5e6-6239-4666-b1a5-f356b5701839">

## YAML Use-cases 🌐

* As YAML is more readable and lightweight format, it is widely used in writing configuration files in different DevOps tools, cloud platforms, and applications.
* Ex:
* <img width="650" alt="image" src="https://github.com/Akashay-Anand/Learn-YAML/assets/82114930/6f127d3f-d89a-4a4e-8877-00167411c16f">

# Now we had an overview of YAML, So let's see how to work with YAML files 🧑🏻‍💻

* > Indentation of whitespace is used to denote structure. (similar to Python) uses indentation to highlight the blocks of code.
* > Tabs are not included as an indentation for YAML files. So please be careful with space and tabs inside YAML files
* > The basic structure of a YAML file is a map/dictionary/hash etc., which means data is stored as key-value pair
* > YAML is case-sensitive in nature. [name: accounts != Name: Accounts]


// Most things in a YAML file are a form of key-value pair. Key-value pairs. where __'Scalars'__ represent a single stored value.   
// YAML supports common types like integer and floating-point numeric values, as well as non-numeric types Boolean and String.  
// Note: There should be space between key and value   
// bellow is the yaml file example   


``` .yml
# Everything is declared Implicitly 
name: Anand
language: "Java python c++"
area: 'Online'
major-version: 2
minor-version: 9.5;
hex: 0x12d6 #evaluated to 4533
Octal: 624432 #evaluated to 105224
goodDay: true
badday: false
niceweekend: Yes
boringweekend: No
positive-infinity: .inf #evaluates to ifinity
negative-infinity: -.Inf #evaluated to negative infinity
invalidNumber: .NAN #Not a Number
no-value: null
```

#### Comments in YAML
* > One of the key differences and advantages of YAML compared to JSON is it will allow comments inside documents. In JSON, comments are not allowed
* > A commented block is skipped during execution and helps to add a description for the specified code block
* > YAML allows you to add comments to files using the hash symbol (#) similar to Python comments
* > YAML does not support multi-line comments. 

``` yml
# This is a single-line comment
# No multi-line comment suported.  
```

### Implicit & Explicit Typing 
> YAML offers versatility in typing by auto detecting data types while also supporting explicit typing options  
> To tag data as a certain type, simply include __!! typeName__ before the value  

``` yaml
# Boolean explicit declaration
YAML is a superset of JSON: !!bool true
Pluto is a planet: !!bool false
Earth is a planet: !!bool true

# Integer explicit declaration
negative: !!int -16
zero: !!int 0
positive: !!int 30

# Float explicit declaration
negative-flot: !!float -3.14
zero-flot: !!float e
positive-float: !!float 16.

# String explicit declaration
sampleNumString: !!str 8.14
sampleString: !!str EazyBytes
sampleDate: !!str 1989—06—16

# Timestamp explicit declaration
randomdate: !!timestamp 2601—12-15 2:59:43.10

# Noll explicit declaration
key with null value: !!null null
```

#### Strings
> Strings in YAML doesn’t need explicit double or single quotes   
> Use single or double quotes in YAML if your value includes special characters. For example, these special characters may require quotes: {, }, [, ], ,, &, :, *, #, ?, |. -, <. >, =, !, %, @, \.  
> "Yes" and "No" should be enclosed in quotes (single or double) or else they will be interpreted as True and False boolean values.  

### Timestamp 
*> A timestamp value represents an instance of time. It is a helpful data type that lets you store times as a unit rather than as a collection of different numbers. 
*> Using __!!timestamp__ data tag we can hold various levels of date formats as per our requirements Below are the few examples,

``` yml
# Example
canonical: 2001-12-15T02:59:43.1Z
iso8601: 2001-12-14t21:59:43.10-05:00
space separated: 2001-12-14 21:59:43.10-5
no time zone (Z): 2001-12-15 2:59:43.10
date (00:00:00Z): 2002-12-14
```
* If the time zone is omitted, the timestamp is assumed to be specified in UTC The time part may be omitted altogether, resulting in a date format In such a case, the time part is assumed to be 00 00 00 Z (start of day, UTC)
* We can define the timezone by including how many hours it is ahead or behind UTC For example, we can set a timestamp as EST with a 5 at the end.

// Resources
* https://yaml-online-parser.appspot.com/
* https://www.json2yaml.com/

### SEQUENCES/COLLECTIONS

> Sequences are values listed in a specific order A sequence starts with a dash and a space You can think of a sequence as a Python list or an array in Bash or Perl They can be defined with either block style or inline flow style

> Block style uses spaces to structure the list or array It’s easier to read but is less compact compared to flow style

> In Flow styles we can write sequences inline using square brackets, similar to an array declaration in a programming language like Python, Java or JavaScript Flow style is more compact but harder to read at a glance

> We can always, embed a sequence into another sequence

> Ex:
> <img width="578" alt="image" src="https://github.com/Akashay-Anand/Learn-YAML/assets/82114930/ea0c4dec-88c4-4ca9-aac1-c9ef307853ef">


### DICTIONARIES/MAPPINGS
> Dictionaries are collections of key value pairs all nested under the same subgroup They’re helpful to divide data into logical categories for later use

> Dictionaries are defined with a name, a colon, and a space followed by 1 or more indented key value pairs

> Using Dictionaries, we can build information related objects like Person, Application, Vehicle etc

> The key value is YAML's basic building block Every item in a YAML document is a member of at least one dictionary The key is always a string The value is a scalar so that it can be any datatype So, as we've already seen, the value can be a string, a number, or another dictionary

> Ex:
> <img width="553" alt="image" src="https://github.com/Akashay-Anand/Learn-YAML/assets/82114930/c40a2ca2-c9b9-45be-b429-41f57029f338">


### COMMON STRUCTURE OF YAML

> <img width="671" alt="image" src="https://github.com/Akashay-Anand/Learn-YAML/assets/82114930/7918800a-2ec9-481a-b176-4b5359cfa162">




# I will be adding more content very soon;
# Happy Learning 🧑🏻‍💻🥷👩🏻‍🚀
