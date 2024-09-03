# PMR446-channels-for-CHIRP
Pre-configured settings for [CHIRP](https://trac.chirp.danplanet.com/chirp_next/next-20230509/) reprogramming tool to tune a Baofeng UV-5R (and similiar) radios into PMR446 frequensies with 4W transmit power.

128 memory slots of the UV-5R are utilized for 8 PMR channels and 15 subchannels. (128 = 8 * (1+15))

## Setting files
* The channel settings are in file `pmr_UV-5R.csv`. You can import it in the CHIRP. 

## subchannels i.e. tone i.e. CTCSS 
If you are not familiar with PMR, here's some basic information about subchannels. 
Subchannels (e.g. "3-13") use the same frequency as the main channel (e.g. "3-0"), but they add an unhearable tone (sine wave), which is makes it possible for the receiving end to filter out other subchannels. This way multiple parties can operate on same frequency simultaneously without hearing each other. If you use the main channel, then you hear every subchannel, but no other subchannel hears you. So, I would recommended to use subchannels.

## Legal
Most baofeng radios are locked outside PMR446 frequencies, and these CHIRP settings do not unlock the radio. These channels work only with the unlocked radio. Unlocking is probably possible, but it is not covered here. In most european countries it is illegal to transmit on PMR446 frequencies using higher powers than 0.5W. These CHIRP settings are for e.g. Australia and New Zealand where 5W transmit power is allowed. These channel settings can be modified to use 0.5W transmit power by opening the CSV file in a text editor, and searching and replacing all occurences of "4.0W" with "0.5W".
