# WAKIO - The first truly decentralized blogging platform

![Screenshots](./img/wakio.png)

Website: https://siasky.net/hns/wakio/

Blog created using Wakio: https://siasky.net/hns/bunnu/

## What is Wakio
A decentralized blogging platform that lives in the sia blockchain. It allows to create self-contained decentralized blogs. This means that the blogs allow to create new posts, and publish them in skynet without the need of external tools. Furthermore, thanks to its integration with namespace's api (through my project https://github.com/gagdiez/skynet_handshake_api), the blogs can update their handshake domain.

## How it works

When adding a post, the HTML of the website grows! (this is, the DOM is updated). Then, at the moment of publishing, the HTML of the whole website is copied and uploaded to skynet. The blog retrieves the new skylink and gives it to the user. Example: http://siasky.net/OABZuWajwfP0CNs3CZ_iUXCo8QIbn-Qbjxy8Es-TMj4QFw

If the user wants, can integrate its handshake domain to the blog, so it gets automatically updated each time a post is published. For this, the user needs to include their access key and secret key from namebase. Using a password that you choose, Wakio encrypts both keys using the AES algorithm, and embeds them into the blog. Then, at the moment of publishing the blog, the user will have to input their password, the keys will be decrypted, and the blog will contact the namebase API to update the handshake domain. The user is forced to use a secure password (>30 characters) in order to use this service.



