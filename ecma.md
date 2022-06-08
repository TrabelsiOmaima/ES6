ES6 = tips and tricks 
Goal : to make your code cleaner, shorter, and easier to read!

# Template literals :
var b = `Hi, I'm ${ fName } ${ sName }, I'm ${ age } and work as a ${ job }.`;


# Syntax Block scoping :
+ var x = 5 ;       //global
+ { let x=7 ; }     // bloc 
+ { let x=1 ;}      // an other bloc
+ (function () {    // IIFE
     let x = 100;
  })();

=> pas de confilit, pas d'error
each x , bound to a block scoping 


# ‘Let’ Declaration :
+ var # let
+ var : global 
+ let : used f scope


# Const :
+ simploe type : constante a ne pas modifier, (ni type,ni valeur)
+ type complexe (array, object) : the value can still be modified.



# Problem with block scoping functions :
+ if declaration ta3 l function wst { } , so t5dmch l barra mn heka scope 



# Spread :   ...a 
+ spreading an array or object into a new array or object :
let a = [3, 4, 5];
let b = [1, 2, ...a, 6]; //123456
+ pass args in a function :
function foo(a, b, c)  { }
let data = [5, 15, 2];
foo( ...data); 



#  Default Parameters :
+ les valeurs par defauts...
+ null and false values are coerced to 0.



# Destructuring :
+ extract part of an object or an array, 
+ extract the values but assign them to a new variable.
let {a,c} = functionName() or = objectname or = arrayname


# Object Literals and Concise Parameters :
c = { a: a, b: b };  //key=value
format consise de  
c = { a, b };  



# Dynamic Property Names :
let  city= 'sheffield_';
{[ city + 'population' ]: 350000}
{[ city + 'county' ] = 'South Yorkshire' }



# Arrow Functions :
let bar = ( a, b ) => a * b;
let b = arr.map( item => item + 3 )

+ One of the most useful places for arrow functions is in array functions like 
.map
.forEach
.sort
.filter



# Loops    for … of  :
to loop Arrays, strings, generators and collections 

    let tab = ['a', 'b', 'c', 'd' ];


+ for ... in  //  key/index :

    for ( var i in tab ) {    
      console.log( i )    // 0 1 2 3
      console.log( tab[i] )    // "a" "b" "c" "d"
      ;} 



+ for … of //value of tab  : 

    for ( var val of tab ) {    
      console.log( val )    // "a" "b" "c" "d"
      ;} 



# Number Literals :
Number( 0b11101 ) // 29 in binary
Number( 0x1d ) // 29 in hexadecimal
Number( 0o35 ) // 29 in new octal 


