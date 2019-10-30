# Palo-Alto-Application-Enable-DLP

As part of an ongoing project, I had to enable Data Loss Prevention or DLP in my company's Palo Alto Firewalls. We had two problems doing that.

Firstly, in order to do that, I had to configure the password to each individual firewall. Even though we are managing our firewalls from the central management platform Panorama, configuring the DLP password is not possible from it.

Secondly, as network security engineer, I should not know the password as I have got write only privileges. Only the InfoSec department should know that password. Nonetheless, the InfoSec dep has goot read-only access. So, they cannot configure it and we should not know it.

Considering the aforementioned problems, I created a Python application that asks the network security engineer for his credentials and then it asks the InfoSec person for the password. The Programme then connects to each firewall via SSH in order to configure the password.

Due to the fact that we rotate passwords in a fixed time, the programme provides the ability to change an already configured password.

I am able to share this application publicly because I created this programme on my own free time and I own the copyrights of it.
