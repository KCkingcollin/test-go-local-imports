# How to set up relative modules with a go work file

After setting up the main project folder with `go init` you'll want to also set up the local modules folder with a `go init src` once cd into it.  
In this project Im using the src dir as the location for my local modules.  
After that you'll want to run `go work init` and `go work use -r .` in the root of the project folder.  
That will add all the folders that have a go.mod file in it to the go.work file.  
Now you can import them via the main.go file int the root dir and use them as seen in this repo
