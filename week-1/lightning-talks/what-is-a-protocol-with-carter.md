# What is a Protocol?

In Italy, when you answer the phone you say "Pronto" which means "Ready." Here
we say "hello" and they say "Hello" and then you start the conversation.

This is a protocol. A protocol is a procedure for how you are going to go about
communicating.

Official definition: "A system for message exchange within or between computers"

## Some Protocols

1. HTTP
1. FTP
1. HTTPS
1. UDP
1. TCP/IP - The main protocol of the Internet.

## TCP/IP

Stands for "Transmission Control Protocol." The sender sends some packets, the
receiver says "I got that packet! Send the next one!" or "I didn't get that
packet, send it again!" This has high overhead, but is very reliable.

You want to use TCP when you care about packet delivery. Like web sites.

## UDP

Sender transmits packets, and the receivr doesn't care if it misses them. They
come through in a stream. It's less reliable; but it's quite fast.

You want to use TCP when you care more about speed than reliability. Like for
conference calls, etc.



