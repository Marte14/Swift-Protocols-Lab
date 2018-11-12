
## Protocols Lab


Question 1.

'''Swift

class Human : CustomStringConvertible, Equatable, Comparable{

var description: String {
return "Person\'s name is \(name) and their age is \(age)"
}

var name : String
var age : Int

init(name: String, age: Int){
self.name = name
self.age = age

}
static func == (lhs: Human, rhs: Human)-> Bool {
return lhs.name == rhs.name  && lhs.age == rhs.age

}
static func < (lhs: Human, rhs: Human) -> Bool {
return lhs.age < rhs.age
}

// print("\(name) is \(age) years young")
}

var People : [Human] = []
let latty = Human(name: "Latty", age: 24)
let lanyAlso = Human(name:"Lany", age : 10)
let lany = Human(name: "Lany" , age : 10)
let gordon = Human(name: "Gordon" , age : 34)
let john = Human(name: "John", age: 26)
let katty = Human(name: "katty", age: 23)

People.append(latty)
People.append(lanyAlso)
People.append(lany)
People.append(gordon)
People.append(john)

if john == katty {
print("They are the same person")
}else{
print("They are different persons")
}

let sortedByAge = [john, katty].sorted { $0 < $1 }


'''

Question 2. 
Create a protocol called Vehicle with two requirements: a nonsettable numberOfWheels property of
type Int, and a function called drive().

Define a Car struct that implements the Vehicle protocol. numberOfWheels should return a value of 4,
and drive() should print "Vroom, vroom!" Create an instance of Car, print its number of wheels, 
then call drive().

Define a Bike struct that implements the Vehicle protocol. numberOfWheels should return a value of 2,
and drive() should print "Begin pedaling!". Create an instance of Bike, print its number of wheels,
then call drive().






Question 3. 
// Given the below two protocols, create a struct for penguin(a flightless bird) and an eagle.
Give your structs some properties and have them conform to the appropriate protocols.

protocol Bird {
 var name: String { get }
 var canFly: Bool { get }
}

protocol Flyable {
 var airspeedVelocity: Double { get }
}






Question 4. 
// Create a protocol called Transformation

// create a mutating method called transform

// Make an enum called SuperHero (have it conform to Transformation) and an instance of it named
bruceBanner. Make it so that when the transform function is called that bruceBanner turns from 
.notHulk to .hulk.

enum SuperHero: Transformation {
    // write code here.
}

Example Output: 
var bruceBanner = SuperHero.notHulk

bruceBanner.transform() . // hulk

bruceBanner.transform()  // notHulk
</pre> 

</br> </br> 

<pre>
Question 5. 
// 1. Create a protocol called Communication

// 2. Give it a property called talk, of type String, and assign it an explicit getter.

// 3. Create three Classes. Cow, Dog, Cat.

// 4. Have your three classes conform to Communication

// 5. talk should return a unique message for each animal when talk is called.

// 6. Put an instance of each of your Classes in an array.

// 7. Iterate over the array and have them print talk.
</pre> 


