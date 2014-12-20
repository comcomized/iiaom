## License - Humanitarian AGPL License: 

You are not allowed to use, produce from or design from this or its part, anything contained with the aim to kill,to cause harm to or to monitor people and any permission beside that is given only under the [AGPL License](http://www.gnu.org/licenses/agpl-3.0.html)!

# iiaom - Inner Identifier And Outer Mask, a Crypto Identity for everyone.

It is a hash of an image + its symmetrically encrypted file, where only the encrypted file is stored in the human's device and in darknet or common server, as the hash is distributed and, if the human is identified, the hash is signed in WOT for gaining its reputation. It is used for authenticating human when accountability and/or equality is required. Eg. in communication  and in democratic applications, while bypassing monitoring done by any kind of syndicate via government documents. [more..](http://namzezam.wikidot.com/blog:12)

Use case: Providing reliable peerid in peerjs and more generally helping in webrtc app (such as webtorrent) for more trustable p2p human identification, to bypass, or reduce, the need of a server (such as peerjs-server). eg. for p2p by iiaom on xmpp or webrtc with tor or other means, consists of: 
    all peers are user having iioam and nodes are cheap serves; 
    the parties are: "a" and "b" communicating peers, "d" - peer or nodeServer in duty and "n" - nodeServer; 
    the date passed between "d" is negotiationData and messagesData per each reading peer, where 
         negotiationData has, hash(iiaom), the current-ip/last-time-seen and
         messagesData has a limited size data of unread msg being encrypted with the public key of the absent reading peer;
    "n" having ip and only optionally domain name, replies only on successful request with ip("d"); and
    "d" having negotiationData and messagesData used when "a" (having iiaom) asks to connect to "b" (defined by other iiaom), so that
        1st "d" try to find after hash the (iiaom("a")) and the(iiaom("b")) and then on success attach the ip("a") negotiationData and  send to "a" the ip("b) or when "b" is not enviable receive from "a" and add the data encrypted with pub of "b".

It is now developed in a [dComcom](http://yes-again-we-can.wikidot.com/s-contract:groups-collaborating-comcomized-platform-gccp/edit/true/title/Groups%20Collaborating%20Comcomized%20Platform%20%28GCCP%29/parentPage/start%3As-contract)  being [Groups Collaborating Comcomized Platform (GCCP)](http://namzezam.wikidot.com/blog:24), and you can  [contact](http://namzezam.wikidot.com/main:contact) to join.

## Install

npm install -g git://github.com/comcomist/iiaom.git

## How-to

http://iiaom.wikidot.com/

## todo:
 this protocol must be performed only in a mutual verifying,
 where H (human) is also V(verifier) and vs,    for making it  more expensive for the mass attackers!
 
1 H: in create <file> to make the hash of both the encrypted and the source and if it was not "safe" still to ask to delete to source!!

2.V: another option - get(encrypted, pubkey )
    sending to H encrypted asymmetrically the symmetrically encrypted file

2.H: another option - give(pubkey, encrypted file)
    sending to V encrypted asymmetrically the file

3. V: in verify
  1. hash both the encrypted and the non encrypted to match the iiaom
  2. try match by other means the human with the pic
  3. sign the iiaom on matching

4. after signing the iiaom (being hash both encrypted and source) should be hashed again and
put in encrypted dir/db or table having also counter (of normality) +optionally with date and notes.
    1, this would  allow measurement of
        1, integer: any time publicly, trust of the human=  number of unique trustees
        2, integer: any time internally, counter normality with trustee= the number of being singed by trustee
        3. percentage:  when the normality is high, between 2 how match they are related per each=
            of those sining me how much singed you
             more related to other probebly more attracted to the other !?

Also see http://namzezam.wikidot.com/blog:12#last-minit-note
