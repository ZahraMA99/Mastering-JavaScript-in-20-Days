## Conditionals :loop:
**Conditional Statment types:** 
  1. if statment.
  2. if-else stament.
  3. shortcut operator! it needs 3 values to work. `syntax` => condition ? value if truth : value if false;

>💌 Note:
>IF WE WANT TO PASS VARIABLES TO CONSOLE.LOG STATMENT WE SEPARAYE THEM BETWEEN **COMMAS**.<br/>
>(e.g. console.log(x, "is less than", y). 

**Loops:**
  1. for loop.
  2. for of: iterative over items in array or over characters in a string.
  3. for in:  iterates only over keys of an object which have their enumerable property set to “true”.

### Complete TicTacToe project:
```
for (let b of optionButtons){
        b.addEventListener("click", event =>{
                        
            explanation.textContent = fact.explanation

            for (let allB of optionButtons)
                disable(allB)
        

            if (isCorrect(b.value)){
                b.classList.add("correct")
            }else{
                b.classList.add("incorrect")
            }

        })
    }
```

## Delieverables⚙️
