- 👋 Hi, I’m @pasawonOfPark
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
pasawonOfPark/pasawonOfPark is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
//-------ค่าตัวแปล ตัวหนังสือ ตัวเลขทศนิยม ตัวเลขจำนวนเต็ม ------

let name: String = "pasawon"
let dateOfBrith: String = "25/12/2547"
let gender: String = "male"

var weiht: Double = 79.0
var height: Double = 179.0

var occpation: String = "student"
var salary: Int = 34500

var statusOfMember: Bool = true 

//----------Array------------ เพิ่ม ลบ แทนที่ ตำแหน่งในอาเร-------

var friend: [String] = ["Anne","kery","keith"]
print(friend)
print(friend.count)

print(friend[1])
print(friend[0])

friend[1] = "paul"
print(friend) 

friend.append("joe")
print(friend)

friend.insert("bob", at: 1)
print(friend)

friend.remove(at:2)
print(friend)

friend.removeAll()
print(friend)

//--------------------- ฟังชั่นต่างๆทางคณิตศาต ต้องอิพอต import Foundation ทุกครั้งตอรใช้ -------------------------

import Foundation

let firstScore: Int = 52
let secondScroe: Int = 24
let thirdScore: Int = 35

var totalScroe = firstScore + secondScroe + thirdScore
print(totalScroe)

var diffScore = firstScore - secondScroe
print(diffScore)

var powerScore = firstScore * 2
print(powerScore)

var myScore = Double(thirdScore) / 4
print(myScore)

var modScore = thirdScore % 4
print(modScore)

let myDouble: Double = -10.75
print(round(myDouble))
print(floor(myDouble))
print(ceil(myDouble))
print(abs(myDouble))
`
var myMesssage: String =  "Hello" + " ," + "my name is "
var myName: String = "Park"
myMesssage = myMesssage + myName
print(myMesssage)


let fristName = "pasawon"
let city = "pathum thani"

let welcomeMessage: String = "Hello \(fristName), wellcome to \(city)" 
print(welcomeMessage)

///------ สูตรคำนวณพื้นที่สามเหลี่ยม ------///
import Foundation

print("กำหนดความยาวฐานของสามเหลี่ยม:")
var base = readLine()!

print("กำหนดความสูงของสามเหลี่ยม")
var height = readLine()!

var area = 0.5 * Double(base)! * Double(height)!
print("พื้นที่สามเหลี่ยม: \(area)")

///------ สูตรคำนวณ หารค่าอาหาร ------///
import Foundation


print("จำนวนค่าอาหาร: ")
var billTotal = readLine()!

print("จำนวนคนที่จ่าย: ")
var numOfPeople = readLine()!

print("ทิปให้พนักงาน(%): ")
var tip = readLine()!

var tip_amount = Double(billTotal)! * Double(tip)! / 100
var totalPayment = Double(billTotal)! + tip_amount


var split = Double(totalPayment) / Double(numOfPeople)!
print("จำนวนเงินที่แต่ละคนต้องจ่าย: \(split) ")




