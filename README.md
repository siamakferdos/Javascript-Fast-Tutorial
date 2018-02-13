# Javascript-Fast-Tutorial

This repository contains a file which has commented statements. Just by uncomment them it can be testable and display the result.

<html>

    <body onload="load()">
        <script>
            //var f1 = "k";
            function load() {
                // //---------------------------------------------------------------------------------- (1) variables
                //var name = "siamak";
                //f = 1;
                //f2 = null;
                //f3 = undefined;
                // //-------------------------------------------------------------------------------  1-1   Numbers
                // //Infinites
                // alert(Infinity); /* Infinity */  
                // alert(Infinity + 1); /* Infinity */  
                // alert(Math.pow(10,1000)); /* Infinity */
                // alert(1 / Infinity); /* 0 */
                    
                // //Finites
                // alert("isFinite(Infinity) : " + isFinite(Infinity));  // false
                // alert("isFinite(NaN) : " + isFinite(NaN));       // false
                // alert("isFinite(-Infinity) : " + isFinite(-Infinity)); // false
                // alert("isFinite(0) : " + isFinite(0));         // true
                // alert("isFinite(2e64) : " + isFinite(2e64));      // true
                // alert("isFinite(null) : " + isFinite(null));
                    
                //Not-A-Number NaN
                // alert("2 is not a Number: " + Number.isNaN(2));
                // alert("2 is not a Number: " + isNaN(2));
                // alert("2 is not a Number: " + isNaN("2"));
                // alert("a is not a Number: " + isNaN("a"));
                    
                // //undefined
                // var obj1 = {};
                // alert(obj1.aNotDefinedProperty);
                // alert(undefined);
                // if(obj1.aNotDefinedProperty || obj1.aNotDefinedProperty != undefined)
                //     alert(true);
                // else
                //    alert(false);
                    
                // //null VS undefined  
                // alert(typeof null);        // object 
                // alert(typeof undefined);   // undefined
                // alert(null === undefined); // false
                // alert(null  == undefined); // true
                    
                // //Parse functions 
                // alert("parseInt('-1111', 2) : " + parseInt("-1111", 2));
                // alert("parseInt('1111', 2) : " + parseInt("1111", 2));
                // alert("parseInt('-F', 16) : " + parseInt("-F", 16));
                // alert("parseInt('2') : " + parseInt("2"));
                // alert("parseFloat('3.14') : " + parseFloat("3.14"));
                //---------------------------------------------------------------------------- 1-2 string
                //alert( 4 + 1 + "2");
                //alert( 1 + "2" + 5);
                //alert( 1 + "2" + 5 + 2);
                    
                // alert('"hello".length is : ' + "hello".length);                
                // alert("hello, world".replace("hello", "goodbye"));                
                // alert("hello UPPERCASE is : " + "hello".toUpperCase());
                    
                // alert('cat'[1]);
                // var myString = 'Hello World. How are you doing?';                                     
                // var splits = myString.split(' ');                    
                // alert(splits);                    
                    
                //---------------------------------------------------------------------------- 1-3 array
                // var animal = new Array();
                // animal[0] = "dog";
                // animal[1] = "cat";
                // animal[2] = "hen";
                // alert(animal.length); // 3
                // alert(animal[2]);
                    
                // var animal = ["dog", "cat", "hen"];
                // alert(animal.length); // 3
                // alert(animal[2]);
                    
                //var diffrentTypeArray = new Array();
                //diffrentTypeArray[0] = "string type";
                //diffrentTypeArray[1] = 2;
                //diffrentTypeArray[3] = {newType : "new", newInt : 3};
                //diffrentTypeArray[4] = [1, "2", {h:1, k:2}]; 
                //diffrentTypeArray.forEach(function(key){
                //    alert(key);
                //});
                    
                //**//--------------------------------------------------------------------------- 1-3-1 every
                //function isBigEnough(element, index, array) {                        
                //    return element >= 10;
                //    }
                //alert([12, 5, 8, 130, 44].every(isBigEnough));   // false
                //alert([12, 54, 18, 130, 44].every(isBigEnough)); // true
                    
                //**//----------------------------------------------------------------------------  1-3-2 map
                //var numbers = [1, 4, 9];
                //var doubles = numbers.map(function(num) {
                //    return num * 2;
                //});
                //doubles.forEach(function (element) {
                //    alert(element)
                //});                    
                    
                //**//----------------------------------------------------------------------------- 1-3-3 some
                // function isBiggerThan10(element, index, array) {
                //     return element > 10;
                // }
                // [2, 5, 8, 1, 4].some(isBiggerThan10);  // false
                // [12, 5, 8, 1, 4].some(isBiggerThan10); // true
                    
                //--------------------------------------------------------------------------------- 1-3-4 filter
                //function isBigEnough(value) {
                //    return value >= 10;
                //}
                //var filtered = [12, 5, 8, 130, 44].filter(isBigEnough);                    
                //filtered.forEach(function(key){alert(key)});                   
                
                // --------------------------------------------------------------------------- 1-3-5 array other function
                //var animalGroup1 = ["dog", "cat", "hen"];
                //var animalGroup2 = ["tiger", "eagle", "bear"];    
                                 
                //var allAnimal = animalGroup1.concat(animalGroup2); //Returns a new array with the items added on to it
                //alert(allAnimal.length);                
                //alert(allAnimal[4]);
                     
                //alert(allAnimal.join(",")); //Converts the array to a string
                // 
                // alert(allAnimal.pop()); //Removes and returns the last item.
                // alert(allAnimal.join(","));
                // 
                // allAnimal.push("wolf"); //Adds one or more items to the end.
                // alert(allAnimal.join(","));
                // 
                // alert(allAnimal.slice(2, 4).join(",")); //Returns a sub-array.
                    
                //----------------------------------------------------------------------------- 1-4 dictionary
                //var myMap = new Map();
                //var keyString = "a string",
                //    keyObj = {},
                //    keyFunc = function () {};
                //myMap.set(keyString, "value associated with 'a string'");
                //myMap.set(keyObj, "value associated with keyObj");
                //myMap.set(keyFunc, "value associated with keyFunc");                   
                //myMap.size; // 3
                //// getting the values
                //alert(myMap.get(keyString));    // "value associated with 'a string'"
                //alert(myMap.get(keyObj));       // "value associated with keyObj"
                //alert(myMap.get(keyFunc));      // "value associated with keyFunc"                    
                //alert(myMap.get("a string"));   // "value associated with 'a string'"
                //                        // because keyString === 'a string'
                //alert(myMap.get({}));           // undefined, because keyObj !== {}
                //alert(myMap.get(function() {})) // undefined, because keyFunc !== function () {}
                
                
                // //------------------------------------------------------------------------- (2) oprators
                // alert(1 == "1");
                // alert(1 === "1");
                // alert(1 != "1");
                // alert(1 !== "1");
                
                //---------------------------------------------------------------------------- (3) functions
                // function multiply1(num1,num2) {
                //     var result = num1 * num2;
                //     return result;
                // }                
                // alert(multiply1(2, 4));
                // 
                //var multiFunc = function multiply2(num1,num2) {
                //    var result = num1 * num2;
                //    return result;
                //}
                //alert(multiFunc(2, 3));
                //alert(multiply2(2, 3)); //Error! Not Found multiply2 function
                
                // function add() {
                // var sum = 0;
                // for (var i = 0, j = arguments.length; i < j; i++) {
                //     sum += arguments[i];
                // }
                // return sum;
                // }
                // alert(add(2, 3, 4));
                // alert(add(2, 3, 4, 5));                
               
                //---------------------------------------------------------------------------- 3-1 callBack
                //setTimeout(3000);
                //alert("finished");
                    
                //setTimeout(callBackFunc, 3000);
                //function callBackFunc(){
                //   alert("finished after call back")
                //}
                    
                   
                    
                // //------------------------------------------------------------------------------ (4) object
                //var car1 = {
                //    name: "bmw",
                //    "weight": 100,
                //    details: {
                //        color: "orange",
                //        wheel: 4
                //        }
                //    }
                //alert("weight : " + car1.weight);
                //car1.long = 280;
                //car1["speed"] = "300 km/h";
                //alert("long : " + car1.long);
                //alert("speed : " + car1.speed);
                
                // //--------------------------------------------------------------------------- 4-1 constructor, prototype
                    //function Tree(name) {
                // this.name = name;
                        //return {
                        //    get a() { return 10; },
                        //    set b(n) {name = n}
                        //}
                     //}
                     //var theTree = new Tree('Redwood');
                     //alert('theTree.constructor is ' + theTree.constructor);
                     //Tree.prototype.area = function (height, width){return height * width;}
                     //alert("the tree area : " + theTree.area(100, 5));
                    // theTree.customArea = function (height, width){return height * width * 2;}
                    // alert("the tree custom area : " + theTree.customArea(100, 5));
                    // 
                    // var secTree = new Tree("MyTree");
                    // alert("sec tree area : " + secTree.area(20, 30));
                    // alert("sec tree custom area : " + secTree.customArea(20, 30)); //Not exist
                
                    // //--------------------------------------------------------------------------- 4-2 inheritance
                    // function Shape() {
                    //     this.x = 0;
                    //     this.y = 0;
                    // }    
                    // // superclass method
                    // Shape.prototype.move = function(x, y) {
                    //     this.x += x;
                    //     this.y += y;
                    //     alert('Shape moved.');
                    // };    
                    // // Rectangle - subclass
                    // function Rectangle() {
                    //     Shape.call(this); // call super constructor.
                    // }    
                    // // subclass extends superclass
                    // Rectangle.prototype = Object.create(Shape.prototype);
                    // Rectangle.prototype.constructor = Rectangle;
                    // var rect = new Rectangle();
                    // alert('Is rect an instance of Rectangle? ' + (rect instanceof Rectangle));// true
                    // alert('Is rect an instance of Shape? ' + (rect instanceof Shape));// true
                    // rect.move(1, 1); // Outputs, 'Shape moved.'
                    
                    //----------------------------------------------------------------------------- 4-3 closures or thunk
                    // function registerFootball(gender) {
                    //     return function(name) {
                    //         if(gender == "m")
                    //             return "Mr." + name;
                    //         if(gender = "f")
                    //             return "Mrs." + name;
                    //          };
                    //     }
                //     
                //     var x = registerFootball("m");
                //     alert(x("ferdos")); 
                //     alert(x("zakeri"));     
                //     var y = registerFootball("f");                        
                //     alert(y("ghandfrooshan")); 
                //     alert(y("pour mohammad"));
                    
                     //var counter = (function() {
                     //                    var privateCounter = 0;
                     //                    function changeBy(val) {
                     //                        privateCounter += val;
                     //                    }
                     //                    return {
                     //                        increment: function() {
                     //                        changeBy(1);
                     //                        },
                     //                        decrement: function() {
                     //                        changeBy(-1);
                     //                        },
                     //                        value: function() {
                     //                        return privateCounter;
                     //                        }
                     //                    };   
                     //                })();                    
                     //alert(counter.value()); 
                     //counter.increment();
                     //counter.increment();
                     //alert(counter.value()); 
                     //counter.decrement();
                     //alert(counter.value()); 
                    
                    //------------------------------------------------------------------------------ 4-4 getter setter
                     //var o = {
                     //a: 7,
                     //get b() { return this.a + 1; },
                     //set c(x) { this.a = x / 2;}
                     //};                    
                     //alert(o.b);
                     //o.c = 4;
                     //alert(o.c);//undefined
                     //alert(o.b);
                     //alert(o.a);
                    
                    //----------------------------------------------------------------------------- 4-5 typeof, instanceOf
                     //alert(typeof 'example string');
                     
                     //function Tree(name) {
                     //    this.name = name;
                     //}
                     //var o = new Tree("MyTree");
                     //alert(o instanceof Tree);
                     //alert(typeof o);
                    
                    //----------------------------------------------------------------------------- 4-6 polymorphism
                     //function Class1(cl)
                     //{
                     //    this.cl = cl;
                     //}
                     //var cl1 = new Class1("Ferdos") 
                         
                     //alert(cl1.toString());
                     //cl1.toString = function () {return  this.cl + "Hi"};
                     //alert(cl1.toString());       
                    
                    //------------------------------------------------------------------------------ 4-7 json
                     //var obj = JSON.parse('{"1": 1, "2": 2, "3": {"4": 4, "5": {"6": 6}}}', function(k, v) {
                     //    alert(k); 
                     //    return v;    
                     //});         
                     //alert(obj["1"]);
                    
                     var foo = {foundation: "Mozilla", model: "box", week: 45, transport: "car", month: 7};
                     var jsonString = JSON.stringify(foo);
                     alert(jsonString);
            }
        </script>
    </body>
</html>
