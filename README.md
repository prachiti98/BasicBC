# BasicBC

https://hackernoon.com/learn-blockchains-by-building-one-117428612f46

Run using Postman or curl
Make 2 ports
Run on both the ports
Increase the length of the chains
  
  
 GET: http://localhost:3000/mine (make a new node)
 
 POST: http://localhost:3000/transactions/new (add it to the chain) (mention the transaction that you get in the body when you mine)

Repeat this on both ports : 3000 and 3002
Add the node of 3002 to 3000
  POST: http://localhost:3000/nodes/register (mention the name of the port you want to add)
  
Node will be added
    GET: http://localhost:3000/nodes/resolve  (Will choose the biggest length chain based on the consensus)
    
    
You can check your chain 
  GET : http://localhost:3000/chain
