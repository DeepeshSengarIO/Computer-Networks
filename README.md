# Introduction to Computer Networks

## Computer Network

    A Computer Network is formed by two or more devices connected together.
    Resources sharing etc operations occur via computer networks. Example, Printer connected to PC in office

## Key Challenges in Computer Networks

    Reliability
    Scalability
    Allocation of Bandwidth
    Security

# OSI and TCP/IP Model

## What is protocols?

    Protocols are set of rules which are used by two devices tio communicated. There are some fixed headers defined by the protocols.
    These headers specify the content of the message and how the content has to be messaged.
    These headers might be source address, destination address, check sum of the address to do the error detection.
    IP, TCP, UDP, HTTP

## Why do we need layers?

    To organise all the layers inside the protocols. Do not get dependent on the Wifi etc.
    There are two popular models to layer the computer networks.
    OSI Model and TCP IP Model

## OSI Model - 7 Layers

    Here we can device the network into the 7 Layers
    1. Application      - Applications like skype etc. (HTTP, SMTP, DNS, FTP, SSH)
    2. Presentation     - Data Compression/Uncompression, Encoding/Decoding of Data, Encryption/Decryption
    3. Session          - session management and authentication, combining of multiple streams ( syncronization )
    4. Transport        - end to end delivery ( 0 to 4 types of services according to flexibility of how many sercvices provided )
    5. Network          - help find routing. implemented by IP Protocol, reliable or unreliable
    6. Data Link        - One device to other device communication
    7. Physical         - Physical Device (Binary)

    Every layer from sender add headers to the message and that header is removed only when it is removed by receiver.
    Every layer encapsulate the previous one and move it further.
    It is a theoretical model and never implemented in practical sessions and more practical model and most widely used is TCP/IP Model and this model has 4 layers.

## TCP/IP Model - 4 Layers

    Here we have the only 4 layers.
    1. Application  (Units - Message)  -> using either of transport layer and IP address, application layer implements the applications
    2. Transport    (Units - Segment)  -> UDP(DNS), TCP(HTTP)
    3. Network      (Units - Packet)   -> Always Unreliable, always use IP protocol
    4. Link         (Units - Frame)    -> Does both Physical and Data Link layer function from OSI model

    Order goes this way:
        1.HTTP -> 2.TCP -> 3.IP -> 4.(Ethernet/Wifi)
