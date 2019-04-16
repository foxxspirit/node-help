# Seting env variable for Windows, Linux, Mac OS for Node.js

## This is small guide made for pirple node master class.

There is a lot of people havig trouble with this, so here is examples on how
to set env variables for Node.js on Windows, Linux and Mac OS

We will run super simple script for this example. Script will just print out NODE_ENV to console so we can test that our env variable was set.

```javascript
// index.js
const ENV = process.env.NODE_ENV;
console.log(`The NODE_ENV has bean set to ${ENV}`);
```

### CMD (Windows)
```bat
C:\path\to\your\project> set NODE_ENV=production&&node index.js
``` 
```bat
C:\path\to\your\project> set NODE_ENV=production
C:\path\to\your\project> node index.js
```

### PowerShell (Windows)
```powershell
PS C:\path\to\your\project> $env:NODE_ENV="production"
PS C:\path\to\your\project> node index.js
```

```powershell
PS C:\path\to\your\project> $env:NODE_ENV="production";node index.js
```

### Linux and Mac OS
```bash
# Note that promts in linux can be customised, so your might look diffrent
# then in this example.
some-user@some-linux path/to/your/project $ NODE_ENV=production node index.js
```