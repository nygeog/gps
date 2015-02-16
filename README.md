# gps
GPS devices, methods, information, etc. 



Why does GPS use so much more battery than any other antenna or sensor in a smartphone?

http://www.quora.com/Why-does-GPS-use-so-much-more-battery-than-any-other-antenna-or-sensor-in-a-smartphone/?share=1

GPS is expensive because it is a very slow communication channel—you need to communicate with three or four satellites for an extended duration at 50 bits per second. There is no time division as in other communication mechanisms, necessitating powering the antenna for the duration of any communication. Worse, while the GPS is on, the system cannot enter a sleep state. Mobile devices such as Android and the iPhone achieve their battery life largely because they can aggressively and quickly enter into and exit from sleep states. GPS prevents this.

GPS's battery draining behavior is most noticeable during the initial acquisition of the satellite's navigation message: the satellite's state, ephemeris, and almanac. Acquiring each satellite takes 12 to 30 seconds, but if the full almanac is needed, this can take up to 12 minutes. During all of this, your phone is unable to enter a deep sleep. A-GPS (Assisted GPS) partially solves this, by sending the navigational message to your mobile device over your cellular data network or even Wi-Fi. As the bandwidth of either of these greatly dwarves the 50bps of the GPS satellites, the time spent powering the GPS antenna or avoiding deep sleep is greatly reduced.

Nonetheless, even with A-GPS, using your GPS is a noticeable battery hog. This is again due not to powering the GPS itself, but by preventing the phone from going to sleep. Compounding the cost, most mapping software is processor-intense. A well-designed app can make a significant difference here; Google Maps boasts several optimizations to reduce battery consumption from GPS usage.
  
Written 30 Jul, 2013.
Upvote466
