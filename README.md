# LAB-14
REGULAR EXPRESSION
import re
banyak = int(input("Masukkan banyaknya kartu kredit : "))

for i in range (banyak) :
    nomor = input("Masukkan nomor togel : ")
    a = re.findall("^[456]",nomor)
    b = re.findall("\s",nomor)
    c = re.findall("-",nomor)
    d = re.split("-",nomor)

    if (a) :
        if (c) :
            for i in d :
                if len (i) == 4 :
                 print("valid")
                break
            else :
                print("invalid")
                break
        elif (len(nomor)==16) :
            print("valid")
        else :
            print("invalid")
    elif (b) :
            print("invalid")
            
