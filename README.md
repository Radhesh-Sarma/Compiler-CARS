# Compiler CARS

Our language is named 'CARS'
Parser designed in Python 3.x

# Group Details

* Radhesh Sarma: 2017B4A70886H
* Chatrik Singh Mangat: 2017B5A70822H
* Ashi Sinha: 2017B5A71149H
* Simran Sahni: 2017B5A70856H

## Parser Capabilities

Current parser capabilites:
1) Tokenizing & identifying the tokens
2) Lines starting with '#' are skipped, only single line comments supported right now
3) Read the C files in the same folder line by line & parse it, calling the Class token objects & static methods
4) A big dictionary of all possible token kinds is maintained & checked from

## BNF for our Mini Language

  
* `'<program> -> <statement><delimiter>|<delimiter>'`
*  `<statement> -> <keyword><var><operator><var><delimiter> | <statement> | `
*  `<conditional><statement> | <loop><statement>`
* `<keyword> -> true | false | return | void | main`
* `<datatype> -> int | float | boolean | string | while`
* `<loop> -> while<statement>{}| for<statement> {} | until<statement> {}`
* `<conditional> -> if <statement> {} | else <statement> {}`
* `<var> -> <datatype><id>|<id>`
* `<operator> -> +| - | % | / | * | == | > | < | >= | <= | != |&&| || | | ! 		 | ? | : | = | " | $`
* `<delimiter> ->  { | } | ( | ) | [ | ] | , | ;`

## Basic syntactical rules

1) strings only in double quotes
2) all standard data-types recognized in keywords
3) Most of the arithmetic & boolean operators supported
4) Identifier names cannot start with numbers & cant include any substring that is a keyword

