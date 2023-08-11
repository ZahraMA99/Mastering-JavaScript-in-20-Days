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

### Complete TicTacToe project::confetti_ball:
```
for (let ob of optionButtons){
        ob.addEventListener("click", event =>{
                        
            explanation.textContent = fact.explanation

            for (let allB of optionButtons)
                disable(allB)
        

            if (isCorrect(b.value)){
                ob.classList.add("correct")
            }else{
                ob.classList.add("incorrect")
            }

        })
    }
```
## Map & Filters:hourglass_flowing_sand:
- `.map` creates a new array with the results of calling a provided function on every element in the calling array.
- `.filter` it calls a true/false function on each items and creates a new array with only items where the function return true.
  
>💌 Note:
>Arrow function are useful for map method.<br/>

>💌 Note:
```
 console.log( "My name" + s.name + "Aqel" ) is equivelent to console.log( `My name ${s.name} Aqel` );
```

## Delieverables⚙️
