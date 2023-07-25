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


// Most things in a YAML file are a form of key-value pair. Key-value pairs. where 'Scalars' represent a single stored value.   
// YAML supports common types like integer and floating-point numeric values, as well as non-numeric types Boolean and String.  
// Note: There should be space between key and value   
// bellow is the yaml file example   

``` .yml
name: Anand
languagge: "Java python c++"
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


#### Strings in YAML
> Strings in YAML doesn’t need explicit double or single quotes   
> Use single or double quotes in YAML if your value includes special characters. For example, these special characters may require quotes: {, }, [, ], ,, &, :, *, #, ?, |. -, <. >, =, !, %, @, \.  
> "Yes" and "No" should be enclosed in quotes (single or double) or else they will be interpreted as True and False boolean values.  



// Resources
* https://yaml-online-parser.appspot.com/
* https://www.json2yaml.com/



# I will be adding more content very soon;
# Happy Learning 🧑🏻‍💻🥷👩🏻‍🚀
