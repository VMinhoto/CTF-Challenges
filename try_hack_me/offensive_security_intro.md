# URL 
https://tryhackme.com/room/offensivesecurityintro
# Category
Intro/Open Source Information
# Concept
Intro to the platform. How to use it and submit answers
# Methof of solve
## Task 1
* Read and the answer is `Offensive Security`
## Task 2
* A How to on how to interact with vms within the platform
* It starts a web app and promps you to get the bank nomber
* Answer is in the WebPage `8881`
## Task 3
* You need to find URLs available in the application
* For this you can run the command `dirb` against the base url. In this case: `dirb http://fakebank.thm`
* Answer with the found url: `http://fakebank.thm/bank-deposit`
## Task 4
* You need to add funds to your account using the found URL
* Navigate to it and add founds to your user account
* A green pop up appears with the anwer to the challenge `BANK-HACKED`
