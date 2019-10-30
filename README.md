# VotingDapp
Secure voting application utilizing Solidity and JavaScript

A voting application utilizing blockchain to ensure one single vote per person.
Developed as part of Cal POly BlockChain Club
Base voting dapp was created by following this tutorial: https://www.dappuniversity.com/articles/the-ultimate-ethereum-dapp-tutorial 

*Note:* The tutorial has some slight errors due to changes in syntax.  If following the tutorial, the following should be accounted for:
- The constructor in Election.sol should be assigned as "constructor() public {...}"
- The parameter for addCandidate must have its data location declared as "memory," as this argument will not be stored on the blockchain
- The votedEvent thrown during the vote function must be declared with "emit", so it should look like "emit votedEvent(_candidateID);"
- "LocalHost" must be added to MetaMask's trusted networks

To run:
1) Have ganache-cli or ganache gui running in the background
2) Type "truffle migrate" into the command line
3) Type "npm run dev" into the command line
4) Your default browser will open with the front end of the voting dapp.
5) Click on the metamask menu to change your network to "LocalHost____"
6) Vote!
