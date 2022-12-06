# Handle-Files Qustions

- how can we catch the file from response? 1-from body 2-from header 3-from formDate
- from where do we send the files? 1-from the client side 2-from serve side
- where do we save the files that we catch in the server app first? 1-temp file 2-database 3-all above
- what client side needs to show files? we need the full path for the file that we save on the database and the temp file or S3
- how do we send multiple files from the client side ?
- what is the difference between single and array on multer, and when do we use each one?
- what is a body-parser used for?
- in any file can we check if we install the packages or not? 
- how can we require multer package or any packages and use it in our project? 
- where we should use body-parser, after the app, or before and why?
- could we use another way in express to parse data instead install a body-parse package, what this way?
- is multter an express middleware and what does that mean?
- what is FormData interface used for? and how we can append data to it?
- how can we send multiple files from the client side?
- in the header request what we should send when we send files?
- why do we send some data with header request ?
- why do we send application/json on the header when we send the requset to server?
- look at the below code and answer the question
```js
	const storage = multer.diskStorage({
	  destination: function (req, file, cb) {
	    cb(null, '/tmp/my-uploads')
	  },
	  filename: function (req, file, cb) {
	    const uniqueSuffix = Date.now() + '-' + Math.round(Math.random() * 1E9)
	    cb(null, file.fieldname + '-' + uniqueSuffix)
	  }
	})
	const upload = multer({ storage: storage })
	
	app.post('/api' , upload.single('file') , (req,res) =>{
		res.send('filed saved')
	}
```
- look at the above code and answer the questions
        -why do we use single instead of array?
	- why do we write upload.single('file') after '/api' and what does this mean?
	- did we send a response if we have an error in multer storge progress?
	- How can we access the file from req ? by calling req.files?
	- where will data be stored in disk or memory?
- Each file contains the following information: destination , filename, path, originalname , size , fieldname
	- explain what each one means
	- what is the difference between filename and originalname and fieldname?
	- from each one we can Determine the folder to which the file has been saved in?
	- 
- what fileFilter used for in multer?
- is fileFilter work before or after storage files?
- who can we determine if we have a valid file to save?
- what we should do if we have not a valid file in fileFilter ? return cb(with false)
- what should pass to the callback function to accept the file
- what should pass to the callback function to reject the file
- each file has mimetype element, how can use mimetype by checking on the file type?
- What is multer used for?
- Can we use multer without Express?
- can we upload pdf file with multer ?
- where multer save files on requeset?
- what type of input do we need to deal with files ?
- is multter an express midlewhere?
- What is the difference between multer.memoryStorage and multer.diskStorage
- how do we get the directory name of the current module?
- how do we get fullpath for specific file?
- Should we use get HTTP method to send files if not what should we use and why?
