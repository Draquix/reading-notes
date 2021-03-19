## Exception Handling and Debugging

[source article: Try Catch](https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-use-the-try-catch-block-to-catch-exceptions)

Code placed in a try block can have the exception handled in a catch block.
Specific errors can be logged as to their type to find bugs in code.

     try {
         //perform an operation
     }
     catch (FileNotFoundException e)
     {
         Console.WriteLine($"The file was not found: {e}",e);
     }

throw syntax:  throw [e];  || throw new IndexOutOfRangeException
catch syntax: catch [e]; || catch(IndexOutOfRangeException e){//how to handle it.}

Throw can be used inside a catch block to rethrow an exception. [source](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/throw)
throw can be used in an if condition to trigger an exception handling.

With the Therac-25 radiation therapy machine, bugs in the software ended lives prematurely.  
Some causes of death from the machine can be traced to the software design methods.
They didn't run automatic tests on their code or have it independantly reviewed.
Certain common user errors were not accounted for and seemingly standard operations of the machine could cause it to deliver lethal amounts of radiation.
Failsafes were not put in place to barr operations of the machine that could have been distinguished to the software as dangerous and not to be performed.

Ariane_5 is a new design model for a surface to space shuttle.
It has an integrated 2 stage booser jet for liftoff.
The first test flight triggered the rocket to explode because of the software's error.
A 64-bit float was converted to a 16-bit signed integer in a way that triggered a processor trap and the controls locked up.
Ariane 5 model shuttles have delivered the largest known satelite payloads to space.