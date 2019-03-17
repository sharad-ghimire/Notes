## Lecture 1 Web Application Basics

The Internet is a global computer network that provides a way for remote computers and local networks to communicate and share services and resources. (What). From another viewpoint, the Internet can be seen as a set of Communication Protocols. (How). A protocol is a set of rules that govern data communication, how it is to be communicated and when it is to be communicated.
Internet of Everything? Cloud Computing? Big Data Analysis?

**The essence of Big Data**
Big data brings us three subversive ideas to change: all data, not random sampling; is the general direction, not the precise guidance; is the correlation, not the causal relationship.

1. is not a random sample, but the whole data: in the era of large data, we can analyze more data, and sometimes even deal with a particular phenomenon related to all the data, rather than relying on random sampling;
2. is not the accuracy, but the complexity: the research data so much, so that we are no longer keen on the pursuit of accuracy; before the need to analyze the data is very small, so we must be as accurate as possible to quantify our records, with Scale expansion, the accuracy of the obsession will be weakened; have a large data, we no longer need to dig a question at the end, as long as the master of the general direction of development can be appropriate to ignore the micro level of accuracy, Level has better insight;
3. is not a causal relationship, but a relationship: we are no longer keen to find a causal relationship, looking for causal relationship is a long habit of mankind, in the era of large data, we no longer need to focus on the causal relationship between things, but should find The relationship between things may not be able to accurately tell us why something happens, but it will remind us that this thing is happening.

**Internet Application Protocols**
| Protocol | Description |
| -------- | ----------------------------------------------------------------------------- |
| HTTP | Hypertext Transfer Protocol - used to retrieve web pages |
| HTTPS | Similar to HTTP - but data transfer is encrypted (HTTP- Secure) |
| SMTP | Simple Mail Transfer Protocol - used to send email |
| POP3 | Post Office Protocol - used to retrieve email |
| IMAP | Internet Message Access Protocol -such as Gmail, Outlook.com and Yahoo Mail |
| FTP | File Transfer Protocol - used to send and retrieve files |
| Telnet | Used to login to a remote machine for remote administration of Unix computers |
| SSH | Like telnet, used to login but data is encrypted. Secure Shell (SSH) |
| NNTP | Network News Transfer Protocol (NNTP) -used for serving Usenet Posts |

**Layered Protocols**

- Global Data Communications are implemented through several levels. There is an internationally ratified standard (model) setting out that defines the worldwide internet communication in seven layers and how they relate to each other. This is the famous OSI (Open Systems Interconnect) Model.
- An alternative and (simpler ) model is the TCP/IP Model. Here, we focus application layer of protocols, which are built on the top of the TCP/IP protocol stack.

**The OSI Data Communication Model**

1. Application: Allows Access to network resources
2. Presentation: Encrypts, translates and compresses data
3. Session: Establish, manages and terminates sessions
4. Transport: Provides reliable process-to-process message delivery and error recovery
5. Network: Moves data from source computer to destination computer
6. Data: Organizes bits into frames
7. Physical: Transmits bits (like electrical pulses) over a medium through defined physical interfaces.

The lower layers provide services for the upper layers. The lower layers are more hardware oriented than the upper ones. The very bottom layer i.e Physical is solely concerned with the physical and electrical properties of interfaces.

**The TCP/IP Data Communication Model**

- Application: This layer provides the same services as the Application; Presentation and Session Layers in the OSI Model.
- Transport: This layer is responsible for source to destination delivery of an entire message.
- Internet: This layer is responsible for the transmission of individual parts of a message (packets) from source to destination.
- Network Access: These protocols are not part of TCP/IP strictly speaking. However, TCP/IP supports most common protocols at this level including ethernet, FDDI, etc.

## Lecture 1.1 Unix Notes

## Lecture 2 Dynamic HTML

## Lecture 3 PHP Basics

## Lecture 4 PHP Sessions

## Lecture 5 JavaScript and AJAX

## Lecture 6 jQuery

## Lecture 7 XML

## Lecture 8 PHP DOM

## Lecture 9 OOP PHP

## Lecture 10 Web Security

## Lecture 11 Web Management
