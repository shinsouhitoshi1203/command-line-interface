@shinsouhitoshi1203
# `npm.cli` ～ getting started


> prerequisite: `cli starter pack`

## ⓪ definition 
1. `npm` stands for `node package manager`
2. a tool to manage libraries

`npm` is always installed when installing `nodejs`. 

to check the existant of    **[ npm ]** , 
type `npm -v` or `npm --version`

## ① initialize package > `package.json` 
```bash
npm init
```

> [ ⁉️ ] if you wish to skip this step and quickly move to **section 2 :: install libraries**,<br><br>
> type `npm init -y`

follow the instruction in your console window.

## ② install libraries
to install a library in npm, type 
```bash
npm install  lib1 [lib2 lib..] [--flag]
```

👍 `npm install react` &nbsp; `npm install vite react@17.0.2` &nbsp; `npm install css-loader --save-dev`

### explanation
1. `lib` is the library you want to install

    :smile: for example: `react` 
    <br><br>
    > if you want indicate **the `specific version`** of the library, follow this syntax: <br><br>
    > `library`**`@`**`ver` :arrow_right: *library at version*<br><br>
    > for example: `react-dom@18.0.2`

    <br/>

    > if you want indicate **the `latest version`** of the library, follow this syntax: <br><br>
    > `library`**`@`**`latest` :arrow_right: *library at latest*<br><br>
    > for example: `react-dom@latest`

    <br/>

    > more examples: `react@17.0.2` &nbsp;&nbsp; `sass`&nbsp;&nbsp; `babel`  

    <br/>

2. `(list of libraries)` is the list of libraries. each library is separated by space character (` `)


    :smile: for example: `react@17.0.2 react-dom@17.0.2`

3. *`--flag`* 
    
    the following flags are the most common flags when using the command

    | flag name | shorthand | how to use the flag |
    | ----- | ----- | ----- |
    | `--save-dev` | `-D` | only install libraries for development stage. this will be noted in `devDependencies` | 
    | `--global` | `-g` | install libraries globally | 


## ③ update libraries' version

to update a library, simply follow the structure like **[this](#explanation)**

```bash
npm update  lib1 [lib2 lib..] [--flag]
```

**but make sure to replace all `install` word with `update`**

👍 `npm update react` &nbsp; `npm update vite react@17.0.2` &nbsp; `npm update css-loader`

## ④ uninstall libraries

to uninstall a library, simply follow the structure like **[this](#②-install-libraries)**

```bash
npm uninstall  lib1 [lib2 lib..] [--flag]
```

**but make sure to replace all `install` word with `update`**

👍 `npm uninstall react` &nbsp; `npm uninstall vite react@17.0.2` &nbsp; `npm uninstall css-loader`
