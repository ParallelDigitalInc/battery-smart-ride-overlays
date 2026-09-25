# Battery Smart — ride-time overlay audio prototype

Clickable prototype of the six ride-time overlays (BaaS and Swap), with alert sounds and Hindi voice lines.

**Live:** https://paralleldigitalinc.github.io/battery-smart-ride-overlays/

## What's in it

| State | App | Sound | Voice line |
|---|---|---|---|
| Payment overdue / penalty | BaaS | Gentle chime | सोलह सौ रुपये का पेमेंट लेट है। अभी भरें, वरना पचास रुपये लेट फीस लगेगी। |
| Battery critical (5%) | BaaS | Urgent pulse | बैटरी सिर्फ़ पाँच परसेंट बची है। घर जाकर चार्ज करें। |
| Battery issue detected | BaaS | Urgent pulse | बैटरी में खराबी है। बैटरी बंद होने से पहले सर्विस सेंटर जाएं। |
| Battery not charging | BaaS | Gentle chime | बैटरी चार्ज नहीं हो रही। चार्जिंग बयालीस परसेंट पर रुक गई है। |
| Plan renewal overdue | Swap | Gentle chime | प्लान रिन्यू का पेमेंट लेट है। अभी रिन्यू करें, वरना पचास रुपये लेट फीस लगेगी। |
| Low charge to reach station (10%) | Swap | Urgent pulse | बैटरी सिर्फ़ दस परसेंट बची है। इंदिरानगर में नज़दीकी स्टेशन पर स्वैप करें। |

## Files

- `index.html` — the prototype. Self-contained: screens and audio are embedded, so it works offline.
- `audio/` — the same clips as separate files. `vo-*.m4a` are the voice lines; `ear-urgent.m4a` and `ear-gentle.m4a` are the alert sounds.

## Notes

- Screens are exported at 3× from the Figma file *Swap - BaaS (int)*, section "Section 3".
- The voice is a stand-in (Microsoft Swara, hi-IN neural voice). Final lines should be recorded with the production voice (e.g. ElevenLabs "Devi") under the same file names.
- The alert sounds are synthesised placeholders for a sound designer.
