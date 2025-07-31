# Windows Firewall rule - Allow Web Access only to Microsoft Edge 


This rule configures Windows Firewall to Allow Internet Access only through Microsoft Edge Browser from a windows machine (e.g. Win11). All other browsers such as Chrome, Firefox, or others will be blocked from accessing the internet			


*note*: you can adapt this rule to allow or block any other browser by changing the application path.		


*note*: Note: Make sure your windows firewall is set to block outbound connections by default(in windows defender firewall properties). otherwise this rule may not restrict access as expected

Steps To Create This Rule:

1.Open Windows Firewall: in run menu type *wf.msc*

2.Create a new Outbound Rule:

        i.Select *Outbound Rule* then click *New Rule*
        
        ii.Choose *Custom* then click next
        
        iii.Choose *This Program Path* then type the *Path of your allowed Browser*
        
        iv.for *Protocol Type* choose *TCP* and for *Remote Port* select *Specific Ports* then type *8, 443*
        
        v.for *local ip address* and *Remote ip adress* Choose *any ip address*
        
        vi.Choose the firewall profiles(public or private or domain) depending on your network
        
        vii.Choose *Allow the Connections*
        
        viii.type a name for example *Allow Web Access to MS Edge*
        
