
## Internet Telephony (1L):

Internet Telephony Protocol is also called Voice Over IP . It is a real-time interactive audio/video application. As from the name Internet Telephony, it uses internet as a telephone network with additional features. To communicate between two parties, it uses packet-switched Internet.

There are two different types of protocols that enable Internet Telephony.

1. H.323
2. Session Initiation Protocol (SIP)

### H.323 :
Basically, H.323 may be a standard set by ITU which allows telephones on the general public telephone network to speak to computers connected to internet. The architecture of H.323 is shown as shown as:

![image](https://github.com/pritamhazra21/WIT/assets/75198912/0e278eaf-3895-4f63-9f63-da0c28cc6070)

H.323 Architecture Model

At the center, there is gateway placed which connects the internet to the telephone network. Gateway translates a message from one protocol to another. It speaks H.323 protocol on Internet site and PSTN i.e. Public Switched Telephone Network protocol on telephone side. It will act as both computer and telephone. A LAN may have a gatekeeper which controls the terminals under its jurisdiction calledzone.

### Protocols of H.323 :
To maintain audio or video communication, H.323 uses a number of protocols. The various protocols used are as shown in the following figure.

![image](https://github.com/pritamhazra21/WIT/assets/75198912/f9f1ab85-bf42-4498-8599-afbae1810248)

H.323 Protocol Stack

1. G.711 or G.723.1 –
These protocols are used for compression.
2. H.245 –
In this, multiple compression protocols are permitted, H.245 allows the terminals to negotiate which protocol to use for compression. H.245 also negotiates bit rate.
3. RTCP –
It is used to control RTP channels.
4. Q.931 –
This protocol is required for establishing and releasing connections, providing dial tones, making ringing sounds.
5. H.225 –
This protocol enables the terminals to talk to gatekeepers. This protocol also manages PC-to-gatekeeper channel called RAS channel. This channel allows the terminals to join and leave the zone, request and return bandwidth and provide status updates.
6. RTP –
It is used for actual data transmission.

## VoIP.

Voice over Internet Protocol (VoIP), is a technology that allowing you to make voice calls over a broadband Internet connection instead of an analog (regular) phone line. Some VoIP services allow you to call people using the same service, but others may allow you to call anyone. They can have a telephone number – including local, long-distance, mobile, and international numbers or not. Some VoIP services only work over your computer or a special VoIP phone while other services allow you to use a traditional phone connected to a VoIP adapter. 

How VoIP / Internet Voice Works – 

Voice is converted into a digital signal by VoIP services that travel over the Internet. If the regular phone number is called, the signal is converted to a regular telephone signal i.e. an analog signal before it reaches the destination. VoIP can allow you to make a call directly from a computer having a special VoIP phone, or a traditional phone connected to a special adapter. Wireless hot spots in locations such as airports, hospitals, cafes, etc allow you to connect to the Internet and can enable you to use VoIP service wirelessly. 

Equipments Required – 

A high-speed Internet connection is required which can be through a cable modem or high-speed services such as a local area network. A computer, adaptor, or specialized phone is required. Some VoIP services only work over your computer or a special VoIP phone. Other services allow you to use a traditional phone connected to a VoIP adapter. If you use your computer some software and an inexpensive microphone are needed. VoIP phones plug directly into your broadband connection and operate largely like a traditional telephone. If you use a telephone with a VoIP adapter, you can dial just as you always have, and the service provider may also provide a dial tone. 

Advantages of VoIP – 
 

1. Some VoIP services offer features and services that are not available with a traditional phone, or are available but only for an additional fee. 
1. Paying for both a broadband connection and a traditional telephone line can be avoided. 
1. Smoother connection than an analog signal can be provided. 
 
Disadvantages of VoIP – 
 

1. Some VoIP services don’t work during power outages and the service provider may not offer backup power. 
1. Not all VoIP services connect directly to emergency services through emergency service numbers. 
1. VoIP providers may or may not offer directory assistance. 


## Multimedia Applications (2L):
### Multimedia over IP: 
#### RSVP


RSVP stands for Resource Reservation Protocol. It is a protocol used in computer networks to provide Quality of Service (QoS) guarantees for multimedia applications over IP (Internet Protocol) networks. RSVP is specifically designed to support real-time, interactive, and multimedia applications such as voice and video conferencing.

The main purpose of RSVP is to enable network devices, such as routers, to reserve and allocate network resources along a specific path to ensure the required QoS for multimedia traffic. RSVP operates on a per-flow basis, meaning that it establishes and maintains reservations for individual data flows.

#### RTP,

RTP (Real-time Transport Protocol) is a protocol used for transporting real-time multimedia data over IP networks. It breaks media streams into packets, assigns timestamps and sequence numbers to ensure proper sequencing and synchronization. RTP supports different payload types for different media formats. It works in conjunction with RTCP (RTP Control Protocol) for feedback and control purposes. RTP uses UDP for transport and is widely used in applications such as VoIP, video conferencing, and streaming media.

#### RTCP

RTCP (RTP Control Protocol) is a protocol used in conjunction with RTP (Real-time Transport Protocol) for control and feedback purposes in real-time multimedia applications. It enables participants to exchange information about the quality and delivery of RTP streams, including feedback reports, statistics, and control messages. RTCP works alongside RTP to ensure smooth and efficient transmission of real-time media over IP networks.

#### RTSP

RTSP (Real-Time Streaming Protocol) is a network protocol used for controlling the delivery of real-time multimedia streams over IP networks. It enables clients to remotely control playback of media files or live streams from a server. RTSP establishes a session and facilitates communication for commands like play, pause, seek, and stop. It is commonly used for streaming applications, video surveillance, and video-on-demand services.

Streaming media, Codec and Plugins, IPTV.
## Search Engine and Web Crawler (2L):
Definition, Meta data, 

### Web Crawler


A web crawler, also known as a spider or web robot, is an automated software program that systematically navigates through the World Wide Web, indexing and gathering information from web pages. It is an essential component of search engines, used to build and maintain their vast indexes of web content.

+ Purpose: Discover and retrieve web pages.
+ Crawling Process: Follows links to explore and retrieve more pages.
+ URL Frontier: Maintains a list of URLs to be crawled.
+ Politeness and Respect: Adheres to robots.txt guidelines and server load limitations.
+ Indexing and Data Extraction: Collects and processes information for search engine indexing.
+ Freshness and Recrawling: Updates indexed pages by periodically revisiting them.

### Indexing:

Indexing is the process by which search engines analyze and store information about web pages. When a web crawler discovers a new page, it collects relevant data such as the page's content, metadata, and links. This information is then indexed, allowing the search engine to quickly retrieve and present relevant results when users perform searches. Indexing helps search engines organize and categorize vast amounts of web content for efficient retrieval.

### Page Rank:

Page Rank is an algorithm developed by Google co-founders Larry Page and Sergey Brin. It assigns a numerical value, known as a Page Rank score, to each web page based on its relevance, authority, and popularity. The Page Rank algorithm considers factors such as the number and quality of incoming links to a page to determine its importance. Pages with higher Page Rank scores are generally considered more authoritative and are likely to appear higher in search engine result pages (SERPs). Page Rank is one of many factors used by search engines to rank web pages and determine their visibility in search results.



### overview of SEO.

SEO (Search Engine Optimization) is the practice of optimizing a website to improve its visibility and ranking in search engine results pages (SERPs). It involves various techniques and strategies aimed at increasing organic (non-paid) traffic to a website.

Here's an overview of SEO:

1. Keyword Research: SEO begins with keyword research, which involves identifying the relevant keywords and phrases that people use when searching for information related to your website's content or products.

2. On-Page Optimization: On-page optimization focuses on optimizing individual web pages to make them more search engine-friendly. This includes optimizing meta tags, headings, content, URL structure, and internal linking. It also involves incorporating relevant keywords naturally within the content.

3. Technical SEO: Technical SEO ensures that a website is technically optimized for search engines to crawl, index, and understand its content. This includes optimizing website speed, improving mobile responsiveness, implementing structured data markup, and ensuring proper XML sitemap and robots.txt file setup.

4. Off-Page Optimization: Off-page optimization refers to activities conducted outside of your website to improve its online reputation and authority. This includes link building, social media engagement, online PR, and influencer marketing. The goal is to acquire high-quality backlinks from reputable sources to increase the website's credibility.

5. User Experience: SEO also focuses on enhancing the user experience of a website. This involves optimizing site navigation, improving page load times, making the website mobile-friendly, and providing relevant and valuable content that meets user needs.

6. Content Marketing: Producing high-quality and relevant content is crucial for SEO. Content marketing involves creating and promoting content such as blog posts, articles, videos, infographics, and more to attract and engage users. Good content also increases the likelihood of earning natural backlinks.

7. Monitoring and Analysis: SEO is an ongoing process that requires monitoring and analysis. It involves tracking keyword rankings, website traffic, user behavior, and conversions. This data helps identify areas for improvement and adjust SEO strategies accordingly.

The ultimate goal of SEO is to improve a website's visibility in search results, drive organic traffic, and increase the chances of attracting and converting users. By implementing effective SEO strategies, businesses can enhance their online presence and reach a wider audience.
