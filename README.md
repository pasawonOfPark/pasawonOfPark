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

///------ if else แบบ case switch ex2 ------///

import Foundation
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


///------ วนลูปแบบนับจำนวนยอด ------///
import Foundation

for i in 1...5{
print("this is \(i)")
}  

let name = ["kunk","looknam","Cathy"]
for name in name{
  print("Hello! \(name)")
}

///------ วนลูปแบบเช็คเงื่อนไข ------///

var myLevel: Int = 0
var finalLevel: Int = 5

while(myLevel <= finalLevel){
  print("you have play in level \(myLevel)")
  // myLevel = myLevel + 1
  myLevel += 1
  
}
print("outside of while loop")


///------ วนลูปแบบเช็คเงื่อนไข ------///

var items: Int = 0
var totalPrice: Double = 0.0 
var discount: Double = 0.0 
var netPrice: Double = 0.0

print("จำนวนสินค้า:")
items = Int(readLine()!)!

//หาราคารวมสินค้า
for i in 1...items{
  print("ราคาสินค้าชิ่นที่ \(i):")  
  let productPrice = Double(readLine()!)!
  totalPrice = totalPrice + productPrice 
}

//คำนวนส่วนลด
if totalPrice >= 1000 {
  discount = totalPrice * 0.1
} else {
discount = 0.0
}

//คำนวนราคาสุทธิ
netPrice = totalPrice - discount
print("ยอดสินค้ารวม: \(totalPrice) บาท")
print("ส่วนลด: \(discount) บาท")
print("ยอดสุทธิ: \(netPrice) บาท")

print("จำนวนที่เงินชำระสินค้า")
var payment = Double(readLine()!)!

var change = payment - netPrice
print("รับจำนวนเงิน: \(payment) บาท")
print("เงินทอน: \(change) บาท")


------------------------------------ เทส
var items: Int = 0
var total: Double = 0
var discount: Double = 0
var netPrice: Double = 0

print("จำนวนสินค้า")
items = Int(readLine()!)!

for i in 1...items{
  print("ราคาสินค้าต่อชิ้น")
  var price = Double(readLine()!)!
  total = total + price
}
  
if total >= 1000{
  discount = total * 0.1
}else{
  discount = 0
}

netPrice = total - discount
print("ราคาสินค้า = \(total)")
print("ส่วนลด = \(discount)")
print("ราคราคาสุทธิ = \(netPrice)")

print("เงินที่ลูกค้าชำระ" )
var payment = Double(readLine()!)!

print("เงินทอน = \(payment - netPrice)") 

//----การใช้คำสั่งฟังชั่น----//
import Foundation

func displaypi(){
  print("3.14")
}

displaypi()

func triple(value: Int){
  let result = value * 3
  print("If you multiply \(value) by 3, you'll get \(result).")
}

triple(value: 10)

func sayHello(to: String, and: String){
  print("Hello \(to) and \(and)")
}
sayHello(to:"pasawon", and:"bootsuwon")

func sayHelloAgine(to name: String, and anotherName: String){
  print("Hello \(name) and \(anotherName)")
}
sayHelloAgine(to: "park", and: "bootsuwon")


