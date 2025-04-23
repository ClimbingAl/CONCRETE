---
title: IPFS
parent: The CONCRETE stack
nav_order: 4
---
# Inter-Planetary File System 
{: .fs-9 .no_toc }


Content (not location) addressed distributed data storage
{: .fs-6 .fw-300 }
----
[![ipfs logo](../../../../images/current/ipfs.png)](https://ipfs.tech/)

The [Inter-Planetary File System (IPFS)](https://ipfs.tech/) provides a distributed and decentralised approach to data storage[^bittorrent].  In centralised systems, the name of a data source commonly reflects its location eg a file location, or a web-address. This approach is not appropriate for distributed and decentralised systems. In an IPFS network, data is immutable (it cannot change); it can be stored and replicated, as often as desired, on any node.  The name of the data represents its content.  Users can request that content from anywhere.  As long as one connected node has it, it can be recovered.

[^bittorrent]:
    As a mental short-cut for some people 'of a certain age', IPFS has many similarties with Bittorrent file sharing.  A data source is named, and can be requested, and served, from anywhere across a distributed network. 

![data being split up into different channels](../../../../images/current/data_output_division.png)

In a CONCRETE world, the expectation (above) is that data would be disaggregated into separate data streams, and within those streams the data would be 'chunked' into IPFS's Inter-Planetary Linked Data (IPLD) data objects. (Security related discussion - LINK).  


In IPFS the names for blocks of data (green fingerprints below - aka Content IDentifiers CIDs in IPFS) are calculated from, and uniquely identify, the associated data (blue).  A user can request a block of data by providing the fingerprint, retreive it, and subsequently re-calculate the fingerprint/CID from the data received to confirm that they have exactly what was requested.

![basic ipfs fingerprint contains a hash of the data and some extra data about the fingerprinting method](../../../../images/current/fingerprint_details.png)

The IPFS/IPLD functionality enables larger blocks of data (below) to be referred to compactly by fingerprint links.

![a satellite image split up into tiles.  Each tile has its own fingerprint.  The whole image is a fingerprint of fingerprints](../../../../images/current/sat_dag_basic.png)

