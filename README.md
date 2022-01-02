# Blockchain-UI
Java application that creates a block and add it to a live block-chain server for the sake of practice & learning 

## Application technology
- Swing 
- Spring 

## Security
Securing the block is made by pubKey & priKey mixed with all block data and then hashing them using hashing-algorithms like (SHA-512). after that our block is now ready to be sent to the server

## Block data
In this application the data is just the username and a message that he wasnt to say <br>
```
public class BlockData {
    public String username
    public String message;
  }
```
## Block 
The block contains the following elements
```
public class BlockModel {
    private String prevhash;
    private DataModel data;
    private String signature;
    private String ts;
    private String publickey;
    }
```
after creation it is sent to the server for validations, once it passed it, it gets added to the chain

#### Note
- In this application only the client side was made.
- You can view the whole blocks in server in the json form on [SERVER](http://188.93.211.195/dis/chain)
