# [Internet of Things] COVID's Communication Technology!
We heard a rumor that COVID was leveraging that smart city's 'light' technology for communication. Find out in detail on the technology and what is being transmitted.


# logicdata file

We are provided with a .logicdata file for the challenge. A quick google search shows that it is data from a Saleae logic analyser. We download the software from their [website](https://support.saleae.com/logic-software) to take a look at the file. 

We see what looks like a bunch of data packets, one of which looks like this:
![enter image description here](https://drive.google.com/uc?export=download&id=1dY63dCOfZAGo21OK-A_Zf5azBMWmbc-U)

## NEC IR Protocol
This data looks very similar to the NEC IR Protocol
![enter image description here](https://drive.google.com/uc?export=download&id=1yEE9V4L9cwoT1FRY9ZtfdpjRL1f740NB)

We can find a plugin for the Saleae software for the NEC IR protocol [here](https://github.com/kodizhuk/Salae-Logic-NEC-Analyzer), but when trying it out, it seems like it is unable to parse the data properly, showing no output, probably because of the 38kHz carrier frequency.

## Manual Decoding

The Saleae software allows us to export the data as a csv file, which we can use to decode the data.
![enter image description here](https://drive.google.com/uc?export=download&id=1MH-Q1Rjmx6B_K90rbaDYM7lqyznoeTSf)

