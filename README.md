# Static-analysis-Js


###Regular expression for API key
#Amazon AWS
grep -Re "AKIA[0-9A-Z]{16}"
grep -RE "[0-9a-zA-Z/+]{40}"

#Bitlfy
grep -Re "[0-9a-zA-Z_]{5,31}"
grep -Re "R_[0-9a-f]{32}"

#Facebook
grep -Re "[0-9]{13,17}"
grep -Re "[0-9a-f]{32}"

#Flickr
grep -Re "[0-9a-f]{32}"
grep -Re "[0-9a-f]{16}"

#Foursquare 
grep -Re "[0-9A-Z]{48}"
grep -Re "[0-9A-Z]{48}"

#LinkedIn
grep -Re "[0-9a-z]{12}"
grep -Re "[0-9a-zA-Z]{16}"

#Twitter
grep -Re "[0-9a-zA-Z]{18,25}"
grep -Re "[0-9a-zA-Z]{35,44}"


Using Waybackurls:
go get github.com/tomnomnom/waybackurls
waybackurls internet.org | grep "\.js" | uniq | sort


Ref:
https://blog.appsecco.com/static-analysis-of-client-side-javascript-for-pen-testers-and-bug-bounty-hunters-f1cb1a5d5288

