# Mason Standard Google Tag Manager (GTM) Container

**The Mason Standard GTM Container is a pre-configured Google Tag Manager Container that is designed for use on George Mason University websites.**

## Key Features

* tracks page views, embedded YouTube video activity, and clicks on outbound, email, and file links, as well as user interaction with expandable content areas
* supports one Google Analytics property for the website as well as up to two additional roll-up properties

## Configuration

When deploying this container template into GTM containers used on other websites, you will need to customize the following items, all of which can be found in the folder called “00 standard configuration settings”.

* Variable: **Hostname - local** - Stores the host name (domain name) of the website on which the GTM container is implemented. Set this to the domain name of your website. Analytics will not fire unless the domain name of the website matched the domain name specified in this variable. This help to prevent GTM code from activating if inadvertently included on other websites, or when operating in a pre-production or testing environment.
* Variable: **UAID - local** - Stores the Google Analytics property ID number for the primary GA property used by the website. 
* Variable: **UAID - rollup01** - Stores the Google Analytics property ID number for the optional first GA roll-up property used by the website (typically the Mason university roll-up).  This is pre-set to use the Mason university roll-up, and typically does not need to be changed.
* Variable: **UAID - rollup02** - Stores the Google Analytics property ID number for the optional second GA roll-up property used by the website, if applicable. This is typically used for a unit- or department-level roll-up property.
* Trigger: **click - expandable area** - This trigger is responsible for sending the tracking information relating to clicks on expandable content areas. The trigger firing conditions must be set to indicate the CSS selector which identifies the elements used to expand expandable content areas.  This is pre-set to work for Mason standard Drupal websites. If your website is on a different platform, and uses expandable content areas, set this to a CSS selector which will identify the elements used to expand expandable content areas.



