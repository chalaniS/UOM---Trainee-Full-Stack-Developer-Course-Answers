fhandle1 = open("file1.txt","r")
fhandle2 = open("file2.txt","w")

str = fhandle1.readline()
fhandle2.write(str)
str = fhandle1.readline()
fhandle2.write(str)

fhandle1.close()
fhandle2.close()

fhandle3 = open("file2.txt")
print(fhandle3.read())
fhandle3.close()