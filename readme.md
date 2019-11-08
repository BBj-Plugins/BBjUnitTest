# Introduction

The BBjUnitTest BBj plug-in is the standalone version of the Eclipse BBjUnitTest plug-in. It is used to develop and run unit tests for your BBj code.

More information about unit tests with BBj can be found [here](https://documentation.basis.com/advantage/v18-2014/14unittest.pdf)

## Prerequisites

This plug-in requires the lib/BBjUnitTest.jar to be added to session's classpath in order to run properly.

## Example Usage

1. Create a new BBj Session specific classpath called "unittest" (without the quotes)
2. Add the BBjUnitTest.jar file from the lib/ folder to the classpath unittest 
3. Save the classpath
4. Open a command prompt
5. Execute the following command by replacing the placeholders (&lt;xxx&gt;) by the correct values:

&lt;BBjHome&gt;/bin/BBj.exe -CPunittest -q -WD&lt;PathToProject&gt;/pgms/ &lt;PathToProject&gt;/BBjUnitTest.bbj - TestMathOperations.bbjt

**Note:** By default the generated results file (saved in the tmp directory by default) will not be overwritten automatically by the plugin, unless you explicitly configured it to do so.

## Execution Options

The plug-in has a set of options which can be used to alternate its behavior. The following options can be used:

|                | Name             | Description                                                             |
|----------------|------------------|-------------------------------------------------------------------------|
| --f            | Force overwrite  | Causes the plugin to overwrite any existing output file without nagging |
| --o <FileName> | Output file path | Sets the output file path                                               |
| --q            | Quiet Execution  | Supresses Exceptions causing the program to continue its execution      |

**Note:** The plugin options should be placed last in the command.
