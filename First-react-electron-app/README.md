create react app:
    npx create-react-app my_first_app

go into the newly created directory

npm i -D electron electron-builder concurrently wait-on

npm i cross-env electron-is-dev

after this go to the public directory and create 'electron.js' and paste the boiler code

go to package.json and create a property named 'main' and add 'public/electron.js' as its value(remove private property).
add description
add author
add build
add homepage

win.loadFile('index.html') to .loadURL

add path in electron.js 
and change .loadURL to isDev ? statement to load from local host if in development mode else load from build folder.

next change the scriupts before we can use them:
start to react-start
and similarly for build,test,eject

add new scripts :
electron-build
build
start


to change the icon follow instruction on 
<https://www.electron.build/icons>

And paste the image in the public folder.