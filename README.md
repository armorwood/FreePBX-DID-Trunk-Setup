# FreePBX-DID-Trunk-Setup
Simple guide for setting up DID trunks for FreePBX, and the possible complications when setting up.

**NOTE: I AM NOT A PROFESSIONAL; THIS IS MAINLY FOR EDUCATIONAL AND DOCUMENTARY PURPOSES. This tutorial is mainly for home lab PBXs**

# What is a DID, and where can I purchase one? 
A DID (Direct Inward Dialing) number is a standard public phone number that connects external callers over the PSTN (Public Switched Telephone Network) directly into your PBX. Instead of needing a physical copper line for every single phone, a DID allows your PBX to handle incoming calls digitally over the internet and route them pretty much anywhere as long as you have an internet connection, such as an automated IVR attendant, a specific desk phone, or a ring group.

DIDs are very inexpensive for lab setups. You can lease a local area code number from SIP trunk providers (like Callcentric, VoIP.ms, or Telnyx) for around $1.00 to $5.00/month, then add a few dollars of pay-per-minute credit to cover incoming and outgoing traffic. I personally, for this tutorial, will be utilizing Callcentric, specifically their pay-as-you-go plan.

# My Enviroment/Prerquisties
**PBX Host** I will be using Oracle VirtualBox, running FREEPBX 
