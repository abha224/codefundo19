# codefundo++ 19 
The official repo of Team Exterminator for codefundo++ 2019.

# Why online voting ?

Elections have always been an integral part of every democracy, and secure elections have been a part of the sucessful ones. A lot of money in billions is spent every year to conduct elections throughout India.
With the era of digitalization, massive cost of conducting elections can be decreased by deploying an online portal for the same.
Voters may not be able to be present on the day of election for a number of reasons, including being away from the electorate, travelling, impending maternity, having religious beliefs that prevent you from attending a polling place, or being more than 8 km from a polling place. The participation in the voting can be exponentially increased with the use online service.We plan to build this online platform and integrate it with Azure blockchain to provide security and reliability.

# Aim and idea

- As mentioned above,we plan to enable secure online voting by using **Azure Blockchain**. This will ensure the confidentiality of the voter and provide easy and user friendly platform for the voters to cast their votes. 

- The front end and backend applications will be handled by **Web App for Containers** provided by Azure.

- Once the voting application is filled by the voter , the code will automatically check if the voter is eligible to cast a vote by accessing the dataset provided in https://data.gov.in/. It will also display the list of candidates according to the region where the voter is registered.The voter is verified through various documents like aadhaar card, voters id, phone number, address proof to eliminate the problem of no reliable voter identification. Added to this , a digital key gets associated with every new user for more security.

- During the time of elections, the voter can vote through a particular district by filling in the pincode or by using live location service that can be implemented using **Google maps API.** This is mainly to allow the people who arent present in their respective districts to also participate.

- After the voter creates a request for casting a vote, an unique QR code is generated using **zxing** . 

- In addition to the web app, an android application is made that scans this QR code and that navigates them to a one time window for a fixed time interval during which they can cast their vote. 

- The vote gets stored in the Blockchain along with the digital signature. Once they have sucessfully voted, the account remains locked for the rest of the voting period for that voter id. Every vote also receives a timestamp, so if necessary, it is possible to verify later if it was registered in the server.

- Another feature that we plan to add to this is  providing functionality of counting the votes and displaying the result in a structured manner using **Azure Event Hubs.**


