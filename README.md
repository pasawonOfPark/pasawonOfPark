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

let name: String = "pasawon"
let dateOfBrith: String = "25/12/2547"
let gender: String = "male"

var weiht: Double = 79.0
var height: Double = 179.0

var occpation: String = "student"
var salary: Int = 34500

var statusOfMember: Bool = true 

//----------Array------------

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
