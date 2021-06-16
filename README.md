# binance_SplitContract

Staking Smart Contract is based on the DeFi Staking concept in which users can stake their token and BNB for a particular period of time and can get reward based on it.
Staking Contract work on modules like users can stake tokens and BNB for 30 days, 60 days and 90 days respectively.
Rewards are defined which are based on the number of staking days.
Penalty will be applied on early withdrawal that means if the user withdraws a staked token or BNB before stake end time so penalty will be applicable.

Contract are divided into two contract
1. Token Contract  
2. Staking Contract  
(*Note : Token Contract can be used to define new token in future with whom company will collaborate so that it can be used as an interface in staking contract for that particular token staking methods defined in staking contract)  

==> Token Contract Functions List :   
    * View Only Function :  
       # function getowner(): Function to get Contract Owner Address.  
       # function name() : Function to get Token Name.  
       # function symbol(): Function to get Token Symbol.  
       # function decimal() : Function to get Token Decimal place value.  
       # function totalSupply(): Function to get Token Total Supply.  
       # function balanceOf(): Function to get balance of particular address holding tokens.  
       # function allowance(): Function to check the amount of tokens that an owner allowed.  
    * State Change Only Function :   
       # function transfer(): Function to get Transfer token from owner to any user address.  
       # function approve(): Function to approve user to transfer token on behalf of owner.  
       # function transferFrom(): Function to transfer token from one address to another address.  
       # function totalSupply(): Function to get total supply of the token.  
       # function burn(): Function to burn a particular amount of token.  
       # function mint(): Function to mint or produce a more particular amount of token.  
       # function getContractBNBBalance(): function to get BNB Balance from the contract.  
       # function transferOwnership(): Function to transfer ownership of contract.  
       
==> Staking Contract Functions list :  
    * View Only Function :  
      # function getowner(): function to get owner of the contract.  

        ** FOR TOKEN :  
           # function getTokenReward(): function to get value of added token reward.   
           # function getTokenStakingCount(): function to get current staking count which is running in Token Staking.  
           # function getTotalStakedToken(): function to get total staked token value by all users.  
           # function getTokenRewardDetailsByStakingId(): function to get token reward details of users by their staking id.  
           # function getTokenPenaltyDetailByStakingId(): function to get token penalty details for users by their staking id.  
           # function getFinalTokenStakeWithdraw(): function to get the final withdrawal amount the user will get after withdrawing stake token.  
           # function getTokenStakingAddressById(): Function to get Token Staking Address by staking id.  
           # function getTokenStakingIdByAddress(): function to get the staking id of the user by their address for token.  
           # function getTokenStakingStartTimeById(): function to get the user staking start time by their id for token staking.  
           # function getTokenStakingEndTimeById(): function to get user staking end time by their user id for token staking.  
           # function getTokenStakingTotalDaysById(): function to get total staking days of a user by their staking id for token.   
           # function getStakingTokenById(): Function to get the amount of staking token by user by staking id.  
           # function getTokenLockStatus(): function to get the lock status of a particular staking id for a token.  

        ** FOR BNB :
           # function getBNBReward(): function to get value of added BNB reward.  
           # function getBNBLimit(): function to get BNB limit value.  
           # function getBNBStakingCount(): Function to get current staking count which is running in BNB Staking.  
           # function getTotalStakedBNB(): function to get the total staked BNB value by all users.  
           # function getBNBRewardDetailsByStakingId(): function to get BNB reward details of users by their staking id.  
           # function getBNBPenaltyDetailByStakingId(): function to get BNB penalty details for users by their staking id.  
           # function getFinalBNBStakeWithdraw(): function to get the final withdrawal amount the user will get after withdrawing stake BNB.  
           # function getBNBStakingAddressById(): function to get the user address by their staking id for BNB staking.  
           # function getBNBStakingIdByAddress(): function to get the staking id of the user by their address for token.  
           # function getBNBStakingStartTimeById(): function to get the user staking start time by their id for BNB staking.  
           # function getBNBStakingEndTimeById(): function to get user staking end time by their user id for BNB staking.  
           # function getBNBStakingTotalDaysById(): function to get total staking days of a user by their staking id for BNB.  
           # function getBNBStakedById(): function to get the amount of BNB staked by the user by staking id.  
           # function getBNBStakedByUser(): Function to get BNB staked by user by their address.  
           # function getBNBLockStatus(): function to get lock status of particular staking id for BNB staking.  
           
    * State Change Only Function :   
           # function transferOwnership(): Function to transfer ownership of contract.  
           # function setContractAddress():  Function to set cliq token contract address which can be used in interface.  

        ** FOR TOKEN :   
           # function addTokenReward(): Function in which only the owner can add a token in a smart contract as a reward.  
           # function withdrawAddedToken(): function to withdraw added token reward by the owner.  
           # function pauseTokenStaking(): Function which is only owner where owner can pause token staking.  
           # function unpauseTokenStaking(): Function which is only owner where owner can unpause token staking.  
           # function stakeToken(): function used to stake a token for a particular period of time.  
           # function withdrawStakedTokens(): function to withdraw stake token with the help of staking id.  

        ** FOR BNB :  
           # function addBNBReward(): Function in which only the owner can add BNB in a smart contract as a reward.  
           # function withdrawAddedBNB(): function to withdraw added BNB reward by the owner.    
           # function setBNBLimit(): function to set BNB limit per user can stake.  
           # function pauseBNBStaking(): Function which is only owner where owner can pause BNB staking.
           # function unpauseBNBStaking(): Function which is only owner where owner can unpause BNB staking.  
           # function stakeBNB(): function used to stake BNB for a particular period of time.  
           # function withdrawStakedBNB(): function to withdraw stake BNB with the help of staking id.  
           
             
  These are the function list for Token Contract and Staking Contract, for other important fearures refer to contract.  
