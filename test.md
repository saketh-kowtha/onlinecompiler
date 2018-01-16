# API's
**1.compile**			
		```javascript
		var payload  = {
			code : string,
			filename : string,
			input : string,
			extension : string
		}
		var Response = {
			STDOUTPUT : string,
			Error : string,
			STDERROR : string
		}
		```

**2.Login**
		```javascript
		var payload  = {
			username : string,
			Password
		}
		var Response = {
			status : Boolean
		}
		```

**3.Register**
		```Javascript
		var payload  =  {
			Username : string,
			Password : string,
			Gmail : string
		}
		var Response =  {
			status : Boolean
		}
		```

**4.Verfication**
		```Javascript
		var payload  =  {
			OTP : number
		}
		var Response =  {
			status : Boolean
		}
		```

**5.New File**
		```Javascript
		var payload  =  {
			Filename : string,
			Content : string
		}
		var Response =  {
			status : Boolean
		}
		```

**6.Delete File**
		```Javascript
		var payload  =  {
			Filename_or_Folder : string
		}
		var Response =  {
			status : Boolean
		}
		```

**7.Save File**
		```Javascript
		var payload  =  {
			File_or_Folder : string
		}
		var Response =  {
			status : Boolean
		}
		```

**8.Getting Content**
		```Javascript
		var payload  =  {
			Filename : string
		}
		var Response =  {
			data : string
		}
		```

**9.Getiing Files List**
		```Javascript
		var payload  =  {
			user : string
		}
		var Response =  {
			data : Array string
		}
		```

**10.Share**
		```Javascript
		var payload  =  null
		var Response =  {
			data: string
		}
		```

**11.Delete session**
		```Javascript
		var Request  =  {
			user : string,
			session_id : string
		}
		var Response =  {
			status : Boolean
		}
		```

# Functions
**1.Compile**
		```Javascript
		compile_validation = (filename, content, input) =>{
			return Boolean
		}
		(compile_validation)? Backend_API(1) : alert(message)
		```

**2.Login**
		```JAvascript
		user_Validation = (uname,Passwd,email = False) =>{ 							
			return  Boolean
		}
		(user_validation)? Backend_API(2) : alert(message)
		```

**3.Register**
		```Javascript
		user_validation = (uname,Passwd,email) =>{ 									
			return  Boolean
		}
		(user_validation)? Backend_API(3) : alert(message)
		```

**4.OTP**
		```Javascript
		otp_Validation = (Otp) =>{
			return Boolean
		}
		(otp_validation)? Backend_API(4) : alert(message)
		```

**5.NewFile**
		```Javascript
		file_validation = (filename, content) => {
			return Boolean
		}
		(newfile_validation) ? Backend_API(5) : alert(message)
		```

**6.DeleteFile**
		```Javascript
		file_exist_validation = (filename) =>{
			return Boolean
		}
		(file_exist_validation) ? Backend_API(6) : alert(message)
		```

**7.Save File**
		```Javascript
		file_exist_validation = (filename) =>{
			return Boolean
		}
		(file_exist_validation) ? Backend_API(7) : alert(message)
		```

**8.Get content**
		```Javascript
		get_file_content = (filename) =>{
			return string
		}
		(get_file_content) ? Backend_API(8) : alert(message)
		```

**9.Get Files List**
		```Javascript
		get_dir_list = (dir_name) =>{
			return Array string
		}
		(get_dir_list) ? Backend_API(9) : alert(message)
		```

**10.Get Share Details**
		```Javascript
		return Backend_API(10)
		```

**11.Pop Up Save Or Delete**
		```Javascript
		var user_ip = prompt("Do you Want to Save your Session Y/N")
		if(user_ip == "Y")
			alert(message)
		else
			Backend_API(11)
			```
**12.alert**
	```Javascript
		alert = (message) =>{
			show messahe
		}
		```


NOTE:
=====
+ When user registered we have to create one folder with `USERNAME` in Server.
+ When user logged in give one `random 15 chars string` as session name and create folder with that name in user folder
+ When user logged in show all the files located in user folder
+ when user logged in show one default file
+ When user clicks `Run` button or `Save` Button then save the current file in server
+ When user chooses `save session` option or clicks `Share button` then provide him a folder or file URL
+ If user chooses `Delete session` option then delete entire session folder
+ When user runs the program check whether Input all details are entered or not if not entered then ask him for conformation

Technical Info:
===============
```
	payload  -> Api Request
	Response -> Api Response
	API calls Session has details about API we are calling them from Client side and we get Response from Server
	Front end Functions are the functions using in client side
	Back end Functions are the functions using in server side
```
