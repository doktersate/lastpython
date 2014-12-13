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
