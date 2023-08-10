## Values & Data Types :sweat_drops:
**JS has two type of data:**
- Primitive data types:
    1. String
    2. number
    3. boolean
    4. undefind
    5. null  
- Objects (e.g document & friends).
  
💡 We can use The `typeof` operator that returns a string indicating the type of the operand's value! e.g:
 1. `typeof("sofia")` returns String.
 2. `typeof(42)` returns number.
 3. `typeof(null)` returns object. "Sometimes js does stuff that we don't expect.:sweat_smile:"
 4. `typeof(document.title)` returns String.
 5. `typeof(undefiend)` returns undefined.

:ab: **Srings:**
- Length of String:
`.length` property used to know how many characters in the string. 
(e.g):
<br/>`"sofia".length` returns 5.
<br/>`"some string".length` returns 4.
<br/>`" ".length` returns 1. "space is character".

- Index of String:
<br/>`"sofia"[2]` returns "f".
<br/>`"sofia".indexOf("f")` returns 2.
<br/>`"aloha".indexOf("a")` returns 0. "It take the first appearnce of the charachter."
<br/>`"sofia".indexOf("z")` returns -1. "convention in js🚩! if characters not exist in the string, `indexof` will return -1".
<br/>`"sofia".indexOf("fia")` returns 2.
<br/>`"sofia".indexOf("lol")` returns -1. 

- Includes:
<br/>`"sofia".includes("f")` returns `true`.
<br/>`"sofia".includes("lol")` returns `false`.

- Starts with:
<br/>`"sofia".startsWith("s")` returns `true`.
<br/>`"sofia".startsWith("lol")` returns `false`.

 ```
<br/>⚙️ **Exercises:** 
   // 1. Add your last name in the players listing.
    document.getElementById("p1-name").append(" Vakil")
    // 2. Retrieve the first "T" in the page title.
    document.title returns "JavaScripTacToe"
    document.title.indexOf("T") returns 10
    // 3. Answer whether the page title contains the string "JavaScript"
    document.title.includes("javaScript") returns "false
    // 4. Capitalize the heading "Tic Tac Toe"
    document.querySelector("header h1").style.transform = "uppercase" returns TIC TAC TOE. <br/>```

   
🔮 **Note:** 
    <br/>JS CAN MANIPULATE THE HTML AND CSS OF THE PAGE


## Operators :sweat_drops:
- Plus sign (+) 💫
It used for several uses:
    1. Adding numbers: (e.g: 1 + 4).
    2. Concatenating strings: (e.g: "sofia" + "ali") || (e.g: "sofia" + 2). "both sides or one side at least must be string". 
