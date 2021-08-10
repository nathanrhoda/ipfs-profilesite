## Interplanetary File Storage IPFS Profile Site

The InterPlanetary File System is a protocol and peer-to-peer network for storing and sharing data in a distributed file system. 
IPFS uses content-addressing to uniquely identify each file in a global namespace connecting all computing devices.


- Installations:  https://gist.github.com/drwasho/ca224cbd4a21440f7cc1245e594398e4
- To add a file or website: ipfs add <filename>
- To view a file in console: ipfs cat <hash>
- To view locally: http://localhost:5001/webui   Files left nav
- To view online: https://ipfs.io/ipfs/<hash>
- To get a statically named hash that will remain the same when different versions of a website or file is added you can use: ipfs name publish <hash>
this will take a while to run and you will get back 2 hashes first one is static hash second one refers to latest version


Gotcha: 
* Might need to run incognito sometimes struggles to render second hash after viewing first
* Hash is related to data and is addressed accordingly meaning a differently named file with the same contents will have the same hash

To publish website

- ipfs add -r [fs-profilesite]
- Navigate to https://ipfs.io/ipfs/[hash output]
- ipfs name publish [hash of directory(normally last hash from previous command)]
- Naviagate to https://ipfs.io/ipns/[first hash output]
https://ipfs.io/ipns/k51qzi5uqu5dhpv036pojmmya7snaey0sxtp9j1xh4n0oj6myqbnptkcwjzawq/


More documentation and reading here: https://docs.ipfs.io/