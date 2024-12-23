# VoWiFi2024
Reference audio samples for the paper: Access Network requirements for 3GPP Voice over Wi-Fi (VoWiFi) service.

For the performance evaluation and network requirements identification, we have implemented a testbed using real HW and using the Wi-Fi Calling services of a real MNO, as in figure.

<img src="trials.png" width="500">

The reference voice sample file used at the sender side is reference.wav

In the folders, we have included the received voice samples with post-processing of PESQ (full-reference). The different testing conditions are as below:

| Test case  | Ranging parameter         | Values       |
|------------|---------------------------|--------------|
| Reference  | VoLTE and 3G call         | n.a.         |
| Delay      | one-way delay (no jitter) | 0-500 ms     |
| Jitter     | Per packet jitter         | 0-140 ms     |
| Bottleneck | Per call rate cap         | 54-80 Kbit/s |

The Delay test cases are not included, since delay alone is not affecting PESQ evaluation. Full analysis of the quality results under the different configurations is available on https://doi.org/10.1109/ACCESS.2024.3517740

Furthermore, we have included real traffic captures to confirm the traffic model obtained by analysis (including silence periods). 
The main outcomes  of such analysis are reported in the table below.

<img src="table1.png" width="400">


