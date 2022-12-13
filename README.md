## Lottery Dapp

Lottery is a dapp that allows participants to enter a lottery by sending a 0.001 ETH admission fee to the smart contract. 

Participants admission fees accumulate in the smart contract until they are eventually awarded to the winner of the lottery.  

Once all participants have entered, the contract owner clicks the "Pick Winner" via the UI and the smart contract will then leverage [Chainlink VRF V2 Function ](https://docs.chain.link/vrf/v2/introduction/) to determine the winner of the lottery. 

Once a winner is chosen by the contract, the contract owner then clicks "Pay Winner" and the smart contract initiates a transfer of the accumulated funds in the smart contract to the winners ETH address. 

Please see a video of the Lottery Dapp in action [here](https://youtube.com)

- The smart contract ```Lottery.sol``` was deployed on the Goerli ETH Testnet @ [0x7505c04b396c9e133ca912021e680f335f6db131](https://goerli.etherscan.io/address/0x7505c04b396c9e133ca912021e680f335f6db131)
- ```Lottery.sol``` leverages [Chainlink VRF V2 (Verifiable Random Function)](https://docs.chain.link/vrf/v2/introduction/) to retrieve a random value to determine the winner of the lottery without compromising security or usability.
- The frontend was built using [NextJS](https://nextjs.org/), [ReactJS](https://reactjs.org/) and [Bulma](https://bulma.io/).
- The development environment included [Truffle)](https://trufflesuite.com/), [NodeJS](https://nodejs.org/en/) & [Visual Studio](https://visualstudio.microsoft.com/)

![Alt text](/public/UI.png "Lottery Dapp UI")


