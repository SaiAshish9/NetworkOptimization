# NetworkOptimization

```
Load JS Async:
```

<img width="859" alt="Screenshot 2024-08-19 at 12 43 25 PM" src="https://github.com/user-attachments/assets/fca92874-4920-4e0e-a8f8-be728e506b4a">

<img width="791" alt="Screenshot 2024-08-19 at 12 50 47 PM" src="https://github.com/user-attachments/assets/7f10e57d-38a9-48ab-848b-73889f3331ea">

```
Lazy Load Images

<img loading="lazy" src="" />
```

```
Load CSS Async:

<link rel="stylesheet" href="nonCritical.css" onload="this.media='all'" media="print" />
<link rel="stylesheet" href="critical.css" /> // default: media="all"

when media sets to print, media is set for other purpose. It loads async. onload is triggered media to all, now after loading style can be applied after things are ready.

Other ways to load css async via js

<link rel="preload" as="style" href="style.css" />

order:
style.css
critical.css
nonCritical.css

```

```
Preload Prefetch Preconnect

<script src="style.css" /> Priority: Highest
<html>
</html>
<script src="script.js" /> Priority: High
Network Tab
View Waterfall as well to see the way files are loaded


<link rel="preload" as="script" href="script.js" />
<link rel="preload" as="style" href="style.css" />
<script src="style.css" />
<html>
</html>
<script src="style.js" /> If we don't consume here warning will be thrown at console.
these two will be loaded first than other scripts and styles. These are critical and we want these files asap. Spotify benefited a lot.


<link rel="prefetch"" href="script.html" />
<link rel="prefetch" as="script" href="script.js" />
<link rel="prefetch" as="stylesheet" href="style.css" />

we need to be sure that user will visit them. Lowest priority. Other page.
On step 1 we prefetc for step 2, on step 2 we preftech for step 3


<link rel="preconnect" href="https://abc.com" />

loading content from other domain. cdn firebase
at some pt we need to fetch assets.
connection takes some ms. We can make the call beforehand. handshake
```

```
Progressive Images:
```

```

```

```
Responsive Images:
```

```

```


