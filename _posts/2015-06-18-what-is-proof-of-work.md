---
layout: post
title: What is Proof of Work
author: Bitcoin Mining
authorurl: /
published: true
---


<center><img src="/images/what-is-proof-of-work.png">
<a href="/images/what-is-proof-of-work-high-resolution.png" target="_blank">Visualize and Download High-Resolution Infographic</a></center></center>
<p>A proof of work is a piece of data which was difficult (costly, time-consuming) to produce so as to satisfy certain requirements. It must be trivial to check whether data satisfies said requirements.
<p>Producing a proof of work can be a random process with low probability, so that a lot of trial and error is required on average before a valid proof of work is generated. Bitcoin uses the <a href="/what-is-hashcash/">hashcash</a> proof of work.
<p>One application of this idea is using hashcash as a method to preventing email spam, requiring a proof of work on the email's contents (including the To address), on every email.
<p>Legitimate emails will be able to do the work to generate the proof easily (not much work is required for a single email), but mass spam emailers will have difficulty generating the required proofs (which would require huge computational resources).
<p>Hashcash proofs of work are used in Bitcoin for block generation. Proofs of work that are tied to the data of each block are required for the blocks to be accepted. The difficulty of this work is adjusted so as to limit the rate at which new blocks can be generated by the network to one every 10 minutes.
<p>Due to the very low probability of successful generation, this makes it unpredictable which worker computer in the network will be able to generate the next block.
<p>For a block to be valid it must hash to a value less than the current target; this means that each block indicates that work has been done generating it. Each block contains the hash of the preceding block, thus each block has a chain of blocks that together contain a large amount of work.
<p>Changing a block (which can only be done by making a new block containing the same predecessor) requires regenerating all successors and redoing the work they contain. This protects the block chain from tampering.
<p>The most widely used proof-of-work scheme is SHA-256, which was introduced by Bitcoin. Some other hashing algorithms that are used for proof-of-work include scrypt, Blake-256, CryptoNight, HEFTY1, Quark, SHA-3, scrypt-jane, scrypt-n and combinations.