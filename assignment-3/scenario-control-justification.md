Nature of your overall scenario design strategy and scenario control location policy: either
distributed in a roundabout manner, distributed in a principal-object-rooted manner,
centralized in the UI or scenario modules, or centralized in principle object modules. Why
did you choose this architecture?


The scenario design strategy that will be used is the principal-object method. This method 
was selected since the principal object knows best what information it requires to complete  
the scenario it is in. Considering this, having the principal object initiate and control the 
calls to the other modules seemed like a logical decision. 



Inline value classes are a feature of Kotlin which allow you to represent 
a single value as a domain specific type and take advantage of the optimization 
done by the compiler on those types. An example of inline value classes are 
```
value class RGBValue(val intensity: Int) {
init {
    require(intensity in 0..255) {
    "RGB value must be in [0, 255]"
    }
   }
}

fun RGBTripletToColor(redIntensity: RGBValue,
                      blueIntensity: RGBValue,
                      greenIntensity: RGBValue): String {
                      .....
}
```

By defining `RGBValue`, the intention of using only RGB values in the function becomes 
clearer. Furthermore, if we had rewritten `RGBTriple` to be instead

```
fun RGBTripletToColor(redIntensity: Int,
                      blueIntensity: Int,
                      greenIntensity: Int): String {
                        .....
}
```

our intent of only taking RGB values is not as clear.

Furthermore, the ... operator takes two numbers, A, and B, and returns all the numbers in [A, B]. 



DescribeSpec is a testing style which wraps scenarios to be tested in the `describe` keyword 
and tests within the `it` keyword. An example is shown below.

```
class EmailTest : DescribeSpec({
                    describe("isValidEmail") {
                        describe("When email is blank") {
                            it("Returns false") {
                                Test goes here
                            }
                        }
                        describe("When email does not contain @") {
                            it("Returns false") {
                                Test goes here
                                }
                            }    
                        }    
                        ......
                        
                    })    
```

The first use of `describe` denotes the function being tested, while further uses of 
`describe` clarify what scenario is being tested. The `it` keyword is used to 
denote the expected result of the test.