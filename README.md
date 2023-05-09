# PMR446-channels-for-CHIRP
Pre-configured settings for (CHIRP)[https://trac.chirp.danplanet.com/chirp_next/next-20230509/] reprogramming tool to tune a Baofeng UV-5R (and similiar) radios into PMR446 frequensies.

The 128 memory slots of the UV-5R are utilized for 8 PMR channels and 15 subchannels each of the 8 channels.

## Setting files
* The channel settings are in file `pmr_UV-5R.csv`. You can import it in the CHIRP. 
* Also, there's a file `pmr_UV-5R.img`, which contains channel settings **AND** my other radio settings. This file is for those people who just want their baofen to work as PMR without touching any of the settings themself. Most of the settings are the default, but few are tuned a bit, like lowered power-saving.

## subchannels i.e. tone i.e. CTCSS 
If you are not familiar with PMR, here's some basic information about subchannels. 
Subchannels (e.g. 3-13) use the same frequency as the main channel (e.g. 3-0), but they add an unhearable tone (sine wave), which is makes it possible for the receiving end to filter out other subchannels. This way multiple parties can operate on same frequency simultaneously without hearing each other. If you use the main channel, then you hear every subchannel, but no other subchannel hears you. So, I would recommended to use subchannels.

## Legal
Most baofeng radios are locked outside PMR446 frequensies, and these settings does no unlocking. Unlocking may be possible via other means, which are not covered here. In most european countries it is illegal to transmit on PMR446 frequencies using higher powers than 0.5W. This guide is e.g. for Australia and New Zealand where 5W transmitting power is legal.
