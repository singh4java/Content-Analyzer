web-Analyzer
This is a web Analyzer micro service exposed as REST web service using spring boot and the JSoup Framework.

Getting Started
These instructions will get you a copy of the project up and running on your local machine.

Prerequisites
Java 8 maven Access to port 8088 on the local box where this code will be executed.

Installing
Clone the repository from git hub by running the following command git clone https://github.com/singh4java/Content-Analyzer.git

mvn package
or 

cd to web-Analyzer directory and run command 'mvn spring-boot:run' This will startup a standalone tomcat instance on port 8088.

to access the application in the browser enter
http://localhost:8088/wipro/webAnalyzer or http://localhost:8088/wipro/webAnalyzer?domain=http://wiprodigital.com

Request Parameters
url takes a parameter by name domain this will be the domain name which needs to be web crawled. 
By default this value is set http://wiprodigital.com/
----------------------------------------------------------------------------------------------------------------------

Request URL
http://localhost:8088/wipro/webAnalyzer?domain=https://google.com
Response JSON

{
linkName: "https://google.com",
childLinks: null,
externalLinks: [
"https://www.google.co.in/imghp?hl=en&tab=wi",
"https://maps.google.co.in/maps?hl=en&tab=wl",
"https://play.google.com/?hl=en&tab=w8",
"https://www.youtube.com/?gl=IN&tab=w1",
"https://news.google.co.in/nwshp?hl=en&tab=wn",
"https://mail.google.com/mail/?tab=wm",
"https://drive.google.com/?tab=wo",
"https://www.google.co.in/intl/en/options/",
"http://www.google.co.in/history/optout?hl=en",
"/preferences?hl=en",
"https://accounts.google.com/ServiceLogin?hl=en&passive=true&continue=https://www.google.com/",
"/advanced_search?hl=en-IN&authuser=0",
"/language_tools?hl=en-IN&authuser=0",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=hi&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAU",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=bn&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAY",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=te&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAc",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=mr&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAg",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=ta&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAk",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=gu&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAo",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=kn&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAs",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=ml&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCAw",
"https://www.google.com/setprefs?sig=0_eGp5YEN2SxZGOkKtYqJEzM4u6nE%3D&hl=pa&source=homepage&sa=X&ved=0ahUKEwibtOuw-rLaAhVFp48KHTeLCjsQ2ZgBCA0",
"/intl/en/ads/",
"http://www.google.co.in/services/",
"https://plus.google.com/104205742743787718296",
"/intl/en/about.html",
"https://www.google.com/setprefdomain?prefdom=IN&prev=https://www.google.co.in/&sig=__IGAC8YLbrG90y1MfopSwW6TOW30%3D",
"/intl/en/policies/privacy/",
"/intl/en/policies/terms/"
],
images: [
"/images/branding/googlelogo/1x/googlelogo_white_background_color_272x92dp.png"
]
}
