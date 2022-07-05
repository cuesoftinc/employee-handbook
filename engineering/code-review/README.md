# CODE REVIEW AND BEST PRACTICES

## SOME USEFUL GUIDES

- [IMPORTANT: Flutter Best Practices](https://medium.com/flutter-community/flutter-best-practices-and-tips-7c2782c9ebb5)


- [IMPORTANT: JavaScript Best Practices](https://www.w3.org/wiki/JavaScript_best_practices)

## Few basics. 
- `print` should NOT be present in production code. Never push this in. If you're using this for debugging - please stop doing that and use a standard debugger like `log` instead. 
- Never push commented code in. Comments are fine, commented code is not. 
- Endeavour to use `SVG` for icons always, because it scales really really well. Never use `PNG, GIF, JPEGS`. 

## General
- If working on a Codebase for the first time, make sure Codebase and the project's essential tools are installed and working properly on your machine. If you experience any difficulty or require any help, reach out to your senior engineers for help. 
Make sure to send a PR daily so your code can be reviewed.
- Both private and public repositories are hosted on Github.
- To work on a repo, clone it to your local device.
- Endeavour to always create feature branches if you're working on a feature. For example, if you're working on login feature, create a branch from main called `feature/login`
- If you're working on a bug then create a new branch from main called `bug/login-fix`.
- **Important:** Send a PR to develop and not to main.
- Only send a PR to develop when you're completely done with your feature and properly tested.
- Push changes in everyday. It's important to push changes in when you're done with your work daily.This would result in a server backup of your work. Your work does not stop if your local pc crashes.
-  It is YOUR responsibility to get a PR merged in when you send it to develop. For review, contact a peer developer.
- When your work is on develop, test it manually on the develop server. When everything looks good. Go to your develop branch and send in a PR to main. Your task is ONLY done when your work is merged to main.
- Function names should be a verb. Functions do something. Example: save(), delete(), login(), etc. If you're writing JavaScript or Dart, function names should be camelCase (The first letter of the function should be lower case, the next subsequent word should be upper case). If you're writing code in any other language then follow the best practices of that language. For example: In C# function names are PascalCase  (The first letter of the function is upper case, the next subsequent word is also upper case).
-Reusable code is the way to go! If you're copy and pasting code on your app, this is a clear indication you're on the wrong path. Make the code you want to copy paste into widget/ module / component / function  / class  and reuse that.
When you're starting to write a new function think it through. Think about:
- Is the same functionality is already implemented in another function, then use that instead of the new one.
- Think twice about the function name. Do you get what the function does if you read the function name.
- Write quick documentation before the function.

```
FunctionName: One quick sentence of what this function does.
Parameters:
<Param1> |  <Type>  | <One quick sentence on what this param does>
<Param2> |  <Type>  | <One quick sentence on what this param does>
<ParamN> |  <Type>  | <One quick sentence on what this param does>
Returns:
What does this function returns, If this function is a Future or a Promise. Then say what the it returns when it is successful and when it fails.  
```


- Class names should be a noun. Classes are something. Example: Student, CloudObject, etc. If you're writing JavaScript or Dart, class names should be PascalCase  (The first letter of the class is upper case, the next subsequent word is also upper case). If you're writing code in any other language then follow the best practices of that language.
- Write quick documentation before the Class.


```
ClassName: One quick sentence of what this class does.
<Property1> |  <Type>  | <One quick sentence on what this property is>
<Property2> |  <Type>  | <One quick sentence on what this property does>
<PropertyN> |  <Type>  | <One quick sentence on what this property does>
```



