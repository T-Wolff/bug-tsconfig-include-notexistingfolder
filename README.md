#(tsconfig.json) including a not existing folder breaks the tsserver

- Windows 10
- VSCode 1.7.1 | 1.8.0-insider
- Typescript 2.0.6 | 2.0.7 | 2.1.0-dev.20161107

1) start visual studio code<br>
2) open Folder/Project: *bug-tsconfig-include-notexistingfolder*<br>
3) npm install<br>
4) open "./src/app.ts"<br>
5) check if intellisense is working  => yes it's working<br>
6) close "./src/app.ts"  (close all .ts or .tsx files)<br>
7) open "./src/app.ts"<br>
8) check if intellisense is working  => nope its not<br>
9) add folder "./notexistingfolder"<br>
10) restart visual studio code<br>
11) no problems<br>
