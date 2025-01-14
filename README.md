# Cross Platform Desktop Applications

This is a repository containing applications and code samples from the book [Cross Platform Desktop Applications With Node, Electron, and NW.js](https://manning.com/books/cross-platform-desktop-applications).

### Requirements ( I used )

- VS Code ( v1.82.2 )
  + Debugger for NWjs by ruakr
- Node.js ( v20.05.0 )
- NW.js ( v0.80.0 )
- Electron ( v21.1.1+ )

### Runtime Sequence
실행 환경 순서

- NW.js
  + nw.exe -> package.json -> "main": "index.html'

- electron.js
  + electron.exe -> package.json -> "main": "main.js" 
  + main.js -> BrowserWindow() -> win.loadURL("index.html" )

### Debugging

- NW.js
  + nw.js sdk 버전을 이용한 디버깅이다.
  + open index.html or open main.js
  + select [Debug][NWjs]index.html in Debug Options
  + F5 or Run -> Start Debugging
- Electron
  + Main Process( node.js ) + Render Process( chorome debugging )
  + open main.js or open index.html
  + BlahBlah

### Installing the code examples

    git clone git@github.com:paulbjensen/cross-platform-desktop-applications.git
    cd cross-platform-desktop-applications
    
### Browsing the examples

The apps and code samples are organised in folders that match the chapter that they appear in.

### Troubleshooting

If you run into any issues running the applications, please create an issue on this Github repository and I will take a look.

### License and Credits

&copy; 2016 Paul Jensen. All source code is licensed under the MIT License.  
&copy; 2023 MrMoonKr. All source code is licensed under the MIT License.  
