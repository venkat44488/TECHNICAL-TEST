**Challenge1:**
In general terms a 3-teir environments runs with WebSphere application server in the central  hub. It runs with 
1.	IBM AIX servers as physical middle-tier 
2.	IBM Z systems which is virtual middle tier.
In both cases web clients will be used as standard web browsers to communicate with an application that is based on WebSphere application server or physical or virtual sever. 
Web application that build on top of servlets /JSPs, JSTL, structs, EJBs send request to through Java beans to access data and carry response back to web server.
An example of a 3-tier implementation might be a Java servlet running on the Web Application Server (WebSphere/WebLogic) that provides access to Database. The servlet might allow regular customers send requests over the Internet, using the required security layers.
 
**Challenge2.**

	We can retrieve AWS ec2 instance metadata using curl command and 169.254.169.254 IP. These works on any cloud.
1.	Curl http:// 169.254.169.254/latest/metadata/  this prints complete data about ec2 instance. 
2.	Curl http:// 169.254.169.254/latest/user-data/ prints userdata.
3.	Curl http:// 169.254.169.254/latest/metadata/public-ipv4  prints IP address of that instance.


Note: the same command works with OpenStack, AWS,Azure and Google Cloud as well.

**Challenge3:**

**Example 1**
object1 = {'a':{'b':{'c':'d'}}}
for x,y in object1.items():
   for i,j in y.items():
       for a,b in j.items():
        print(x,"/",i,"/",a)
        print(b)
	
**Example2**
Object2 = {'x':{'y':{'z':'a'}}}
for x,y in object2.items():
   for i,j in y.items():
       for a,b in j.items():
        print(x,"/",i,"/",a)
        print(b)



