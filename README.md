## So fügen Sie die Komplimente zu Ihrem MagicMirror hinzu
### Step 1: welches File soll benutzt werden.
folgende Files stehen momentan zur Verfügung: 

- **Philosophien des SWR3-Radios ```philo.json```


### Step 2: Change config
Open your config:
```bash
sudo nano ~/MagicMirror/config/config.js
```

Scrollen Sie, bis Sie das compliments module sehen können. Es sieht in etwa so aus
```javascript
{
    module: "compliments",
    position: "lower_third"
},
```
Change it to:

```javascript
{
    module: "compliments",
    position: "bottom_bar", 
    config: {
      remoteFile: "https://raw.githubusercontent.com/grimsi/MagicMirrorCompliments/main/philo.json",
      specialDayUnique: true,
      classes: "thin medium bright"
    },
```
Filosophie: https://www.swr3.de

# Visit MagicMirror!
[MagicMirror](https://github.com/MichMich/MagicMirror)
