การเขียนโปรแกรมภาษา Swift ด้วย Replit 

//-------ค่าตัวแปล ตัวหนังสือ ตัวเลขทศนิยม ตัวเลขจำนวนเต็ม ------

let name: String = "pasawon"
let dateOfBrith: String = "25/12/2547"
let gender: String = "male"

var weiht: Double = 79.0
var height: Double = 179.0

var occpation: String = "student"
var salary: Int = 34500

var statusOfMember: Bool = true 


//----------Array------------ เพิ่ม.append  ลบ.remove ลบทั้งหมด.removeAll แทนที่.insert ตำแหน่งในอาเร-------

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


///------ ค่าทางตะกะ ------///
import Foundation

var a = 5
var b = 3

print("a == b" , a == b )
print("a != b" , a != b )
print("a < b " , a < b )
print("a <= b" , a <= b )
print("a >= b" , a >= b )


///------ if else ------///

import Foundation

let temperlature = 80

if temperlature >= 100{
  print("น้ำเดือด")
} else{
  print("น้ำไม่เดือด")
}

(temperlature >= 100) ? print("น้ำเดือด") : print("น้ำไม่เดือด")



///------ if - else if   ------///
import Foundation


var finishPossition = 2

if finishPossition == 1{
  print("คุณได้เหรียนทอง")
}else if finishPossition == 2{
  print("คุณได้เหรียนเงิน")
}else if finishPossition == 3{
  print("คุณได้เหรียนทองแดง")
}else{
  print("คุณไม่ได้รางวัล")
}


///------ switch case   ------///

switch finishPossition{
  case 1:
  print("คุณได้เหรียนทอง")  
   case 2: 
  print("คุณได้เหรียนเงิน")
  case 3:
  print("คุณได้เหรียนทองแดง")
  default:
  print("คุณไม่ได้รางวัล")
}


///------ switch case  ex2 ------///
import Foundation

let approximateCount = 24
let countedThings = "moons orbiting the planet"
let naturalCount = String

switch approximateCount{
  case 0:
    naturalCount = "no"
  case 1...5:
    naturalCount = "a few"
  case 6...12:
    naturalCount = "several"
  case 13..<100:
    naturalCount = "dozens of"
  case 100..<1000:
    naturalCount = "hundreds of"
  default:
    naturalCount = "many"
}
print("There are \(naturalCount) \(countedThings).")






