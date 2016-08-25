# fable-electron

Fable bindings and samples for Github Electron

## What's electron?

> The Electron framework lets you write cross-platform desktop applications using JavaScript, HTML and CSS. It is based on Node.js and Chromium and is used by the Atom editor and many other apps.
> https://github.com/electron/electron

Electron documentation official website: 
[http://electron.atom.io/docs/](http://electron.atom.io/docs/)


## How to run the samples?


### 1. Install electron

`npm install -g electron`
 
### 2. Navigate to any of the samples

Every sample have a `fableconfig.json` file, so you only need to run:

```
bash-3.2$ cd samples/material-ui/                                                                                                                                                                                                                                   
bash-3.2$ fable 
```

The `npm` packages should install and fable will compile the `fsx`.

```
bash-3.2$ fable                                                                                                                                                                                                                                                     
npm install                                                                                                                                                                                                                                                         
fable-compiler 0.5.6: Start compilation...                                                                                                                                                                                                                          
Compiled renderer.fsx at 5:49:52 PM                                                                                                                                                                                                                                 
Compiled main.fsx at 5:49:52 PM                                                                                                                                                                                                                                     
node node_modules/webpack/bin/webpack                                                                                                                                                                                                                               
Hash: 7cbedbac26f715a9ccf7                                                                                                                                                                                                                                          
Version: webpack 1.13.2                                                                                                                                                                                                                                             
Time: 1766ms                                                                                                                                                                                                                                                        
          Asset     Size  Chunks             Chunk Names                                                                                                                                                                                                            
        main.js  2.83 kB       0  [emitted]  main                                                                                                                                                                                                                   
    renderer.js  1.29 MB       1  [emitted]  renderer                                                                                                                                                                                                               
    main.js.map  3.24 kB       0  [emitted]  main                                                                                                                                                                                                                   
renderer.js.map  1.54 MB       1  [emitted]  renderer                                                                                                                                                                                                               
    + 371 hidden modules    
```

### 3. Run electron sample

When the compilation is done, there should be a `app/js/main.js`.
It is the entrypoint for electron.

To run the sample execute the following command:

```
bash-3.2$ npm run start                                                                                                                                                                                                                                             
                                                                                                                                                                                                                                                                    
> @ start /Users/[USERNAME]/Projects/fable-electron/samples/material-ui                                                                                                                                                                                            
> electron app/js/main.js 
```