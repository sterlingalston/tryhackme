### What are Packets and Frames?

- Packets and frames are small pieces of data that, when forming together, make a larger piece of information or message
- **packet** is a piece of data from Layer 3 (Network Layer) of the OSI model, containing information such as an IP header and payload
- **frame**, however, is used at Layer 2 (Data Link) of the OSI model, which, encapsulates the packet and adds additional information such as MAC addresses.
- the _envelope_ is the _frame_ and the frame is used to move the contents
- once the recipient opens the _envelop_, they will know how to forward the _packet_
- process is called _**encapsulation**_ which we discussed in [room 3: the OSI model](https://tryhackme.com/room/osimodelzi)
- packets are efficient because the data is moved in small pieces across network devices
- packet = Layer 3
- frame = Layer 2
- packet using this protocol will have a set of headers that contain additional pieces of information to the data that is being sent across a network.

Some notable headers include:

|     |     |
| --- | --- |
| **Header** | **Description** |
| Time to Live | This field sets an expiry timer for the packet to not clog up your network if it never manages to reach a host or escape! |
| Checksum | This field provides integrity checking for protocols such as TCP/IP. If any data is changed, this value will be different from what was expected and therefore corrupt. |
| Source Address | The IP address of the device that the packet is being sent **from** so that data knows where to **return to**. |
| Destination Address | The device's IP address the packet is being sent to so that data knows where to travel next. |