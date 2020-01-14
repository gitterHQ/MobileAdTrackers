## As of January 14,2020 this list is no longer maintained.  After talks with PerfectSlayer, this list now replaces the Adaway list and I will help maintain it there.
## https://github.com/AdAway/adaway.github.io
## PerfectSlayer also made a slick domain sorting utility in the adaway repo that replicated some sorting to the list that I'd do in LibreOffice Calc to keep domains and subdomains clumped together.  it's in that repo under the /tools folder.  To run it you have to have node.js or some other javascript program and execute js index.js which will then read the contents of whatever is in the hosts.txt file in the main directory and sort the file outputted as formatted-hosts.txt.  Looks pretty!

# MobileAdTrackers
Taken from DNS logs, formatted in hostfile format.

Direct link to list:
https://raw.githubusercontent.com/jawz101/MobileAdTrackers/master/hosts

To give you an idea of why we need better mobile ad lists take a look at [Marketing Technology Landscape Supergraphic - Martec](https://chiefmartec.com/2019/04/marketing-technology-landscape-supergraphic-2019/).

Rationale: Other blocklists are fine for blocking desktop and browser-based domains but not too focused on mobile app traffic.

Apps and other resources interested in Android mobile privacy efforts:

|Utilities & Resources|
|---|
|[Koodous](https://koodous.com/apks) - [Play Store](https://play.google.com/store/apps/details?id=com.koodous.android),[Github](https://github.com/Koodous) Community-driven apk analysis + app that scans your apps for malware they've detected|
|[Exodus Privacy](https://exodus-privacy.eu.org/) - [Github](https://github.com/Exodus-Privacy),[F-Droid](https://www.f-droid.org/en/packages/org.eu.exodus_privacy.exodusprivacy/),[Play Store](https://play.google.com/store/apps/details?id=org.eu.exodus_privacy.exodusprivacy) France gave a privacy grant to these guys.  They have an app and a site.  I've submitted about domains and dug up the sdk information for about 20 or so companies from this very host file|
|[Yale Privacy Lab](https://privacylab.yale.edu) - [Github](https://github.com/YalePrivacyLab) Buddies with the Exodus Privacy project|
|[Data Transparency Lab](http://datatransparencylab.org) Funds several data privacy projects on this list.|
|[Lumen Privacy Monitor (formerly Project Haystack) - ICSI UC Berkeley](https://www.haystack.mobi/) - [Play Store](https://play.google.com/store/apps/details?id=edu.berkeley.icsi.haystack) Research project that made an app.  The app is novel because it is a local VPN that has you install a self-signed SSL certificate so it can decrypt encrypted traffic.  The traffic never leaves your device for analysis but what it does is scan all traffic for personally identifiable information and then passes it through to the destination.  This is how your NetGuard, AdGuard, ANTMonitor, Blokada, DNS66 use VPNs.  But only a few do SSL interception and only 2 (this and ANTMonitor) are designed to look for PII.|
|[Protect My Privacy(PMP) - Carnegie Mellon/Synergy Labs](http://www.android.protectmyprivacy.org) - [XPosed Repo](http://repo.xposed.info/module/org.synergylabs.pmpandroid) - Reasearch Project that kinda works but it's screwy when trying to control 3rd party library data independent of the host app. I like the idea, though: pass valid data to the host app but the 3rd party gets junk.  In theory.|
|[Recon - Northeastern University](https://recon.meddle.mobi) - another DTL grant project|
|[AntMonitor - UC Irvine](http://antmonitor.calit2.uci.edu) - [Play Store](https://play.google.com/store/apps/details?id=edu.uci.calit2.anteatermo), [YouTube presentation](https://www.youtube.com/watch?v=fymI9uM7TFo) - another DTL grant project. Similar to Lumen Privacy Monitor but very optimized.|
|[NetGuard](https://www.netguard.me/) - [Play Store](https://play.google.com/store/apps/details?id=eu.faircode.netguard),[Github](https://github.com/M66B/NetGuard/releases),[F-Droid](https://f-droid.org/en/packages/eu.faircode.netguard/) - One of the best traffic blockers for Android.  It's logging functions are one of the reasons I can make this host file.  Another thing it uniquely does is let you block one app from hitting a domain.  I can block facebook traffic from all apps but leave the Facebook app traffic alone.  That way Facebook can still be a social network for me but not an ad company.  Non-Playstore versions incorporate hostfile ad blocking.|
|[XprivacyLua/Pro](https://lua.xprivacy.eu/) - [Play Store](https://play.google.com/store/apps/details?id=eu.faircode.xlua.pro), [F-Droid](https://f-droid.org/packages/eu.faircode.xlua/), [Xposed Repo](http://repo.xposed.info/module/eu.faircode.xlua),[Github](https://github.com/M66B/XPrivacyLua) XPosed Module to hook into Android to pass fake data and identifiers to apps instead of what they try to get.|
|Dexplorer - [Play Store](https://play.google.com/store/apps/details?id=com.dexplorer) - lets you inspect an app on-device.  I find myself installing it frequently to see what 3rd party companies they have embedded in an app.|
|My Android Tools(Pro) - [Play Store](https://play.google.com/store/apps/details?id=cn.wq.myandroidtoolspro) dead link (I assume Google kicked them off because their app let you view and disable services, receivers, activities and content providers). find the free version on [apkmirror](https://www.apkmirror.com/apk/wangqi/my-android-tools/)|
|[Inspeckage - Package Inspector](http://ac-pm.github.io/Inspeckage/) - [Play Store](https://play.google.com/store/apps/details?id=mobi.acpm.inspeckage),[XPosed Repo](http://repo.xposed.info/module/mobi.acpm.inspeckage),[Github](https://github.com/ac-pm/Inspeckage) Sets up a web server on your device to let you inspect apps rom your computer.|
|[PyFunceble](https://funilrys.github.io/PyFunceble/) - [Github](https://github.com/funilrys/PyFunceble) Every hostfile maintainer should use this to validate their lists.  Companies close up shop all the time so having a huge hostfile of down sites makes no sense.|
|[OpenWPM - Princeton Web Transparency & Accountability Project](https://webtap.princeton.edu) - [Github](https://github.com/citp/OpenWPM) - automate Firefox to visit a bunch of sites.|
|[FilterLists.com](https://filterlists.com) - [Github](https://github.com/collinbarrett/FilterLists) A list of most every hostfile, IP blocklist, and AdBlock Plus syntax blocklist out there. Even the dumb ones. You'd think we could cooperate.|
