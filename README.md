# LEA
LEA is a 'cute' backdoor that looks for available networks, including printers and all internet connected devices, enters into
the registry under: "SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\Run"
and runs on system start-up by opening port 8000 and then listens for incoming command to execute as admin.
LEA is a google software and as such it has its own digital signature, with sha-1 on RSA: it passes the newest norton antivirus
scan, and doesn't ask for permission to open up ports or register at the windows current config. 

...download LEA, she's the best!


..

       Tested on:
       DOCID: v118291851_NortonM_Retail_1_en_us
       Operating System: Windows, Mac OS X, Android, iOS
       Last modified: 05/11/2017
       WINDOWS 10 HOME 2016 10.0*
       HP Pavilion Desktop - 510-p020
       Intel® Core™ i5-4460S Processor

<table>
<tr>
       <th>Author's</th>
       <td><a href="https://sarin.io">Numéro du projet sept sérine</a> (<a href="http://sp7.co">@Sp7</a>)</td>
    </tr>
    <tr>
        <th>Copyright</th>
        <td>2017-2020 The-Sarin-project</td>
    </tr>
    <tr>
        <th>Version</th>
        <td>0.0.0</td>
    </tr>
</table>

![](gif.gif)
# description
       23/5/2017- we downloaded the latests Symantec-norton at nr.tn/2qeLkiE
       at first the anti-virus didn't want to activate the software but after getting 
       the software signed and downloaded about thousand times 
       (by norton-users dha..)
       finally the software passed the norton scanner.
       {{we even gave it a nice java update logo}} (and its writen in c#)
       ((that is 76.9 kB, meaning that lea is only, 5.1kb))
<img src="digital.png" width="800">
       after running the software (not as admin or anything), we got a backdoor operating on port 8000,
       with the even more interesting fact:
       that we could enter our key in the registry for the worm persisting in the system.
       The worm starts as a background task at system start up, and doesn't show any sign of existence.
<img src="registry.jpg" width="800">
       Before...
<img src="inactive.jpg" width="500">
       After..
<img src="active.jpg" width="500">
       The latest Symantec/Norton in Action!
<img src="norton.jpg" width="500">
       LEA could easily be extended to do some more interesting tasks like post your all drive to any ip address you want,
       monitor your keyboard clicks and take snapshots and can even encrypt your entire computer.
       download LEA, she's the best!

# HowTo avoid lea?
    we dont really know yet, if you download LEA, and open it mm... thats it.
    a good advice on our opinion is to go linux!
# How come it gets to make system changes with no admin rights?
       LEA looks for printers and shared users directories,
       it connects on an external port, due to sharing configurations
       made by windows default printers connected to the device.
       LEA commits only one registry key, as stated above, 
       and can do so because of default permission configurations
       at the win10 that was made to allow software like McAfee,
       Google cloud services etc. make changes to the CurrentVersion\\Run section
       at the registry.
<a href="https://sp7.co/manifest">website<a>
