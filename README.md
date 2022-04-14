# Introduction 
### This file is only used to add/edit/delete the pool infomation in poolsV2.config on the Launchpad website. Below is the guidance on how to fill in information under each title. Besides, I have also written how to check the participants and their investment amount at the end of this introduction.
# How to add pool.
![](https://trustfi.s3.ap-southeast-1.amazonaws.com/images/new.png)
Copy the text in the red box in the above picture and paste them to new line. Then make sure there is no "," at the end of "}"

Below are some information about each title:
### poolid (no "")
Before you create a pool on the website, you can ping me to know what's the PoolId, cause I need to build the pool on chain first.
### IdoFactory (with" ")
Fixed value:0xE1F2297616f443853664425DCb4B149f3AB8e88A
### Name (with" ")
The project name
### Namekey (with" ")
It will show on the website link. For example:https://launchpad.trustfi.org/#/v2/**MetaFighterFPS**/join in this link, MetafighterFPS is what you fill in. 
**Pay attention**: you should make sure that each time you edit the poolid the namekey should be edited a little bit different as well. For example, if we have built a pool called Trustfi as Pool10 and also have write the information in github with poolid "10" and namekey:"TrustfiIDO". But the project party wants to change the IDO date or pool size etc. now, then we need to rebulid a new pool 11. At this time, the information in github should be poolid"11" and the namekey should be "TrustfiIDO2" or something else as long as it is not "TrustfiIDO".
### ChianId (no "")
Fixed value:56
### Type (with" ")
It can be "IDO" or "Private Sale"
### distribution (with" ")
It can be "Airdrop" or "claim"
### avatar (with" ")
The project's Logo url. 
### subName (with" ")
$+Token symbol. For exmaple: $TFI
### claimStarts (no "")
If the distribution way is "Airdrop" then fill in "0" here, if the distribution way is "claim" then fill in time here. For the time you should add a **Unix timestamp** in ms form. For example if it is 2022/4/14 2PM then it should be 1649944800000 here.
### idoTokenPrice  (no "")
The price of Token. For example 0.14
### launchTime (no "")
When the pool will start. Also need to fill in a **Unix timestamp** in ms form. For example if it is 2022/4/14 2PM then it should be 1649944800000 here.
### vesting (with" ")
Vesting schedule
### claimRatio (no "")
Claim ratio=1/price* how much rate will the distribute on TGE. For example, token price is 0.14 and vesting schedule is 10% at TGE, 90 day cliff, then 8% every month then the claim ratio=1/0.14* 0.1=0.7
### description (with" ")
Description about the project. Please don't make a new line no matter how long the description is.
### about (with" ")
Some other introduction about the project. It can be the same as description but still should be in on line.
### idoType (with" ")
It will be shown as the tag on the pool so it can be "Flash Sale"or"IDO"or"FCFS Sale"etc.
### pic1/2/3/4/5 (with" ")
They will be shown on the top of the pool. Fill in the url of the 5 pics here.
### website (with" ")
website url
### twitter (with" ")
twitter url
### telegram (with" ")
telegram url
### chainName (with" ")
The project is on which chian. For example: BSC/Solona
### startTime (with" ")
When will the pool start. No need for Unix timestamp form this time. For example, the pool will start on 2022/4/14 2pm UTC then fill in "2PM 04/14/2022 UTC" here.
### endtime  (with" ")
When will the pool finish. No need for Unix timestamp form this time. For example, the pool will finish on 2022/4/14 2pm UTC then fill in "2PM 04/14/2022 UTC" here.
### idoTokenSymbol (with" ")
Token Symbol. For example:TFI
### idoOnChainName (with" ")
The IDO is on which chian. fixed value: BSC
### idoOnChainLogo  (with" ")
Fixed value:https://pbs.twimg.com/profile_images/1493575277498503170/mEoTGl9c_400x400.jpg
### distributedName (with" ")
On which chain will the project distribute its token. For example, SOL/BSC
### distributedLogo (with" ")
For example, if "distributedName"is SOL then fill in SOL's logo url here :https://pbs.twimg.com/profile_images/1472933274209107976/6u-LQfjG_400x400.jpg. If the "distributedName"is BSC the  fill in BSC's logo url here: https://pbs.twimg.com/profile_images/1493575277498503170/mEoTGl9c_400x400.jpg
# How to edit/delete a pool
### 1. edit a pool: You can edit the information you want to edit under any title except for those fixed value.
### 2. delete pool: delete all the above information(Like the blue part from the pic above) of the pool you want to delete. 

# Some problems you may meet
### 1. Cannot see the new information after your edit: 
1. please wait for at least 3 minutes, and refresh the website.
2. please make sure the namekey is new and different from the previous pool.
3. please google a Json verified tool that can check whether the form of your added information is correct.
4. If still cannot solve the problem, please let us know.
### 2. Cannot see the new pool after you add a new pool:
1. please wait for at least 3 minutes, and refresh the website.
2. please make sure the poolid has been updated and is correct.
3. please make sure the namekey is new and different from the previous pool.
4. please google a Json verified tool that can check whether the form of your added information is correct.
5. If still cannot solve the problem, please let us know.
### 3. Still can see the pool after you delete the pool information
1. Make sure you have deleted the right information. And wait for at least 3minutes and refresh it.
2. If you made mistakes and want to find the previous information you can click the history button on the right corner to see your edit histroy.
3. If still cannot solve the problem, please let us know.

# How to check the participants and their investment amount
### 1.0xE1F2297616f443853664425DCb4B149f3AB8e88A search it on BscScan 
### 2.Choose BEP-20 Token Txns and download it. 
1. please choose time according to the pool start time and end time.
2. After you got the information you can check 1. whether the token is BUSD, if not, ignore it. 2.check whether there has duplicate address, if yes, combine them.
3. **Pay attention**:
If there are 2 or more pools start at the same time or some pools duration time is some overlap, please let me know in the group since it will be difficult to distinguish which pool are they in.

