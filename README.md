mxunit_sublime_snippets
=======================

SublimeText snippets to help scaffold MXUnit test cases.

##Installation

 1. Clone this repository into your Sublime Packages directory.
 2. Download the zip for this repository, copy the files into a new folder into your Sublime Packges directory.

##Usage

These snippets will only be triggered in a .cfc so you'll need to create a new file and save it as a .cfc before using these.


###To stub a new test case type: 
```
  _tc<tab>
```

The resulting code will look like:

```cfml
component extends="mxunit.framework.TestCase"{
  public void function setUp(){
		
	}
}
```

The cursor will be in the body of the new setup method.

###To create a new test method type:

```
_t<tab>
```

The resulting code will look like:

```cfml
  public void function test(){
		var expected = ;
		var actual = ; 
		
		
	}
```

The cursor will be right after the word ```test```.  The first tab will highlight the entire ```var expected = ;``` line, the second tab will place the cursor after the ```=```, the third tab will highlight the entire ```var actual = ;``` line, the fourth tab will place the cusor after the ```=```, the fifth tab will place the cursor on the empty line below the expected and actual expressions.

