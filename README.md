import urllib2 import time

def WebData(): timeT = 0 length = '' while timeT < 5: URL = urllib2.urlopen('http://www.ign.com') data = URL.read() datastring = str(data) lengthA = len(datastring)

            print (lengthA)
            if length8 != '' and lengthA != length8:
                    print ("This website has been updated")
                    return
            else:
                    length8 = lengthA
            timeT += 1
            time.sleep(5)
WebData()
