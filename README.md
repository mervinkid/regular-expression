# Personal and common use regular expressions

#### Match stdout code from java or groovy.
```
(System.out.print)(ln)?(\()(( )*(")?([\w ])+(")?( )*)?(\))(;)*
```

#### Match block comment.
```
(/\*)([\s\S]*?)(\*/)
```

#### Match line comment.
```
(?<!(:))(//)( )*(\w|\W)*?(\n)
```

#### Match part of java jar file name.
This regular expression used to match the version and extion name of full jar file name.
```
(-)((\d)|(\.))+((-|.)(\w)+)*.jar
```