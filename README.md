# Simple-open-auction
Simple blind auction contract anyone can send their bids during a bidding period.

**Description**

By use of blockchain technologies to realize decentralized auctions. The risks from the third-party auctioneers are well eliminated.
The proposed project addresses the following issues faced by physical auctions;

*Sealability:* All information in the auction transaction is encrypted by the public keys of the smart contract.
				
*Fairness:* All bidders are equally treated by the smart contract.

*Validity:* The contract selected the winning bid price and the related bidder as the auction result, obeying the basic rule of the first-price sealed auction.
				
*Nonrepudiation:* All information in the auction transaction was saved in the blockchain.
				
*Decentralized Verification:* All bidders can verify and prove the auction result.

*Cost-Effectiveness:* The scheme was free of the cost of the third-party auctioneer.
 
 **System Content(boundaries)**
 
 Storage variables such as; bool public canceled, address public owner,uint public bidIncrement,uint public startBlock.
 
 **Interaction with other products and components**
 
 Intergration with web based platforms using Html, Css and Javascript frameworks.
 
 **Product features**
 
 1. **The Register Phase:** The users including the owner of goods and all bidders should register in the sealed auction system.
 
 2. **The Publish Phase:** After registration, the owner of goods called the publish() function in the smart contract to publish the goods information.
 
 3. **The Bid Phase:** The registered bidders who were interested in the goods are permitted to bid.
 
 4. **The Open Phase:** 
 
 i. The smart contract counts the bidders attending the auction and checked all bid prices in the auction.
 
ii. All bid price was sorted and the highest bid price is selected as the winning bid price.

iii. The commitment price  bound to highest bidder is published to the blockchain by the smart contract.
								 
iv. Each differential commitment price is calculated and encrypted with the public key of each bidder by smart contract and sent back to each bidder.
								 
  5. **The Verify Phase:** Then all bidders use Bulletproofs protocol to prove prices without leaking any information about the winning bid price.
	
  6. **The Finish Phase:** After all bidders are verified and accepted , the smart contract asks the winning bidder to pay the rest of the payment for goods.
  
  **Security requirements***
	
  i. User Authentication
	
  ii. Secure storage
	
  iii. Realtime Monitoring
	
  iv. Advanced Data Encryption
  
  **Characteristics of users**
	
  i. Owner
	
  ii. Bidders
  
  **Restrictions**
	
It should be noted that the proposed scheme has limitations in running performance. The execution time of the open phase and finish phase is determined by the number of bidders. this means that the auction would become a time-consuming work if conducted in the open platforms such as Internet.
  
                 
