# Personal and common use regular expressions
***
### Java print method invoke
```
(System.out.print)(ln)?(\()(( )*(")?([\w ])+(")?( )*)?(\))(;)*
```
***
### Block comment
```
(/\*)([\s\S]*?)(\*/)
```
***
### Line comment
```
(?<!(:))(//)( )*(\w|\W)*?(\n)
```
***
### Version info of java jar file name
This regular expression used to match the version and extion name of full jar file name.
```
(-)((\d)|(\.))+((-|.)(\w)+)*.jar
```
***
### XML
#### XML tags with comments
```
((<)(!)?(((\w)+([ \n]+(\w|-)+(( )*(=)( )*("|')[\s\S]*?("|'))?)*)|(/(\w)+))( )*(/)?(>))|(<!--[\s\S\n]*?-->)
```
#### XML tags without comments
```
(<)(!)?(((\w)+([ \n]+(\w|-)+(( )*(=)( )*("|')[\s\S]*?("|'))?)*)|(/(\w)+))( )*(/)?(>)
```
#### XML comments
```
<!--[\s\S\n]*?-->
```
#### JS code block
```
(<script([ \n]+(\w|-)+( )*(=)( )*("|')[\s\S]*?("|'))*)( )*(>)[\s\S\n]*?(</script)( )*(>)
```