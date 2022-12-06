- how we can catch the file from respose ? 1-from body 2-from hrader 3-from formDate
- from where we send the files ? from client side or serve side
- where we save the files thet we catch in server app first ? 1-temp file 2-database 3-all above
- what client side need to show up the file ? we need the fullpath for file that we save on database and temp file or S3
- how we send multible files from client side ?
- what is the deffrince between single and array on multer , and when we use each one?
- what is body-parser used for ?
- in any file we can check if we install the pakeges or not ? pakage json file and see if the pakege adde in dependencies or not
- how can we require multer pakeges or any pakages and use it in our project ? requier('multter)
- where we shold use body-parser , after the app or before and why ?
- colud we use another way in express to parse data insted install body-parse pakege , what this way ?
- is multter an express midlewhere and what thats mean ?
- what is FormData interface used for ? and how we can append data to it ?
- how can we send multible file from client side ?
- in header request what we sould send when we send files ?
- why we send some data with header request ?
- why we send application/json on header when we send requset to server ?
- look at the below code and answer the qustion
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
	
* why we use single insted of array ?
* why we write upload.single('file') after '/api' and what does this  mean ?
* did we send response if we have an error in multer storge progress ?
* how can we accses the file from req ? by calling req.files ?
* where will data store in disk or memory ?
- Each file contains the following information : destination , filename , path , originalname ,size ,fieldname
* explain what each one means
* waht is the deffrence between filename and originalname and fieldname
* from each one we can Determine the folder to which the file has been saved in
- what fileFilter used for in multer ?
- is fileFilter work before or after storage files ?
- who can we detrimine if we have valid file to save ?
- what we shold do if we have not valid file in fileFilter ? return cb(with false)
- what shold pass to callback function to accept the file
- what shold pass to callback function to reject the file
- each file have mimetype element , how can use mimetype by chiking on file type ?
- What is multer used for?
- Can we use multer without Express?
- can we upload pdf file with multer ?
- where multer save files on requeset ?
- what type of input we need to deling with files ?
- is multter a express midlewhere ?
- What is the different between multer.memoryStorage and multer.diskStorage
- how we get directory name of the current module ?
- how we get fullpath for specific file ?
- shold we use get http method to send files if not what shold we use and why ?
