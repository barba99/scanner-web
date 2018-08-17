#!/usr/bin/env python
from urllib2 import *
from platform import system
import sys
def clear():
    if system() == 'Linux':
        os.system("clear")
    if system() == 'Windows':
        os.system('cls')
        os.system('color a')
    else:
        pass
def slowprint(s):
    for c in s + '\n':
        sys.stdout.write(c)
        sys.stdout.flush()
        time.sleep(4. / 100)
banner = '''
                   ,                \033[96m
                   |'.             ,
                   |  '-._        / )
                 .'  .._  ',     /_'-,
                '   /  _'.'_\   /._)') \033[91m
               :   /  '_' '_'  /  _.'
               |E |   |Q| |Q| /   /
              .'  _\  '-' '-'    /
            .'--.(S     ,__` )  /    
                  '-.     _.'  /      \033[92m
                __.--'----(   /     
            _.-'     :   __\ /
           (      __.' :'  :Y
            '.   '._,  :   :|        \033[96m
              '.     ) :.__:|      
                \    \______/
                 '._L/_H____]                                                                                          
======= Script Name: scanner-web =======\033[91m
======= edición By: JORGE BARBA ==================\033[92m
======= @Jorge_Barba  - el conocimiento libre ====\033[96m
'''
print banner
def menu():
   print'''
\033[91m 1 \033[92m)\033[96m DNS Lookup

\033[91m 2 \033[92m)\033[96m Whois Lookup

\033[91m 3 \033[92m)\033[96m Reverse IP Lookup

\033[91m 4 \033[92m)\033[96m GeoIP Lookup

\033[91m 5 \033[92m)\033[96m Subnet Lookup

\033[91m 6 \033[92m)\033[96m Port Scanner

\033[91m 7 \033[92m)\033[96m Extract Links 

\033[91m 8 \033[92m)\033[96m Zone Transfer

\033[91m 9 \033[92m)\033[96m HTTP Header

\033[91m 10\033[92m)\033[96m Host Finder

\033[91m 11\033[92m)\033[96m About o Info!!!

\033[91m 0 \033[92m)\033[96m Exit
'''
slowprint("\033[1;91mEsto es un simple script By Real Strategy " + "\n Let's Start")

menu()
def ext():
    ex = raw_input ('\033[92mContinue/Exit -=[C/E]=- -> ')
    if ex[0].upper() == 'E' :
           print 'Exiting!!!'
           exit()
    else:
           clear()
           print banner
           menu()
           select()

def  select():
  try:
    joker = input("\033[96mEnter \033[92m0/\033[91m11 -> ->  ")
    if joker == 2:
      dz = raw_input('\033[91mEnter IP Address : \033[91m')
      whois = "http://api.hackertarget.com/whois/?q=" + dz
      dev = urlopen(whois).read()
      print (dev)
      ext()
    elif joker == 3:
      dz = raw_input('\033[92mEnter IP Address : \033[92m')
      revrse = "http://api.hackertarget.com/reverseiplookup/?q=" + dz
      lookup = urlopen(revrse).read()
      print (lookup)
      ext()
    elif joker == 1:
      dz = raw_input('\033[96mEntre Your Domain :\033[96m')
      dns = "http://api.hackertarget.com/dnslookup/?q=" + dz
      joker = urlopen(dns).read()
      print (joker)
      ext()
    elif joker == 4:
      dz = raw_input('\033[91mEnter IP Address : \033[91m')
      geo = "http://api.hackertarget.com/geoip/?q=" + dz
      ip = urlopen(geo).read()
      print (ip)
      ext()
    elif joker == 5:
      dz = raw_input('\033[92mEnter IP Address : \033[92m')
      sub = "http://api.hackertarget.com/subnetcalc/?q=" + dz
      net = urlopen(sub).read()
      print (net)
      ext()
    elif joker == 6:
      dz = raw_input('\033[96mEnter IP Address : \033[96m')
      port = "http://api.hackertarget.com/nmap/?q=" + dz
      scan = urlopen(port).read()
      print (scan)
      ext()
    elif joker == 7:
      dz = raw_input('\033[91mEntre Your Domain :\033[91m')
      get = "https://api.hackertarget.com/pagelinks/?q=" + dz
      page = urlopen(get).read()
      print(page)
      ext()
    elif joker == 8:
      dz = raw_input('\033[92mEntre Your Domain :\033[92m')
      zon = "http://api.hackertarget.com/zonetransfer/?q=" + dz
      tran = urlopen(zon).read()
      print (tran)
      ext()
    elif joker == 9:
      dz = raw_input('\033[96mEntre Your Domain :\033[96m')
      hea = "http://api.hackertarget.com/httpheaders/?q=" + dz
      der =  urlopen(hea).read()
      print (der)
      ext()
    elif joker == 10:
      dz = raw_input('\033[91mEntre Your Domain :\033[91m')
      host = "http://api.hackertarget.com/hostsearch/?q=" + dz
      finder = urlopen(host).read()
      print (finder)
      ext()
    elif joker == 11:
      slowprint("Script Name :  scanner-web \033[92m")
      slowprint(".....................")
      slowprint("edición: JORGE BARBA \033[96m")
      slowprint(".........................")
      slowprint("TELEGRAM : @Jorge_Barba \033[91m")
      slowprint("............................"
      slowprint("Github : https://github.com/barba99   \033[92m")
      slowprint(".........................................")
      slowprint("YOUTUBE :https://www.youtube.com/channel/UCXXRtv7G43pc-yTkGQwUQNQ  \033[96m")
      slowprint("........................................................")
      slowprint("facebook fan page: https://www.facebook.com/Http-inyector-and-custom-138324883422250 \033[91m")
      slowprint("..........................................................")
      slowprint("MENSAJE: El conocimiento es libre\033[96m ")
      slowprint("................................................................... ")
      ext() 
    elif joker == 0:
      print "Exiting!!"
      ext()
  except(KeyboardInterrupt):
    print "\nCtrl + C -> Exiting!!"
select()
