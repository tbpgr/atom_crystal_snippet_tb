# atom_crystal_snippet_tb

Crystal snippet for atom.
[![apm install atom_crystal_snippet_tb](https://apm-badges.herokuapp.com/apm/atom_crystal_snippet_tb.svg)](https://atom.io/packages/atom_crystal_snippet_tb)

## Types
* .source.crystal

## Snippets
### if … else … end
prefix: if else  
body:

~~~
if (${1:condition})
	$2
else
	$3
end
~~~

### if … end
prefix: if  
body:

~~~
if (${1:condition})
	$0
end
~~~

### it … end
prefix: it  
body:

~~~
it "${1:text}" do
	$0
end
~~~

### case … end
prefix: case  
body:

~~~
case ${1:object}
when ${2:condition}
	$0
end
~~~

### begin … rescue … end
prefix: beging rescue  
body:

~~~
begin
	$1
rescue ${2:ExceptionName}
	$3
end
~~~

### begin … ensure … end
prefix: beging ensure  
body:

~~~
begin
	$1
ensure
	$2
end
~~~

### begin … rescue … ensure … end
prefix: beging rescue ensure  
body:

~~~
begin
	$1
rescue ${2:ExceptionName}
	$3
ensure
	$4
end
~~~

### alias
prefix: alias  
body:

~~~
alias ${1:new_name} = ${0:old_name}
~~~

### getter
prefix: getter  
body:

~~~
getter ${0:attr_name}
~~~

### getter default
prefix: getter default  
body:

~~~
getter ${1:attr_name} = ${0:default}
~~~

### getter type
prefix: getter type  
body:

~~~
getter ${1:attr_name} : ${0:type_name}
~~~

### getter type default
prefix: getter type default  
body:

~~~
getter ${1:attr_name} : ${2:type_name} = ${0:default}
~~~

### setter
prefix: setter  
body:

~~~
setter ${0:attr_name}
~~~

### setter default
prefix: setter default  
body:

~~~
setter ${1:attr_name} = ${0:default}
~~~

### setter type
prefix: setter type  
body:

~~~
setter ${1:attr_name} : ${0:type_name}
~~~

### setter type default
prefix: setter type default  
body:

~~~
setter ${1:attr_name} : ${2:type_name} = ${0:default}
~~~

### print
prefix: print  
body:

~~~
print ${0:argument_name}
~~~

### property
prefix: property  
body:

~~~
property ${0:attr_name}
~~~

### property default
prefix: property default  
body:

~~~
property ${1:attr_name} = ${0:default}
~~~

### property type
prefix: property type  
body:

~~~
property ${1:attr_name} : ${0:type_name}
~~~

### property type default
prefix: property type default  
body:

~~~
property ${1:attr_name} : ${2:type_name} = ${0:default}
~~~

### puts
prefix: puts  
body:

~~~
puts ${0:argument_name}
~~~

### class .. end
prefix: class  
body:

~~~
class ${1:ClassName}
	$0
end
~~~

### def … end
prefix: def  
body:

~~~
def ${1:method_name}(${2:args_name})
	$0
end
~~~

### do .. end
prefix: do end  
body:

~~~
do
	$1
end$0
~~~

### do .. args .. end
prefix: do args end  
body:

~~~
do |${1:e}|
	$2
end$0
~~~

### initialize
prefix: initialize  
body:

~~~
def initialize(${1:argument})
$0
end
~~~

### def self .. end
prefix: def self  
body:

~~~
def self.${1:class_method_name}(${2:argument})
	$0
end
~~~

### each { |e| .. }
prefix: each  
body:

~~~
each { |${1:e}| $0 }
~~~

### each_key { |key| .. }
prefix: each key  
body:

~~~
each_key { |${1:key}| $0 }
~~~

### each_value { |value| .. }
prefix: each value  
body:

~~~
each_value { |${1:value}| $0 }
~~~

### each_with_index { |e, i| .. }
prefix: each_with_index  
body:

~~~
each_with_index { |${1:e}, ${2:i}| $0 }
~~~

### each_with_object { |e, memo| .. }
prefix: each_with_object  
body:

~~~
each_with_object(${1:default}) { |${2:e}, ${3:memo}| $0${3:memo} }
~~~

### elsif ...
prefix: elsif  
body:

~~~
elsif (${1:condition})
	$0
~~~

### error ArgumentError ...
prefix: error ArgumentError  
body:

~~~
ArgumentError
~~~

### error Base64::Error ...
prefix: error Base64::Error  
body:

~~~
Base64::Error
~~~

### error Channel::ClosedError ...
prefix: error Channel::ClosedError  
body:

~~~
Channel::ClosedError
~~~

### error Concurrent::CanceledError ...
prefix: error Concurrent::CanceledError  
body:

~~~
Concurrent::CanceledError
~~~

### error Crypto::Bcrypt::Error ...
prefix: error Crypto::Bcrypt::Error  
body:

~~~
Crypto::Bcrypt::Error
~~~

### error CSV::Error ...
prefix: error CSV::Error  
body:

~~~
CSV::Error
~~~

### error DivisionByZero ...
prefix: error DivisionByZero  
body:

~~~
DivisionByZero
~~~

### error Enumerable::EmptyError ...
prefix: error Enumerable::EmptyError  
body:

~~~
Enumerable::EmptyError
~~~

### error Errno ...
prefix: error Errno  
body:

~~~
Errno
~~~

### error IndexError ...
prefix: error IndexError  
body:

~~~
IndexError
~~~

### error InvalidByteSequenceError ...
prefix: error InvalidByteSequenceError  
body:

~~~
InvalidByteSequenceError
~~~

### error IO::Error ...
prefix: error IO::Error  
body:

~~~
IO::Error
~~~

### error IO::Timeout ...
prefix: error IO::Timeout  
body:

~~~
IO::Timeout
~~~

### error JSON::ParseException ...
prefix: error JSON::ParseException  
body:

~~~
JSON::ParseException
~~~

### error KeyError ...
prefix: error KeyError  
body:

~~~
KeyError
~~~

### error OAuth2::Error ...
prefix: error OAuth2::Error  
body:

~~~
OAuth2::Error
~~~

### error OAuth::Error ...
prefix: error OAuth::Error  
body:

~~~
OAuth::Error
~~~

### error OpenSSL::Error ...
prefix: error OpenSSL::Error  
body:

~~~
OpenSSL::Error
~~~

### error OptionParser::Exception ...
prefix: error OptionParser::Exception  
body:

~~~
OptionParser::Exception
~~~

### error Socket::Error ...
prefix: error Socket::Error  
body:

~~~
Socket::Error
~~~

### error Time::Format::Error ...
prefix: error Time::Format::Error  
body:

~~~
Time::Format::Error
~~~

### error TypeCastError ...
prefix: error TypeCastError  
body:

~~~
TypeCastError
~~~

### error URI::Error ...
prefix: error URI::Error  
body:

~~~
URI::Error
~~~

### error XML::Error ...
prefix: error XML::Error  
body:

~~~
XML::Error
~~~

### error YAML::ParseException ...
prefix: error YAML::ParseException  
body:

~~~
YAML::ParseException
~~~

### error Zlib::Error ...
prefix: error Zlib::Error  
body:

~~~
Zlib::Error
~~~

### find { |e| .. }
prefix: find  
body:

~~~
find { |${1:e}| $0 }
~~~

### first
prefix: first  
body:

~~~
first
~~~

### grep(/pattern/)
prefix: grep  
body:

~~~
grep(${1:/${2:pattern}/})
~~~

### group_by { |e| .. }
prefix: group_by  
body:

~~~
group_by { |${1:e}| $0 }
~~~

### include
prefix: include  
body:

~~~
include ${1:class_name}
~~~

### join
prefix: join  
body:

~~~
join(${1:separator})
~~~

### last
prefix: last  
body:

~~~
last
~~~

### loop { .. }
prefix: loop  
body:

~~~
loop { $0 }
~~~

### map { |e| .. }
prefix: map  
body:

~~~
map { |${1:e}| $0 }
~~~

### map_with_index { |e, i| .. }
prefix: map_with_index  
body:

~~~
map_with_index { |${1:e}, ${2:i}| $0 }
~~~

### max
prefix: max  
body:

~~~
max
~~~

### max_by { |e| .. }
prefix: max_by  
body:

~~~
max_by { |e| $0 }
~~~

### min
prefix: min  
body:

~~~
min
~~~

### min_by { |e| .. }
prefix: min_by  
body:

~~~
min_by { |e| $0 }
~~~

### minmax
prefix: minmax  
body:

~~~
minmax
~~~

### none?
prefix: none?  
body:

~~~
none?
~~~

### module .. end
prefix: mod  
body:

~~~
module ${1:ModuleName}
	$0
end
~~~

### raise exception
prefix: raise exception  
body:

~~~
raise ${1:exception}
~~~

### raise message
prefix: raise message  
body:

~~~
raise "${1:message}"
~~~

### rand
prefix: rand  
body:

~~~
rand
~~~

### reduce { |memo, e| .. }
prefix: reduce  
body:

~~~
reduce(${1:default}) { |${2:memo}, ${3:e}| $0${2:memo} }
~~~

### require ".."
prefix: require  
body:

~~~
require "$0"
~~~

### reverse
prefix: reverse  
body:

~~~
reverse
~~~

### scan(/../) { |match| .. }
prefix: scan  
body:

~~~
scan(/${1:pattern}/) { |${2:match}| $0 }
~~~

### select { |e| .. }
prefix: select  
body:

~~~
select { |${1:e}| $0 }
~~~

### sort
prefix: sort  
body:

~~~
sort
~~~

### ternary_if
prefix: ternary_if  
body:

~~~
${1:case} ? ${2:result1} : ${3:result3}

~~~

### unless … end
prefix: unless  
body:

~~~
unless (${1:condition})
	$0
end
~~~

### when …
prefix: when  
body:

~~~
when ${1:condition}
	$0
~~~

### yield
prefix: yield  
body:

~~~
 :yield ${0:arguments}
~~~

### Array
prefix: Array  
body:

~~~
Array
~~~

### Bool
prefix: Bool  
body:

~~~
Bool
~~~

### Char
prefix: Char  
body:

~~~
Char
~~~

### Class
prefix: Class  
body:

~~~
Class
~~~

### Enum
prefix: Enum  
body:

~~~
Enum
~~~

### Enumerable
prefix: Enumerable  
body:

~~~
Enumerable
~~~

### Float
prefix: Float  
body:

~~~
Float
~~~

### Float32
prefix: Float32  
body:

~~~
Float32
~~~

### Float64
prefix: Float64  
body:

~~~
Float64
~~~

### Int
prefix: Int  
body:

~~~
Int
~~~

### Int32
prefix: Int32  
body:

~~~
Int32
~~~

### Int64
prefix: Int64  
body:

~~~
Int64
~~~

### JSON
prefix: JSON  
body:

~~~
JSON
~~~

### Nil
prefix: Nil  
body:

~~~
Nil
~~~

### Object
prefix: Object  
body:

~~~
Object
~~~

### Proc
prefix: Proc  
body:

~~~
Proc
~~~

### Range
prefix: Range  
body:

~~~
Range
~~~

### Regex
prefix: Regex  
body:

~~~
Regex
~~~

### Set
prefix: Set  
body:

~~~
Set
~~~

### String
prefix: String  
body:

~~~
String
~~~

### Struct
prefix: Struct  
body:

~~~
Struct
~~~

### Symbol
prefix: Symbol  
body:

~~~
Symbol
~~~

### Time
prefix: Time  
body:

~~~
Time
~~~

### Tuple
prefix: Tuple  
body:

~~~
Tuple
~~~

### describe
prefix: describe  
body:

~~~
describe ${1:target} do
	$2
endd$0
~~~

### context
prefix: context  
body:

~~~
context ${1:message} do
	$2
end
~~~

### it
prefix: it  
body:

~~~
it ${1:message} do
	$2
end
~~~

### pending
prefix: pending  
body:

~~~
pending ${1:message} do
	$2
end
~~~

### fail
prefix: fail  
body:

~~~
fail("${1:message}")
~~~

### be_a
prefix: be_a  
body:

~~~
be_a(${1:type})
~~~

### be value
prefix: be value  
body:

~~~
be(${1:value})
~~~

### be_close
prefix: be_close  
body:

~~~
be_close(${1:expected}, ${2:delta})
~~~

### be_false
prefix: be_false  
body:

~~~
be_false
~~~

### be_falsey
prefix: be_falsey  
body:

~~~
be_falsey
~~~

### be_nil
prefix: be_nil  
body:

~~~
be_nil
~~~

### be_true
prefix: be_true  
body:

~~~
be_true
~~~

### be_truthy
prefix: be_truthy  
body:

~~~
be_truthy
~~~

### contain
prefix: contain  
body:

~~~
contain(${1:expected})
~~~

### eq
prefix: eq  
body:

~~~
eq(${1:expected})
~~~

### expect_raises
prefix: expect_raises  
body:

~~~
expect_raises(${1:klass}) do
	$2
end
~~~

### expect_raises message
prefix: expect_raises message  
body:

~~~
expect_raises(${1:klass}, ${2:message}) do
	$2
end
~~~

### match
prefix: match  
body:

~~~
match(${1:value})
~~~

### parametrized
prefix: parametrized  
body:

~~~
macro ${1:method_name}(${2:macro_args}, expected)
  it "${4:it}" do
    actual = ${5:some_logic}
    actual.should eq({{expected.id}})
  end
end

describe "${6:describe}" do
  ${1:method_name} ${7:some_args1}, ${8:some_expected1}
  ${1:method_name} ${9:some_args2}, ${10:some_expected2}
end$0
~~~
