#(tsconfig.json) including a not existing folder breaks the tsserver

Windows 10

VSCode 1.7.1 | 1.8.0-insider

Typescript 2.0.6 | 2.0.7 | 2.1.0-dev.20161107


- 1) start visual studio code
- 2) open Folder/Project: *bug-tsconfig-include-notexistingfolder*
- 3) npm install
- 4) open "./src/app.ts"
- 5) check if intellisense is working  => yes it's working
- 6) close "./src/app.ts"  (close all .ts or .tsx files)
- 7) open "./src/app.ts"
- 8) check if intellisense is working  => nope its not
- 9) add folder "./notexistingfolder"
- 10) restart visual studio code
- 11) no problems


(tsconfig.json)
including a not existing folder breaks the tsserver
