## ***[Applying The CIA Triad To Your Enterprise File Transfer](https://www.jscape.com/blog/implementing-the-cia-triad-when-transferring-files-through-the-internet)***

## ***[What Are MD5, SHA-1, and SHA-256 Hashes, and How Do I Check Them?](https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/)***

### You have been made responsible for the company’s file server. How would you preserve the three elements of the CIA triad?
I have yet to be responsible for a company file server, but if I were, I would implement the CIA triad. Here's how I would implement that: 
* Confidentiality, I would implement end-to-end encryption
* Integrity, I would implement verify digital signatures.
* Availability, I would implement a Data Loss Prevention system that automatically detects sensitive data and takes appropriate action, such as canceling downloads or applying encryption.
### Explain how hashing verifies data integrity using non-technical terms.
Imagine you are using a food delivery app to order food. You receive a detailed receipt of your order, which lists all the items you have ordered. You want to ensure that your order is not lost or tampered with during the delivery process. In this case, hashing generates a unique code from the data. If any food item goes missing or your receipt does not match up, the hashing value will change, indicating that the data has been altered. This helps to ensure the integrity of your order.
### How is hashing and encryption different?
Hashing is a one-way function. If any data has been altered, the hash value will change. Encryption generates a unique and complex key that is required to decrypt the data.
