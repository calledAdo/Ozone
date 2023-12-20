# Ozone 

Ozone is a unique platform that aims to give creators of all kinds the freedom to truly own their arts and create strong communities with their Art lovers.<br>

Ozone brings back ownership into the hands of the true owners of any art which are the Art lovers and the Artists ,from an industry that is currently run by big firms who at most times put their profit as a priority over the Artists by deceitfully or forcefully taking ownership over their contents .<br>

Most independent artists struggle to promote their contents from Musicians to Content creators due to an apparent gap that has been exploited to the deterrment of Art lovers .

Ozone aims to solve this current issue by ensuring an immutable ownership of art to the artits by utilising the [DIP721](https://github.com/Psychedelic/DIP721).to allow artists bring their arts on the ICP Blockchain 



## Core Features

* ### Art Rights as NFTs<br>
   This would help artists monetise their contents and also serve as a source of promotion for their arts,as their fans are now incentivized to promote that particular Art.

* ### Arts as an Investment<br>
  Ozone provides an avenue for art lovers to invest in Arts that dey love e.g Music lovers can invest in a particular music by buying streaming rights or publishing rights and enjoy the benefits while also receiving others perks from the artist..

* ### Law onChain<br>
   Ozone provides for the existence of bringing law firms onChain,since users can buy rights to music ,these law firms can ensure that those royalties are splitted in a predetermined manner thereby facilitating transparency.<br>

__To Run The Project Locally__
  
  to start up your local replica run
```bash

dfx start 

```
now we would need to deploy our free Dip721 NFT canister by running and set its custodian to the Main canister
``` bash
# create an empty cansiter for Main
dfx canister create Main

#copy the resulting canister id and the run to deploy
dfx deploy DIP721 --argument "( principal \"$(dfx canister id Main)\",record {logo = record{
   logo_type = \"ICO\";
   data = \"NFT series\";
};
name = \"MY NFT\";symbol = \"m_NFT\";maxLimit = 100})"
```

```bash 
  dfx deploy Main --argument "(principal \"mxzaz-hqaaa-aaaar-qaada-cai\",principal \"asrmz-lmaaa-aaaaa-qaaeq-cai\")"
```
  

  Now you can create a collection from your already deployed NFT canister and  set anyone to mint it  after paying the fee ;

  __Note:Use the freeMint function if running locally  __ <br>

  currently deployed at  [Main](https://a4gq6-oaaaa-aaaab-qaa4q-cai.raw.icp0.io/?id=zbrhb-qyaaa-aaaal-adi5q-cai)
  with sample collection at [Sample Collection](https://a4gq6-oaaaa-aaaab-qaa4q-cai.raw.icp0.io/?id=zgqbv-5aaaa-aaaal-adi5a-cai)


