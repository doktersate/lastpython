lastpython
==========
def getlist(c,ifile,ofile):
    for aline in ifile:
        if aline[0] == c:
            ofile.write(aline)

def getreverseelist(c,ifile,ofile):
    for aline in ifile:
        if aline[len(aline)-3] == c:
            ofile.write(aline)

mf1 = open("words.txt","r")
mf2 = open("blist.txt","w")

Chapter 5
***
rainfile = open("rainfall.txt","r")

for aline in rainfile:
    values = aline.split()
    print(values[0], "had", values[1], "inches of rain.")
***

rainfile = open("rainfall.txt","r")
outfile = open("rainfallInCM.txt","w")

for aline in rainfile:
    values = aline.split()
    
    inches = float(values[1])
    cm = 2.54 * inches
    
    outfile.write(values[0]+" "+str(cm)+"\n")

rainfile.close()
outfile.close()
***


    
    
