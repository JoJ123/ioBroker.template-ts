![Logo](admin/template.png)
# ioBroker.template-ts
=================

This is a template for the creation of an ioBroker adapter with TypeScript. While you don't need it, it serves as a nice starting point for developing your own adapter.

The **bare** branch only contains the main files and admin UI, no widget, no additional www files, no docs.

## Steps 
1. download and unpack this packet from github ```https://github.com/AlCalzone/ioBroker.template-ts/archive/bare.zip```
  or clone git repository ```git clone --depth=1 https://github.com/AlCalzone/ioBroker.template-ts.git```

2. download required npm packets. Write in ioBroker.template directory:

  ```npm install```
  
3. set name of this template. Call
  
  ```grunt rename --name=mynewname --email=email@mail.com --author="Author Name"```
  
  *mynewname* must be **lower** case and with no spaces.

  If grunt is not available, install grunt globally:
  
  ```npm install -g grunt-cli```
 
4. rename directory from *ioBroker.template-ts* (can be *ioBroker.template-bare*) to *iobroker.mynewname*

5. to use this template you should copy it into *.../iobroker/node_modules* directory and then create an instance for it with iobroker.admin

6. create your adapter:

  * you might want to start with main.ts (code running within iobroker) and admin/index.html (the adapter settings page).

  * [Adapter-Development-Documentation](https://github.com/ioBroker/ioBroker/wiki/Adapter-Development-Documentation),
  
  * [Installation, setup and first steps with an ioBroker Development Environment](https://github.com/ioBroker/ioBroker/wiki/Installation,-setup-and-first-steps-with-an-ioBroker-Development-Environment)
   
  * After any files in the *admin* dir are changed you must execute ```iobroker upload mynewname``` to see changes in admin console. 

7. change version: edit package.json and then call ```grunt p``` in your adapter directory.
  
8. share it with the community

## Changelog

#### 0.0.1
* (AlCalzone) initial release

## License
The MIT License (MIT)

Copyright (c) 2017 @@Author@@ <@@email@@>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
