
in schema!!!
req/import krlo mongoose then!!!

const userSchema = new mongoose.schema({
field1 : {},
field2 : {
},

<mark style="background: #FFB86CA6;">
eg: 

mobile : {
type : String, 
required : true
}
</mark>

def export  = mongoose.model("user", userSchema);

timeStamps:true -> by default its "FALSE")

const userData = new userSchema



<span style="color:rgb(100,200,300)">in next file </span> 
const *user* = req('./models/userModel')  => => (dir/fileName)
using schema ->>
*const createUser* = asnc () => {
const usr = new *user*({
name : "batman",
email : "wfwefararg@gamil.com",
mobile : "123423"
});

const userData  = await *user*.save() <-- this will save data in mongo!!!
}

*createUser();*

console.log(userData)!!! 