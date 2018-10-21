# Commands List

| ID   | MODE                           | COMMAND                                                      | DESCRIPTION                                                  |
| ---- | ------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1184 | Insert mode                    | CTRL- @                                                      | Insert the most recently inserted text and stop inserting    |
| 1185 | Insert mode                    | CTRL-A                                                       | Insert the most recently inserted text                       |
| 1187 | Insert mode                    | CTRL-C                                                       | Exit insert mode without checking for abbreviations unless 'insertmode' is set. |
| 1188 | Insert mode                    | CTRL-D                                                       | Remove a shiftwidth indentation in the current line          |
| 1189 | Insert mode                    | CTRL-E                                                       | Insert the character below the cursor                        |
| 1191 | Insert mode                    | CTRL-G CTRL-J                                                | Go down to the beginning of the column                       |
| 1192 | Insert mode                    | CTRL-G j                                                     | Go down to the beginning of the column                       |
| 1193 | Insert mode                    | CTRL-G <Down>                                                | Go down to the beginning of the column                       |
| 1194 | Insert mode                    | CTRL-G CTRL-K                                                | Go up to the beginning of the column                         |
| 1195 | Insert mode                    | CTRL-G k                                                     | Go up to the beginning of the column                         |
| 1196 | Insert mode                    | CTRL-G <Up>                                                  | Go up to the beginning of the column                         |
| 1197 | Insert mode                    | CTRL-G u                                                     | Start a new irrevocable edit                                 |
| 1198 | Insert mode                    | <BS>                                                         | Delete the character before the cursor                       |
| 1199 | Insert mode                    | {char1} <BS> {char2}                                         | Enter the combo (only enabled if the 'digraph' option is on) |
| 1200 | Insert mode                    | CTRL-H                                                       | Equivalent to <BS>                                           |
| 1201 | Insert mode                    | <Tab>                                                        | Insert the <Tab> character                                   |
| 1202 | Insert mode                    | CTRL-I                                                       | Equivalent to <Tab>                                          |
| 1203 | Insert mode                    | <NL>                                                         | Equivalent to <CR>                                           |
| 1204 | Insert mode                    | CTRL-J                                                       | Equivalent to <CR>                                           |
| 1205 | Insert mode                    | CTRL-K {char1} {char2}                                       | Enter the two-letter alphabet                                |
| 1206 | Insert mode                    | CTRL-L                                                       | When 'insertmode' is on: leave insert mode                   |
| 1207 | Insert mode                    | <CR>                                                         | Start a new trip                                             |
| 1208 | Insert mode                    | CTRL-M                                                       | Equivalent to <CR>                                           |
| 1209 | Insert mode                    | CTRL-N                                                       | Find the next match for the keyword in front of the cursor   |
| 1210 | Insert mode                    | CTRL-O                                                       | Executes a single command and then returns to insert mode    |
| 1211 | Insert mode                    | CTRL-P                                                       | Find the previous match of the keyword in front of the cursor |
| 1212 | Insert mode                    | CTRL-Q                                                       | Equivalent to CTRL-V unless it is used for terminal control flow |
| 1213 | Insert mode                    | CTRL-R {0-9a-z "% # *: =}                                    | Insert the contents of the register                          |
| 1214 | Insert mode                    | CTRL-R CTRL-R {0-9a-z "% # *: =}                             | Insert the contents of the register according to the original meaning |
| 1215 | Insert mode                    | CTRL-R CTRL-O {0-9a-z "% # *: =}                             | Insert the contents of the register according to the original meaning, and does not automatically indent |
| 1216 | Insert mode                    | CTRL-R CTRL-P {0-9a-z "% # *: =}                             | Insert the contents of the register according to the original meaning, and amend indentation |
| 1217 | Insert mode                    | CTRL-S                                                       | (For terminal control flow)                                  |
| 1218 | Insert mode                    | CTRL-T                                                       | Insert a shiftwidth indent in the current line               |
| 1219 | Insert mode                    | CTRL-U                                                       | Delete all the input characters of the current line          |
| 1220 | Insert mode                    | CTRL-V {char}                                                | Insert the next non-numeric character as it is               |
| 1221 | Insert mode                    | CTRL-V {number}                                              | Insert a single byte represented by a three-digit decimal number. |
| 1222 | Insert mode                    | CTRL-W                                                       | Delete the word before the cursor                            |
| 1223 | Insert mode                    | CTRL-X {mode}                                                | Enter CTRL-X sub-mode, see \| i_CTRL-X_index \|              |
| 1224 | Insert mode                    | CTRL-Y                                                       | Insert the character above the cursor                        |
| 1225 | Insert mode                    | CTRL-Z                                                       | When 'insertmode' is on: Pauses Vim                          |
| 1226 | Insert mode                    | <Esc>                                                        | End insert mode (unless 'insertmode' is on)                  |
| 1227 | Insert mode                    | CTRL- [                                                      | Equivalent to <Esc>                                          |
| 1228 | Insert mode                    | CTRL- CTRL-N                                                 | Into normal mode                                             |
| 1229 | Insert mode                    | CTRL- CTRL-G                                                 | Into the 'insertmode' specified mode                         |
| 1230 | Insert mode                    | CTRL-a-z                                                     | Reserved for expansion                                       |
| 1232 | Insert mode                    | CTRL-]                                                       | Switch abbreviations                                         |
| 1233 | Insert mode                    | CTRL- ^                                                      | Switch \|: lmap \| Use of mappings                           |
| 1234 | Insert mode                    | CTRL-_                                                       | When 'allowrevins' is on: changing the language (Hebrew, Persian, etc.) {only valid when compiled with the \| + rightleft \| feature} |
| 1235 | Insert mode                    | 0 CTRL-D                                                     | Delete all indentation of the current line                   |
| 1236 | Insert mode                    | ^ CTRL-D                                                     | Delete all indentation of the current line, restore indent indentation on the next line |
| 1237 | Insert mode                    | <Del>                                                        | Delete the cursor character                                  |
| 1238 | Insert mode                    | <Left>                                                       | Move the cursor one character to the left                    |
| 1239 | Insert mode                    | <S-Left>                                                     | Move the cursor one word to the left                         |
| 1240 | Insert mode                    | <C-Left>                                                     | Move the cursor one word to the left                         |
| 1241 | Insert mode                    | <Right>                                                      | Move the cursor one character to the right                   |
| 1242 | Insert mode                    | <S-Right>                                                    | Move the cursor one word to the right                        |
| 1243 | Insert mode                    | <C-Right>                                                    | Move the cursor one word to the right                        |
| 1244 | Insert mode                    | <Up>                                                         | Cursor up one line                                           |
| 1245 | Insert mode                    | <S-Up>                                                       | Equivalent to <PageUp>                                       |
| 1246 | Insert mode                    | <Down>                                                       | Cursor down one line                                         |
| 1247 | Insert mode                    | <S-Down>                                                     | Equivalent to <PageDown>                                     |
| 1248 | Insert mode                    | <Home>                                                       | Move the cursor to the beginning of the line                 |
| 1249 | Insert mode                    | <C-Home>                                                     | Move the cursor to the beginning of the file                 |
| 1250 | Insert mode                    | <End>                                                        | Move the cursor behind the end of the line                   |
| 1251 | Insert mode                    | <C-End>                                                      | Move the cursor to the end of the file                       |
| 1252 | Insert mode                    | <PageUp>                                                     | Full screen roll                                             |
| 1253 | Insert mode                    | <PageDown>                                                   | Full screen roll                                             |
| 1254 | Insert mode                    | <F1>                                                         | Equivalent to <Help>                                         |
| 1255 | Insert mode                    | <Help>                                                       | Stop insert mode display help window                         |
| 1256 | Insert mode                    | <Insert>                                                     | Toggle insert / replace mode                                 |
| 1257 | Insert mode                    | <LeftMouse>                                                  | Move the cursor to the mouse click                           |
| 1258 | Insert mode                    | <ScrollWheelDown>                                            | The window scrolls down three lines                          |
| 1259 | Insert mode                    | <S-ScrollWheelDown>                                          | The window scrolls down a full page                          |
| 1260 | Insert mode                    | <ScrollWheelUp>                                              | The window scrolls up three lines                            |
| 1261 | Insert mode                    | <S-ScrollWheelUp>                                            | The window scrolls up a full page                            |
| 1262 | Insert mode                    | <ScrollWheelLeft>                                            | The window scrolls six columns to the left                   |
| 1263 | Insert mode                    | <S-ScrollWheelLeft>                                          | The window scrolls the entire page to the left               |
| 1264 | Insert mode                    | <ScrollWheelRight>                                           | The window scrolls to the right by six columns               |
| 1265 | Insert mode                    | <S-ScrollWheelRight>                                         | The window scrolls one full page to the right                |
| 1266 | Sub-mode command               | CTRL-X CTRL-D                                                | Completed definition of the identifier                       |
| 1267 | Sub-mode command               | CTRL-X CTRL-E                                                | Roll on                                                      |
| 1268 | Sub-mode command               | CTRL-X CTRL-F                                                | Fill the file name                                           |
| 1269 | Sub-mode command               | CTRL-X CTRL-I                                                | Completion identifier                                        |
| 1270 | Sub-mode command               | CTRL-X CTRL-K                                                | Complement identifier from dictionary                        |
| 1271 | Sub-mode command               | CTRL-X CTRL-L                                                | Complete complete line                                       |
| 1272 | Sub-mode command               | CTRL-X CTRL-N                                                | Next make up                                                 |
| 1273 | Sub-mode command               | CTRL-X CTRL-O                                                | Almighty (omni) Complement                                   |
| 1274 | Sub-mode command               | CTRL-X CTRL-P                                                | Completed on a                                               |
| 1275 | Sub-mode command               | CTRL-X CTRL-S                                                | Spelling suggestions                                         |
| 1276 | Sub-mode command               | CTRL-X CTRL-T                                                | Complement identifier from thesaurus                         |
| 1277 | Sub-mode command               | CTRL-X CTRL-U                                                | Completed with 'completefunc'                                |
| 1278 | Sub-mode command               | CTRL-X CTRL-V                                                | Like: command line that completes                            |
| 1279 | Sub-mode command               | CTRL-X CTRL-Y                                                | Down                                                         |
| 1280 | Sub-mode command               | CTRL-X CTRL-]                                                | Complement the label                                         |
| 1281 | Sub-mode command               | CTRL-X s                                                     | Spelling suggestions                                         |
| 1283 | Normal mode                    | CTRL-A                                                       | Add N to the value at / after the cursor                     |
| 1284 | Normal mode                    | CTRL-B                                                       | Back (Back) scroll N screen                                  |
| 1285 | Normal mode                    | CTRL-C                                                       | Terminate the current (search) command                       |
| 1286 | Normal mode                    | CTRL-D                                                       | Scroll down N lines (default: half screen)                   |
| 1287 | Normal mode                    | CTRL-E                                                       | Scroll up N lines (Extra N lines)                            |
| 1288 | Normal mode                    | CTRL-F                                                       | Scrolls N screens forward                                    |
| 1289 | Normal mode                    | CTRL-G                                                       | Display the current file name and location                   |
| 1290 | Normal mode                    | <BS>                                                         | Equivalent to "h"                                            |
| 1291 | Normal mode                    | CTRL-H                                                       | Equivalent to "h"                                            |
| 1292 | Normal mode                    | <Tab>                                                        | Go to the Nth newer item in the jump table                   |
| 1293 | Normal mode                    | CTRL-I                                                       | Equivalent to <Tab>                                          |
| 1294 | Normal mode                    | <NL>                                                         | Equivalent to "j"                                            |
| 1295 | Normal mode                    | CTRL-J                                                       | Equivalent to "j"                                            |
| 1297 | Normal mode                    | CTRL-L                                                       | Redraw the screen                                            |
| 1298 | Normal mode                    | <CR>                                                         | Move the cursor to the first CHAR below the N line           |
| 1299 | Normal mode                    | CTRL-M                                                       | Equivalent to <CR>                                           |
| 1300 | Normal mode                    | CTRL-N                                                       | Equivalent to "j"                                            |
| 1301 | Normal mode                    | CTRL-O                                                       | Jump to the Nth oldest item in the jump table                |
| 1302 | Normal mode                    | CTRL-P                                                       | Equivalent to "k"                                            |
| 1303 | Normal mode                    | CTRL-Q                                                       | (For terminal control flow)                                  |
| 1304 | Normal mode                    | CTRL-R                                                       | Redo 'u' undo changes                                        |
| 1305 | Normal mode                    | CTRL-S                                                       | (For terminal control flow)                                  |
| 1306 | Normal mode                    | CTRL-T                                                       | Jump to the Nth oldest tag in the tag list                   |
| 1307 | Normal mode                    | CTRL-U                                                       | Upwards N lines (default: half screen)                       |
| 1308 | Normal mode                    | CTRL-V                                                       | Start visualization of column blocks                         |
| 1309 | Normal mode                    | CTRL-W {char}                                                | Window command, see \| CTRL-W \|                             |
| 1310 | Normal mode                    | CTRL-X                                                       | Subtract N from the value of the cursor position             |
| 1311 | Normal mode                    | CTRL-Y                                                       | N roll down                                                  |
| 1312 | Normal mode                    | CTRL-Z                                                       | Pause the program (or start a new shell)                     |
| 1314 | Normal mode                    | CTRL- CTRL-N                                                 | Enter normal mode (empty action)                             |
| 1315 | Normal mode                    | CTRL- CTRL-G                                                 | Into the 'insertmode' specified mode                         |
| 1316 | Normal mode                    | CTRL-a-z                                                     | Reserved for expansion                                       |
| 1317 | Normal mode                    | CTRL-                                                        | Others do not                                                |
| 1318 | Normal mode                    | CTRL-]                                                       | : ta to the cursor where the identifier                      |
| 1319 | Normal mode                    | CTRL- ^                                                      | Edit the Nth rotation file (equivalent to ": e #N")          |
| 1321 | Normal mode                    | <Space>                                                      | Equivalent to "l"                                            |
| 1322 | Normal mode                    | {motion} {filter} 2                                          | Filter Nmove text with the {filter} command                  |
| 1323 | Normal mode                    | {filter}                                                     | N lines are filtered by the {filter} command                 |
| 1324 | Normal mode                    | "{a-zA-Z0-9.% #: -"}                                         | Specify next register, {a-zA-Z0-9.% #: - "} used in uppercase (Add in uppercase) ({.% #:} Can only be used for placement) |
| 1325 | Normal mode                    | #                                                            | Search for the Nth occurrence of the cursor in the reverse direction |
| 1326 | Normal mode                    | $                                                            | The cursor moves after the end of line N down                |
| 1327 | Normal mode                    | %                                                            | Find the next (flower / square) parentheses in this row and go to their matching parentheses, or go to the matching note pair, or to the matching preprocessor command. |
| 1328 | Normal mode                    | {count}%                                                     | Go to the file's Nth position                                |
| 1329 | Normal mode                    | &                                                            | Repeat last: s                                               |
| 1330 | Normal mode                    | '{a-zA-Z0-9}                                                 | The cursor moves to the first CHAR on the line where the position marker {a-zA-Z0-9} is |
| 1331 | Normal mode                    | '                                                            | The cursor moves to the first CHAR on the line before the most recent jump |
| 1332 | Normal mode                    | '(                                                           | The cursor moves to the first CHAR on the line of the current sentence's head |
| 1333 | Normal mode                    | ')                                                           | The cursor moves to the first CHAR on the line where the tail of the current sentence is |
| 1334 | Normal mode                    | '<                                                           | The cursor moves to the first char of the beginning / beginning of the current buffer highlight. |
| 1335 | Normal mode                    | '>                                                           | The cursor moves to the first CHAR on the end of the current buffer highlight / past line. |
| 1336 | Normal mode                    | '[                                                           | The cursor moves to the first CHAR of the line where the text of the most recently manipulated / placed buffer is located in the current buffer |
| 1337 | Normal mode                    | ']                                                           | The cursor moves to the first CHAR of the line where the tail of the text of the most recent operation / placement of the current buffer |
| 1338 | Normal mode                    | '{                                                           | The cursor moves to the first CHAR on the line of the first paragraph of the current paragraph |
| 1339 | Normal mode                    | '}                                                           | The cursor moves to the first CHAR of the line where the tail of the current paragraph is located |
| 1340 | Normal mode                    | (                                                            | Cursor back N sentences                                      |
| 1341 | Normal mode                    | )                                                            | Cursor forward N sentences                                   |
| 1342 | Normal mode                    | *                                                            | Positive search for the Nth occurrence of the cursor in the identifier |
| 1343 | Normal mode                    | +                                                            | Equivalent to <CR>                                           |
| 1344 | Normal mode                    | ,                                                            | Reverse the most recent f, t, F, or TN times                 |
| 1345 | Normal mode                    | -                                                            | The cursor moves to the first CHAR above the N line          |
| 1346 | Normal mode                    | .                                                            | Repeat recent changes, the count is replaced by N.           |
| 1347 | Normal mode                    | / {pattern} <CR>                                             | The positive search for the Nth occurrence of {pattern}      |
| 1348 | Normal mode                    | / <CR>                                                       | Positive search for the most recent search using {pattern}   |
| 1349 | Normal mode                    | 0                                                            | The cursor moves to the first character of the line          |
| 1350 | Normal mode                    | 1,2,3,4,5,6,7,8,9                                            | Append to the command before giving a count                  |
| 1351 | Normal mode                    | :                                                            | Start entering the Ex command                                |
| 1352 | Normal mode                    | {count}:                                                     | Commencing with the Ex command, the line range from the current line to the N-1 line below is given |
| 1353 | Normal mode                    | ;                                                            | Repeat the last f, t, F, or TN times                         |
| 1354 | Normal mode                    | <{motion}                                                    | Move left Nmove text line a 'shiftwidth'                     |
| 1355 | Normal mode                    | <<                                                           | N-line left a shiftwidth                                     |
| 1356 | Normal mode                    | = {motion}                                                   | Filter Nmove lines of text with "indent"                     |
| 1357 | Normal mode                    | ==                                                           | Filter N lines with "indent"                                 |
| 1358 | Normal mode                    | > {motion}                                                   | Right shift Nmove text line a 'shiftwidth'                   |
| 1359 | Normal mode                    | >>                                                           | Right shift N lines a 'shiftwidth'                           |
| 1360 | Normal mode                    | ? {pattern} <CR>                                             | Reverse Search Nth occurrence of {pattern}                   |
| 1361 | Normal mode                    | ? <CR>                                                       | Reverse search for the {pattern} used by the most recent search |
| 1362 | Normal mode                    | @ {az}                                                       | Execute {az} register contents N times                       |
| 1363 | Normal mode                    | @:                                                           | Repeat last ":" command N times                              |
| 1364 | Normal mode                    | @@ @                                                         | Repeat @ {az} N times last time                              |
| 1365 | Normal mode                    | A                                                            | Append text at the end of the line N times                   |
| 1366 | Normal mode                    | B                                                            | Cursor reverse N WORD (string)                               |
| 1367 | Normal mode                    | ["x] C                                                       | From the cursor position to the end of the line, plus N-1 line to modify [to the buffer (translator Note: register should be the same below) x]; equivalent to "c $" |
| 1368 | Normal mode                    | ["x] D                                                       | Delete the position to the end of the line, plus the N-1 line character [to the buffer (see above) x]; equivalent to "d $" |
| 1369 | Normal mode                    | E                                                            | The cursor moves forward to the end of the Nth WORD          |
| 1370 | Normal mode                    | F {char}                                                     | The cursor moves left to the Nth occurrence of {char}        |
| 1371 | Normal mode                    | G                                                            | The cursor moves to the Nth line, the default is the last line |
| 1372 | Normal mode                    | H                                                            | Move the cursor to the top N of the screen                   |
| 1373 | Normal mode                    | I                                                            | Insert the text N times before the first CHAR of the line    |
| 1374 | Normal mode                    | J                                                            | Join (N) line; the default is 2                              |
| 1375 | Normal mode                    | K                                                            | Find the keyword where the cursor is located, using the definition of 'keywordprg' |
| 1376 | Normal mode                    | L                                                            | The cursor moves to the Nth line starting from the bottom of the screen |
| 1377 | Normal mode                    | M                                                            | Move the cursor to the middle of the screen                  |
| 1378 | Normal mode                    | N                                                            | Repeat the last '/' or '?' N times in the opposite direction |
| 1379 | Normal mode                    | O                                                            | Start a new line above the cursor and insert the text, repeating N times |
| 1380 | Normal mode                    | ["x] P                                                       | Place the cursor on the cursor [to buffer (see above) x] N times |
| 1381 | Normal mode                    | Q.                                                           | Switch to "Ex" mode                                          |
| 1382 | Normal mode                    | R                                                            | Enter the replacement mode: Overwrite the existing characters, repeat the text N-1 times |
| 1383 | Normal mode                    | ["x] S                                                       | Delete N lines [to buffer (see above) x]] and start typing; equivalent to "cc" |
| 1384 | Normal mode                    | T {char}                                                     | The cursor moves to the left before the Nth occurrence of {char} |
| 1385 | Normal mode                    | U                                                            | Undo all recent changes in his party                         |
| 1386 | Normal mode                    | V                                                            | Enter the line-oriented Visual mode                          |
| 1387 | Normal mode                    | W                                                            | Cursor forward N WORD                                        |
| 1388 | Normal mode                    | ["x] X                                                       | Delete N characters before the cursor [to buffer (see above) x] |
| 1389 | Normal mode                    | ["x] Y                                                       | Extract N lines [to buffer (see above) x]; equivalent to "yy" |
| 1390 | Normal mode                    | ZZ                                                           | If you have modified, save the current file, and then exit   |
| 1391 | Normal mode                    | ZQ                                                           | Quit the current file anyway                                 |
| 1392 | Normal mode                    | [{char}                                                      | Square brackets command (see below \| [\|)                   |
| 1393 | Normal mode                    | ] {char}                                                     | Square brackets command (see below \|] \|)                   |
| 1394 | Normal mode                    | ^                                                            | Move the cursor to the first CHAR on this line               |
| 1395 | Normal mode                    | _                                                            | The cursor moves to the first CHAR on line N - 1 below       |
| 1396 | Normal mode                    | `{a-zA-Z0-9}                                                 | Move the cursor to the position marker {a-zA-Z0-9}           |
| 1397 | Normal mode                    | `(                                                           | Cursor moves the beginning of the current sentence           |
| 1398 | Normal mode                    | `)                                                           | The cursor moves at the end of the current sentence          |
| 1399 | Normal mode                    | `<                                                           | Move the cursor to the beginning of the highlighted area     |
| 1400 | Normal mode                    | `>                                                           | Move the cursor to the end of the highlighted area           |
| 1401 | Normal mode                    | `[                                                           | The cursor moves to the beginning of the text of the last operation / placement |
| 1402 | Normal mode                    | `]                                                           | The cursor moves to the end of the text of the last operation / placement |
| 1403 | Normal mode                    | ``                                                           | The cursor moves the position of the last jump               |
| 1404 | Normal mode                    | `{                                                           | Move the cursor to the beginning of the current paragraph    |
| 1405 | Normal mode                    | `}                                                           | The cursor moves at the end of the current paragraph         |
| 1406 | Normal mode                    | a                                                            | Append the text N times at the cursor                        |
| 1407 | Normal mode                    | b                                                            | Cursor moves N words backwards                               |
| 1408 | Normal mode                    | ["x] c {motion}                                              | Delete Nmove text [to buffer (see above) x] and start editing |
| 1409 | Normal mode                    | ["x] cc                                                      | Delete N lines [to buffer (see above) x] and start editing   |
| 1410 | Normal mode                    | ["x] d {motion}                                              | Delete Nmove text [to buffer (see above) x]                  |
| 1411 | Normal mode                    | ["x] dd                                                      | Delete N lines [to buffer (see above) x]]                    |
| 1412 | Normal mode                    | do                                                           | Equivalent to ": diffget"                                    |
| 1413 | Normal mode                    | dp                                                           | Equivalent to ": diffput"                                    |
| 1414 | Normal mode                    | e                                                            | The cursor moves forward to the end of the Nth word          |
| 1415 | Normal mode                    | f {char}                                                     | Cursor right to the Nth occurrence of {char}                 |
| 1416 | Normal mode                    | g {char}                                                     | Expand command, see below \| g \|                            |
| 1417 | Normal mode                    | h                                                            | Move the cursor N characters to the left                     |
| 1418 | Normal mode                    | i                                                            | Insert the text N times before the cursor                    |
| 1419 | Normal mode                    | j                                                            | Cursor down N lines                                          |
| 1420 | Normal mode                    | k                                                            | Move the cursor N lines                                      |
| 1421 | Normal mode                    | l                                                            | Move the cursor N characters to the right                    |
| 1422 | Normal mode                    | m {A-Za-z}                                                   | Set the position marker at the cursor position {A-Za-z}      |
| 1423 | Normal mode                    | n                                                            | Repeat the last '/' or '?' N times                           |
| 1424 | Normal mode                    | o                                                            | Start a new line below the cursor and insert the text, repeating N times |
| 1425 | Normal mode                    | ["x] p                                                       | Place the text [from register x] N times after the cursor    |
| 1426 | Normal mode                    | q {0-9a-zA-Z "}                                              | Record the input characters to the command register {0-9a-zA-Z "} (uppercase for adding) |
| 1427 | Normal mode                    | q                                                            | (At the time of recording) stop recording                    |
| 1428 | Normal mode                    | q:                                                           | Edit in the command line window: Command line                |
| 1429 | Normal mode                    | q /                                                          | Edit / Command line in command line window                   |
| 1430 | Normal mode                    | q?                                                           | Edit in the command line window? Command line                |
| 1431 | Normal mode                    | r {char}                                                     | Replace N characters with {char}                             |
| 1432 | Normal mode                    | ["x] s                                                       | (Replace) Delete N characters [to buffer (see above) x] and start typing |
| 1433 | Normal mode                    | t {char}                                                     | Move the cursor to the right before the Nth occurrence of {char} |
| 1434 | Normal mode                    | u                                                            | Undo changed                                                 |
| 1435 | Normal mode                    | v                                                            | Start character-oriented Visual mode                         |
| 1436 | Normal mode                    | w                                                            | Cursor forward N words                                       |
| 1437 | Normal mode                    | ["x] x                                                       | Delete the first N characters of the cursor [to buffer (see above) x] |
| 1438 | Normal mode                    | ["x] y {motion}                                              | Extract Nmove text [to buffer (see above) x]                 |
| 1439 | Normal mode                    | ["x] yy                                                      | Extract N lines [to buffer (see above) x]                    |
| 1440 | Normal mode                    | z {char}                                                     | Commands starting with 'z', see below \| z \|                |
| 1441 | Normal mode                    | {                                                            | Cursor reverse N paragraphs                                  |
| 1442 | Normal mode                    | \|                                                           | Move the cursor to the Nth column                            |
| 1443 | Normal mode                    | }                                                            | The cursor moves forward N paragraphs                        |
| 1444 | Normal mode                    | ~                                                            | When 'tildeop' is off: Toggle the case of the N characters at the beginning of the cursor and move the cursor N characters to the right |
| 1445 | Normal mode                    | ~ {motion}                                                   | When 'tildeop' is on: Toggles the case of Nmove text         |
| 1446 | Normal mode                    | <C-End>                                                      | Equivalent to "G"                                            |
| 1447 | Normal mode                    | <C-Home>                                                     | Equivalent to "gg"                                           |
| 1448 | Normal mode                    | <C-Left>                                                     | Equivalent to "b"                                            |
| 1449 | Normal mode                    | <C-LeftMouse>                                                | ": ta" to the word where the mouse clicks                    |
| 1450 | Normal mode                    | <C-Right>                                                    | Equivalent to "w"                                            |
| 1451 | Normal mode                    | <C-RightMouse>                                               | Equivalent to "CTRL-T"                                       |
| 1452 | Normal mode                    | ["x] <Del>                                                   | Equivalent to "x"                                            |
| 1453 | Normal mode                    | {count} <Del>                                                | Delete the last digit of {count}                             |
| 1454 | Normal mode                    | <Down>                                                       | Equivalent to "j"                                            |
| 1455 | Normal mode                    | <End>                                                        | Equivalent to "$"                                            |
| 1456 | Normal mode                    | <F1>                                                         | Equivalent to <Help>                                         |
| 1457 | Normal mode                    | <Help>                                                       | Open the help window                                         |
| 1458 | Normal mode                    | <Home>                                                       | Equivalent to "0"                                            |
| 1459 | Normal mode                    | <Insert>                                                     | Equivalent to "i"                                            |
| 1460 | Normal mode                    | <Left>                                                       | Equivalent to "h"                                            |
| 1461 | Normal mode                    | <LeftMouse>                                                  | Move the cursor to the mouse click                           |
| 1462 | Normal mode                    | <MiddleMouse>                                                | Equivalent to the mouse click at "gP"                        |
| 1463 | Normal mode                    | <PageDown>                                                   | Equivalent to CTRL-F                                         |
| 1464 | Normal mode                    | <PageUp>                                                     | Equivalent to CTRL-B                                         |
| 1465 | Normal mode                    | <Right>                                                      | Equivalent to "l"                                            |
| 1466 | Normal mode                    | <RightMouse>                                                 | Start the visual mode, move the cursor to the mouse click    |
| 1467 | Normal mode                    | <S-Down>                                                     | Equivalent to CTRL-F                                         |
| 1468 | Normal mode                    | <S-Left>                                                     | Equivalent to "b"                                            |
| 1469 | Normal mode                    | <S-LeftMouse>                                                | Equivalent to the mouse click "*"                            |
| 1470 | Normal mode                    | <S-Right>                                                    | Equivalent to "w"                                            |
| 1471 | Normal mode                    | <S-RightMouse>                                               | Equivalent to the mouse click "#"                            |
| 1472 | Normal mode                    | <S-Up>                                                       | Equivalent to CTRL-B                                         |
| 1473 | Normal mode                    | <Undo>                                                       | Equivalent to "u"                                            |
| 1474 | Normal mode                    | <Up>                                                         | Equivalent to "k"                                            |
| 1475 | Normal mode                    | <ScrollWheelDown>                                            | The window scrolls down three lines                          |
| 1476 | Normal mode                    | <S-ScrollWheelDown>                                          | The window scrolls down a full page                          |
| 1477 | Normal mode                    | <ScrollWheelUp>                                              | The window scrolls up three lines                            |
| 1478 | Normal mode                    | <S-ScrollWheelUp>                                            | The window scrolls up a full page                            |
| 1479 | Normal mode                    | <ScrollWheelLeft>                                            | The window scrolls six columns to the left                   |
| 1480 | Normal mode                    | <S-ScrollWheelLeft>                                          | The window scrolls the entire page to the left               |
| 1481 | Normal mode                    | <ScrollWheelRight>                                           | The window scrolls to the right by six columns               |
| 1482 | Normal mode                    | <S-ScrollWheelRight>                                         | The window scrolls one full page to the right                |
| 1483 | Text object                    | a "                                                          | Double quotes string                                         |
| 1484 | Text object                    | a '                                                          | Single quotes string                                         |
| 1485 | Text object                    | a (                                                          | Equivalent to ab                                             |
| 1486 | Text object                    | a)                                                           | Equivalent to ab                                             |
| 1487 | Text object                    | a <                                                          | "A <> block from '<' to a matching '>'                       |
| 1488 | Text object                    | a>                                                           | Equivalent to a <                                            |
| 1489 | Text object                    | aB                                                           | "One big chunk" starts with "[{" to "]}" (with parentheses)  |
| 1490 | Text object                    | aW                                                           | "A string" (with a blank space)                              |
| 1491 | Text object                    | a [                                                          | "A [] block" from '[' to a matching ']'                      |
| 1492 | Text object                    | a]                                                           | Equivalent to a [                                            |
| 1493 | Text object                    | a`                                                           | Back quote string                                            |
| 1494 | Text object                    | ab                                                           | "One block" starts with "[(" to "])" (with parentheses)      |
| 1495 | Text object                    | ap                                                           | "A passage" (with a blank space)                             |
| 1496 | Text object                    | as                                                           | "A sentence" (with blank space)                              |
| 1497 | Text object                    | at                                                           | "A tab block" (with a blank space)                           |
| 1498 | Text object                    | aw                                                           | "A word" (with blank)                                        |
| 1499 | Text object                    | a {                                                          | Equivalent to aB                                             |
| 1500 | Text object                    | a}                                                           | Equivalent to aB                                             |
| 1501 | Text object                    | i "                                                          | Double quoted string, without quotation marks                |
| 1502 | Text object                    | i '                                                          | Single quotation mark string, without quotation marks        |
| 1503 | Text object                    | i (                                                          | Equivalent to ib                                             |
| 1504 | Text object                    | i)                                                           | Equivalent to ib                                             |
| 1505 | Text object                    | i <                                                          | "Contains <> blocks from '<' to matching '>'                 |
| 1506 | Text object                    | i>                                                           | Equivalent to i <                                            |
| 1507 | Text object                    | iB                                                           | "Contains chunks" from "[{" to "]}"                          |
| 1508 | Text object                    | iW                                                           | "Containing string"                                          |
| 1509 | Text object                    | i [                                                          | "Contains [] blocks from '[' to matching ']'                 |
| 1510 | Text object                    | i]                                                           | Equivalent to i [                                            |
| 1511 | Text object                    | i`                                                           | Back quote string, without backticks                         |
| 1512 | Text object                    | ib                                                           | "Internal block" changes from "[(" to "])"                   |
| 1513 | Text object                    | ip                                                           | "Contains paragraph"                                         |
| 1514 | Text object                    | is                                                           | "Containing Sentences"                                       |
| 1515 | Text object                    | it                                                           | "Contains the label block"                                   |
| 1516 | Text object                    | iw                                                           | "Containing words"                                           |
| 1517 | Text object                    | i {                                                          | Equivalent to iB                                             |
| 1518 | Text object                    | i}                                                           | Equivalent to iB                                             |
| 1519 | Window command                 | CTRL-W CTRL-B                                                | Equivalent to "CTRL-W b"                                     |
| 1520 | Window command                 | CTRL-W CTRL-C                                                | Equivalent to "CTRL-W c"                                     |
| 1521 | Window command                 | CTRL-W CTRL-D                                                | Equivalent to "CTRL-W d"                                     |
| 1522 | Window command                 | CTRL-W CTRL-F                                                | Equivalent to "CTRL-W f"                                     |
| 1523 | Window command                 | CTRL-W CTRL-G                                                | Equivalent to "CTRL-W g .."                                  |
| 1524 | Window command                 | CTRL-W CTRL-H                                                | Equivalent to "CTRL-W h"                                     |
| 1525 | Window command                 | CTRL-W CTRL-I                                                | Equivalent to "CTRL-W i"                                     |
| 1526 | Window command                 | CTRL-W CTRL-J                                                | Equivalent to "CTRL-W j"                                     |
| 1527 | Window command                 | CTRL-W CTRL-K                                                | Equivalent to "CTRL-W k"                                     |
| 1528 | Window command                 | CTRL-W CTRL-L                                                | Equivalent to "CTRL-W l"                                     |
| 1529 | Window command                 | CTRL-W CTRL-N                                                | Equivalent to "CTRL-W n"                                     |
| 1530 | Window command                 | CTRL-W CTRL-O                                                | Equivalent to "CTRL-W o"                                     |
| 1531 | Window command                 | CTRL-W CTRL-P                                                | Equivalent to "CTRL-W p"                                     |
| 1532 | Window command                 | CTRL-W CTRL-Q                                                | Equivalent to "CTRL-W q"                                     |
| 1533 | Window command                 | CTRL-W CTRL-R                                                | Equivalent to "CTRL-W r"                                     |
| 1534 | Window command                 | CTRL-W CTRL-S                                                | Equivalent to "CTRL-W s"                                     |
| 1535 | Window command                 | CTRL-W CTRL-T                                                | Equivalent to "CTRL-W t"                                     |
| 1536 | Window command                 | CTRL-W CTRL-V                                                | Equivalent to "CTRL-W v"                                     |
| 1537 | Window command                 | CTRL-W CTRL-W                                                | Equivalent to "CTRL-W w"                                     |
| 1538 | Window command                 | CTRL-W CTRL-X                                                | Equivalent to "CTRL-W x"                                     |
| 1539 | Window command                 | CTRL-W CTRL-Z                                                | Equivalent to "CTRL-W z"                                     |
| 1540 | Window command                 | CTRL-W CTRL-]                                                | Equivalent to "CTRL-W]"                                      |
| 1541 | Window command                 | CTRL-W CTRL- ^                                               | Equivalent to "CTRL-W ^"                                     |
| 1542 | Window command                 | CTRL-W CTRL-_                                                | Equivalent to "CTRL-W _"                                     |
| 1543 | Window command                 | CTRL-W +                                                     | Increase the current window height N lines                   |
| 1544 | Window command                 | CTRL-W -                                                     | Reduce the current window height N lines                     |
| 1545 | Window command                 | CTRL-W <                                                     | Reduce the current window width N columns                    |
| 1546 | Window command                 | CTRL-W =                                                     | All windows are the same width and height                    |
| 1547 | Window command                 | CTRL-W>                                                      | Increase the current window width N columns                  |
| 1548 | Window command                 | CTRL-W H                                                     | Move the current window to the far left                      |
| 1549 | Window command                 | CTRL-W J                                                     | Move the current window to the bottom                        |
| 1550 | Window command                 | CTRL-W K                                                     | Move the current window to the top                           |
| 1551 | Window command                 | CTRL-W L                                                     | Move the current window to the far right                     |
| 1552 | Window command                 | CTRL-W P                                                     | Jump to the preview window                                   |
| 1553 | Window command                 | CTRL-W R                                                     | Rotate the window up N times                                 |
| 1554 | Window command                 | CTRL-W S                                                     | Equivalent to "CTRL-W s"                                     |
| 1555 | Window command                 | CTRL-W T                                                     | Move the current window to a new tab                         |
| 1556 | Window command                 | CTRL-W W                                                     | Jump to the first Nth window (rewind)                        |
| 1557 | Window command                 | CTRL-W]                                                      | Split window and jump to the label where the cursor is located |
| 1558 | Window command                 | CTRL-W ^                                                     | Split window and edit rotation file N                        |
| 1559 | Window command                 | CTRL-W _                                                     | Set the current window height to N (default: try to be big)  |
| 1560 | Window command                 | CTRL-W b                                                     | Jump to the bottom of the window                             |
| 1561 | Window command                 | CTRL-W c                                                     | Close the current window (similar to \|: close \|)           |
| 1562 | Window command                 | CTRL-W d                                                     | Split the window and jump to the definition of the cursor    |
| 1563 | Window command                 | CTRL-W f                                                     | Split the window and jump to the file name where the cursor is located |
| 1564 | Window command                 | CTRL-W F                                                     | Split window and edit the cursor where the file name, and then jump to the line number given on the file name. |
| 1565 | Window command                 | CTRL-W g CTRL-]                                              | Split the window and execute \|: tjump \| on the label where the cursor is located |
| 1566 | Window command                 | CTRL-W g]                                                    | Split the window and execute \|: tselect \| on the label where the cursor is located |
| 1567 | Window command                 | CTRL-W g}                                                    | Execute \|: ptjump \| on the label where the cursor is located |
| 1568 | Window command                 | CTRL-W gf                                                    | Edit the file name of the cursor in the new tab              |
| 1569 | Window command                 | CTRL-W g F                                                   | Edit the file name of the cursor in the new tab and jump to the line number given after the file name. |
| 1570 | Window command                 | CTRL-W h                                                     | Jump to the left Nth window (stop on the first window)       |
| 1571 | Window command                 | CTRL-W i                                                     | Split the window and jump to the statement of the identifier where the cursor is located |
| 1572 | Window command                 | CTRL-W j                                                     | Jump to the Nth window below (stop on the last window)       |
| 1573 | Window command                 | CTRL-W k                                                     | Jump to the top Nth window (stop on the first window)        |
| 1574 | Window command                 | CTRL-W l                                                     | Jump to the right of the Nth window (stop on the last window) |
| 1575 | Window command                 | CTRL-W n                                                     | Open a new window, N rows high                               |
| 1576 | Window command                 | CTRL-W o                                                     | Close all windows except the current one (similar to \|: only \|) |
| 1577 | Window command                 | CTRL-W p                                                     | Go to the previous (recently visited) window                 |
| 1578 | Window command                 | CTRL-W q                                                     | Quit the current window (similar to \|: quit \|)             |
| 1579 | Window command                 | CTRL-W r                                                     | Rotate the window down N times                               |
| 1580 | Window command                 | CTRL-W s                                                     | Split the current window into two parts, the new window N rows high |
| 1581 | Window command                 | CTRL-W t                                                     | Jump to the top window                                       |
| 1582 | Window command                 | CTRL-W v                                                     | Vertical split the current window, the new window N column width |
| 1583 | Window command                 | CTRL-W w                                                     | Go to the back of the Nth window (rewind)                    |
| 1584 | Window command                 | CTRL-W x                                                     | Exchange current and Nth window (default: next window)       |
| 1585 | Window command                 | CTRL-W z                                                     | Close the preview window                                     |
| 1586 | Window command                 | CTRL-W \|                                                    | Set the window width to N columns                            |
| 1587 | Window command                 | CTRL-W}                                                      | In the preview window shows the cursor where the label       |
| 1588 | Window command                 | CTRL-W <Down>                                                | Equivalent to "CTRL-W j"                                     |
| 1589 | Window command                 | CTRL-W <Up>                                                  | Equivalent to "CTRL-W k"                                     |
| 1590 | Window command                 | CTRL-W <Left>                                                | Equivalent to "CTRL-W h"                                     |
| 1591 | Window command                 | CTRL-W <Right>                                               | Equivalent to "CTRL-W l"                                     |
| 1592 | Square brackets command        | [CTRL-D                                                      | Jump to the first #define that matches the word where the cursor is in the current file and the headers it contains, starting from the current file's head |
| 1593 | Square brackets command        | [CTRL-I                                                      | Jump to the first file in the current file and it contains the header file matching the cursor position, starting from the current file header |
| 1594 | Square brackets command        | [#                                                           | The cursor moves to the first Nth unmatched # if, # else, or #ifdef |
| 1595 | Square brackets command        | ['                                                           | Move the cursor to the front lowercase position marker and position it on the first non-blank character in the line it is in |
| 1596 | Square brackets command        | [(                                                           | The cursor moves to the first Nth unmatched '('              |
| 1597 | Square brackets command        | [*                                                           | Equivalent to"[/"                                            |
| 1598 | Square brackets command        | [`                                                           | Move the cursor to the previous lowercase mark               |
| 1599 | Square brackets command        | [/                                                           | The cursor moves to the beginning of the Nth C comment in front |
| 1600 | Square brackets command        | [D                                                           | Lists all the definitions of words that match the cursor in the current file and the header files it contains, starting at the head of the current file |
| 1601 | Square brackets command        | [I                                                           | Lists all the positions in the current file and the header files it contains matching the word the cursor is located from the head of the current file |
| 1602 | Square brackets command        | [P                                                           | Equivalent to "[p"                                           |
| 1603 | Square brackets command        | [[                                                           | Cursor back N bar                                            |
| 1604 | Square brackets command        | []                                                           | Cursor back N SECTION                                        |
| 1605 | Square brackets command        | [c                                                           | Cursor back N changes where the beginning                    |
| 1606 | Square brackets command        | [d                                                           | Display the first #define that matches the word in the current file and the header it contains, starting with the current file's head |
| 1607 | Square brackets command        | [f                                                           | Equivalent to "gf"                                           |
| 1608 | Square brackets command        | [i                                                           | Shows the first file in the current file and it contains the header file matching the cursor position, starting from the current file header |
| 1609 | Square brackets command        | [m                                                           | Cursor back to the beginning of N member functions           |
| 1610 | Square brackets command        | [p                                                           | Similar to "P", but adjusts the indentation of the current line |
| 1611 | Square brackets command        | [s                                                           | Move to the previous misspelled word                         |
| 1612 | Square brackets command        | [z                                                           | Move to the beginning of the open fold                       |
| 1613 | Square brackets command        | [{                                                           | Cursor back N unmatched '{'                                  |
| 1614 | Square brackets command        | [<MiddleMouse>                                               | Equivalent to "[p"                                           |
| 1615 | Square brackets command        | ] CTRL-D                                                     | Jump to the first #define that matches the word where the cursor is in the current file and the headers it contains, starting at the cursor position |
| 1616 | Square brackets command        | ] CTRL-I                                                     | Jump to the first position in the current file and the header file it contains matching the word where the cursor is located, starting from the cursor position |
| 1617 | Square brackets command        | ] #                                                          | The cursor moves to the Nth unmatched #endif, # else         |
| 1618 | Square brackets command        | ] '                                                          | The cursor moves to the lowercase position marker, positioned on the first non-whitespace of the line in which it is located |
| 1619 | Square brackets command        | ] (                                                          | The cursor moves to the Nth unmatched ')'                    |
| 1620 | Square brackets command        | ] *                                                          | Equivalent to"]/"                                            |
| 1621 | Square brackets command        | ] `                                                          | The cursor moves to the next lowercase mark                  |
| 1622 | Square brackets command        | ] /                                                          | The cursor moves to the end of the Nth C comment             |
| 1623 | Square brackets command        | ] D                                                          | Lists all the definitions of words that match the cursor in the current file and the header files it contains, starting at the cursor position |
| 1624 | Square brackets command        | ] I                                                          | Lists all the locations in the current file and the header files it contains matching the word in the cursor, starting from the cursor position |
| 1625 | Square brackets command        | ] P                                                          | Equivalent to "[p"                                           |
| 1626 | Square brackets command        | ]]                                                           | Cursor forward N bars                                        |
| 1628 | Square brackets command        | ] c                                                          | Cursor forward N changes where                               |
| 1629 | Square brackets command        | ] d                                                          | Display the first #define that matches the word in the current file and the header file it contains, starting at the cursor position |
| 1630 | Square brackets command        | ] f                                                          | Equivalent to "gf"                                           |
| 1631 | Square brackets command        | ] i                                                          | Display the first one in the current file and the headers it contains matching the cursor position, starting from the cursor position |
| 1632 | Square brackets command        | ] m                                                          | The cursor advances N member functions to the end            |
| 1633 | Square brackets command        | ] p                                                          | Similar to "p", but adjust the indentation of the current line |
| 1634 | Square brackets command        | ] s                                                          | Move to the next misspelled word                             |
| 1635 | Square brackets command        | ]z                                                           | Move to the end of the open fold                             |
| 1636 | Square brackets command        | ] {                                                          | Cursor forward N unmatched '}'                               |
| 1637 | Square brackets command        | ] <MiddleMouse>                                              | Equivalent to "] p"                                          |
| 1638 | Commands starting with 'g'     | g CTRL-A                                                     | Only when compiled with MEM_PROFILE when there is definition: Dump memory content |
| 1639 | Commands starting with 'g'     | g CTRL-G                                                     | The current cursor position is displayed                     |
| 1640 | Commands starting with 'g'     | g CTRL-H                                                     | Start select column block mode                               |
| 1641 | Commands starting with 'g'     | g CTRL-]                                                     | \|: tjump \| on the label where the cursor is                |
| 1642 | Commands starting with 'g'     | g #                                                          | Similar to "#" but without the "<" and ">"                   |
| 1643 | Commands starting with 'g'     | g $                                                          | 'wrap' turns off to the currently visible character on the far right screen 'wrap' turns on to the rightmost character of the current screen line when it is closed |
| 1644 | Commands starting with 'g'     | g &                                                          | Repeat on all lines last ": s"                               |
| 1645 | Commands starting with 'g'     | g '{mark}                                                    | Similar to \| '\|, but does not change the jump table        |
| 1646 | Commands starting with 'g'     | g` {mark}                                                    | Similar to `` \|, but does not change the table jump table   |
| 1647 | Commands starting with 'g'     | g *                                                          | Similar to "*", but not "<" and ">"                          |
| 1648 | Commands starting with 'g'     | g0                                                           | 'wrap' turns off to the current line The leftmost character on the far left screen, when the 'wrap' character is on, goes to the current screen line |
| 1649 | Commands starting with 'g'     | g8                                                           | Display the hexadecimal bytecode of the UTF-8 character where the cursor is located |
| 1650 | Commands starting with 'g'     | g <                                                          | Display the last command output                              |
| 1651 | Commands starting with 'g'     | g?                                                           | Rot13 encoding operator                                      |
| 1652 | Commands starting with 'g'     | g ??                                                         | Rot13 encoding the current line                              |
| 1653 | Commands starting with 'g'     | g? g?                                                        | Rot13 encoding the current line                              |
| 1654 | Commands starting with 'g'     | gD                                                           | The definition of the word where the cursor of the current file is located |
| 1655 | Commands starting with 'g'     | gE                                                           | Reverse transfer to the end of the previous WORD             |
| 1656 | Commands starting with 'g'     | gH                                                           | Start select line mode                                       |
| 1657 | Commands starting with 'g'     | gI                                                           | Similar to "I", but always starts with the first column      |
| 1658 | Commands starting with 'g'     | gJ                                                           | Connect the line, do not insert a space                      |
| 1659 | Commands starting with 'g'     | ["x] gP                                                      | Place the text in the light label N [from register x], the cursor remains after the text is inserted |
| 1660 | Commands starting with 'g'     | gR                                                           | Enter the virtual replacement mode                           |
| 1661 | Commands starting with 'g'     | gU {motion}                                                  | Makes Nmove text all uppercase                               |
| 1662 | Commands starting with 'g'     | gV                                                           | When performing a map or menu in selection mode, do not repeatedly select past viewable areas |
| 1663 | Commands starting with 'g'     | g]                                                           | : tselect to the label where the cursor is located           |
| 1664 | Commands starting with 'g'     | g ^                                                          | 'wrap' turns off to the current line The leftmost non-whitespace character visible on the screen 'wrap' opens to the leftmost non-whitespace of the current screen line |
| 1665 | Commands starting with 'g'     | ga                                                           | Prints the ascii value of the character where the cursor is  |
| 1666 | Commands starting with 'g'     | gd                                                           | Go to the current function definition of the word where the cursor is |
| 1667 | Commands starting with 'g'     | ge                                                           | Reverse to the end of the previous word                      |
| 1668 | Commands starting with 'g'     | gf                                                           | Start editing the current cursor corresponding to the name of the file |
| 1669 | Commands starting with 'g'     | gF                                                           | Start editing the cursor where the file name and jump to the file name after the line number. |
| 1670 | Commands starting with 'g'     | gg                                                           | The cursor moves to the Nth line, the default is the first line |
| 1671 | Commands starting with 'g'     | gh                                                           | Start selecting mode                                         |
| 1672 | Commands starting with 'g'     | gi                                                           | Similar to "i", but first moved to the \| '^ \| position marker |
| 1673 | Commands starting with 'g'     | gj                                                           | Similar to "j", but down 'N' when screen wrap opens          |
| 1674 | Commands starting with 'g'     | gk                                                           | Similar to "k", but up to N screen lines when 'wrap' is on   |
| 1675 | Commands starting with 'g'     | gm                                                           | Go to the middle of the screen line that character           |
| 1676 | Commands starting with 'g'     | go                                                           | The cursor moves to the Nth byte of the buffer               |
| 1677 | Commands starting with 'g'     | ["x] gp                                                      | Place text [after register x] N times behind the cursor with the cursor behind |
| 1678 | Commands starting with 'g'     | gq {motion}                                                  | Typographic Nmove text                                       |
| 1679 | Commands starting with 'g'     | gr {char}                                                    | The virtual substitution of N characters is {char}           |
| 1680 | Commands starting with 'g'     | gs                                                           | Sleep N seconds (default 1)                                  |
| 1681 | Commands starting with 'g'     | gu {motion}                                                  | Makes all Nmove text lowercase                               |
| 1682 | Commands starting with 'g'     | gv                                                           | Reselect the last visible area                               |
| 1683 | Commands starting with 'g'     | gw {motion}                                                  | Type Nmove text and keep the cursor position                 |
| 1684 | Commands starting with 'g'     | gx                                                           | Executes the application with the file name under the cursor (\| netrw \| plugin) |
| 1685 | Commands starting with 'g'     | g {motion}                                                   | Call 'operatorfunc'                                          |
| 1686 | Commands starting with 'g'     | g ~ {motion}                                                 | Change the case of Nmove text                                |
| 1687 | Commands starting with 'g'     | g <Down>                                                     | Equivalent to "gj"                                           |
| 1688 | Commands starting with 'g'     | g <End>                                                      | Equivalent to "g $"                                          |
| 1689 | Commands starting with 'g'     | g <Home>                                                     | Equivalent to "g0"                                           |
| 1690 | Commands starting with 'g'     | g <LeftMouse>                                                | Equivalent to <C-LeftMouse>                                  |
| 1691 | Commands starting with 'g'     | g <MiddleMouse>                                              | Equivalent to <C-MiddleMouse>                                |
| 1692 | Commands starting with 'g'     | g <RightMouse>                                               | Equivalent to <C-RightMouse>                                 |
| 1693 | Commands starting with 'g'     | g <Up>                                                       | Equivalent to "gk"                                           |
| 1694 | 'z' the beginning of the order | z <CR>                                                       | Redraw, the cursor moves to the top of the window the first non-blank characters |
| 1695 | 'z' the beginning of the order | z {height} <CR>                                              | Redraw, making the height of the window {height} line        |
| 1696 | 'z' the beginning of the order | z +                                                          | Move the cursor to the Nth line (the default is the first line after the window), the other with "z <CR>" |
| 1697 | 'z' the beginning of the order | z-                                                           | Redraw, the cursor moves to the first non-whitespace in the last line of the window |
| 1698 | 'z' the beginning of the order | z.                                                           | Redraw, the cursor moves to the first non-blank character in the middle of the window |
| 1699 | 'z' the beginning of the order | z =                                                          | Give spelling advice                                         |
| 1700 | 'z' the beginning of the order | zA                                                           | Recursively open a closed fold or close an open fold         |
| 1701 | 'z' the beginning of the order | zC                                                           | Recursively close the fold                                   |
| 1702 | 'z' the beginning of the order | zD                                                           | Recursively delete the fold                                  |
| 1703 | 'z' the beginning of the order | zE                                                           | Remove all the folds                                         |
| 1704 | 'z' the beginning of the order | zF                                                           | Create a fold for N lines                                    |
| 1705 | 'z' the beginning of the order | zG                                                           | Mark words as spelling correctly (good)                      |
| 1706 | 'z' the beginning of the order | zM                                                           | Set 'foldlevel' to zero                                      |
| 1707 | 'z' the beginning of the order | zN                                                           | Set 'foldenable'                                             |
| 1708 | 'z' the beginning of the order | zO                                                           | Recursively open the fold                                    |
| 1709 | 'z' the beginning of the order | zR                                                           | Set 'foldlevel' to the maximum fold level                    |
| 1710 | 'z' the beginning of the order | zW                                                           | Mark words as misspelled                                     |
| 1711 | 'z' the beginning of the order | zX                                                           | Reapply 'foldlevel'                                          |
| 1712 | 'z' the beginning of the order | z ^                                                          | Move the cursor to the Nth line (the default is the line before the window), the other with the "z-" |
| 1713 | 'z' the beginning of the order | za                                                           | Open the closed fold, or close the open fold                 |
| 1714 | 'z' the beginning of the order | zb                                                           | Redraw, the cursor at the bottom of the window               |
| 1715 | 'z' the beginning of the order | zc                                                           | Close the fold                                               |
| 1716 | 'z' the beginning of the order | zd                                                           | Remove the fold                                              |
| 1717 | 'z' the beginning of the order | ze                                                           | When 'wrap' is off, horizontal scrolling positions the cursor to the end of the screen (far right) |
| 1718 | 'z' the beginning of the order | zf {motion}                                                  | Create a fold for Nmove text                                 |
| 1719 | 'z' the beginning of the order | zg                                                           | Mark words as spelling correctly (good)                      |
| 1720 | 'z' the beginning of the order | zh                                                           | When 'wrap' is off, horizontally scrolls the screen N characters horizontally |
| 1721 | 'z' the beginning of the order | zi                                                           | Switch 'foldenable'                                          |
| 1722 | 'z' the beginning of the order | zj                                                           | Move to the beginning of the next fold                       |
| 1723 | 'z' the beginning of the order | zk                                                           | Move to the end of the previous fold                         |
| 1724 | 'z' the beginning of the order | zl                                                           | When 'wrap' is off, horizontally scrolls the screen by N characters |
| 1725 | 'z' the beginning of the order | zm                                                           | Subtract one from 'foldlevel'                                |
| 1726 | 'z' the beginning of the order | zn                                                           | Reset 'foldenable'                                           |
| 1727 | 'z' the beginning of the order | zo                                                           | Open the fold                                                |
| 1728 | 'z' the beginning of the order | zr                                                           | Add one to 'foldlevel'                                       |
| 1729 | 'z' the beginning of the order | zs                                                           | When 'wrap' is off, horizontal scrolling moves the cursor to the beginning of the screen (far left) |
| 1730 | 'z' the beginning of the order | zt                                                           | Redraw, the cursor moves to the top of the window            |
| 1731 | 'z' the beginning of the order | zw                                                           | Mark words as misspelled                                     |
| 1732 | 'z' the beginning of the order | zv                                                           | Open enough folds to make the current line visible           |
| 1733 | 'z' the beginning of the order | zx                                                           | Reapply 'foldlevel' then execute "zv"                        |
| 1734 | 'z' the beginning of the order | zz                                                           | Redraw, move the cursor to the middle of the window          |
| 1735 | 'z' the beginning of the order | z <Left>                                                     | Equivalent to "zh"                                           |
| 1736 | 'z' the beginning of the order | z <Right>                                                    | Equivalent to "zl"                                           |
| 1737 | Visual mode                    | CTRL- CTRL-N                                                 | End visual mode                                              |
| 1738 | Visual mode                    | CTRL- CTRL-G                                                 | Go to the mode specified by 'insertmode'                     |
| 1739 | Visual mode                    | CTRL-C                                                       | End visual mode                                              |
| 1740 | Visual mode                    | CTRL-G                                                       | Switching between the selection mode and the visual mode     |
| 1741 | Visual mode                    | <BS>                                                         | Select mode: Delete the highlighted area                     |
| 1742 | Visual mode                    | CTRL-H                                                       | It is equivalent to <BS>                                     |
| 1743 | Visual mode                    | CTRL-O                                                       | Visual selection mode is switched to the mode, the next command is limited to |
| 1744 | Visual mode                    | CTRL-V                                                       | Visual mode such blockwise or visual mode exit               |
| 1745 | Visual mode                    | <Esc>                                                        | VISUAL mode has ended                                        |
| 1746 | Visual mode                    | CTRL-]                                                       | Jump to highlight the label                                  |
| 1747 | Visual mode                    | ! {Filter}                                                   | Filter the highlighted line by an external command {filter}  |
| 1748 | Visual mode                    | :                                                            | Line highlighting is used as a range, start a command line   |
| 1749 | Visual mode                    | <                                                            | Left a bright line 'shiftwidth'                              |
| 1750 | Visual mode                    | =                                                            | {Equalprg} with the filter specified external program option highlighted lines |
| 1751 | Visual mode                    | >                                                            | A right row highlighting 'shiftwidth'                        |
| 1752 | Visual mode                    | A                                                            | The block mode: Additional same text line highlighted in all the regions |
| 1753 | Visual mode                    | C                                                            | Delete the highlighted lines, and start insert               |
| 1754 | Visual mode                    | D                                                            | Delete the highlighted lines                                 |
| 1755 | Visual mode                    | I                                                            | Column mode: The same text lines until all highlighted       |
| 1756 | Visual mode                    | J                                                            | Join the highlighted lines                                   |
| 1757 | Visual mode                    | K                                                            | Running on the highlight region 'keywordprg'                 |
| 1758 | Visual mode                    | O                                                            | Horizontally moves to an area of the other side              |
| 1759 | Visual mode                    | Q.                                                           | Ex mode does not start                                       |
| 1760 | Visual mode                    | R                                                            | Delete the highlighted line and starts Insert                |
| 1761 | Visual mode                    | S                                                            | Delete the highlighted line and starts Insert                |
| 1762 | Visual mode                    | U                                                            | So that the highlight region becomes full caps               |
| 1763 | Visual mode                    | V                                                            | Such that the visible area line-oriented, visual mode or exit |
| 1764 | Visual mode                    | X.                                                           | Delete the highlighted area                                  |
| 1765 | Visual mode                    | Y.                                                           | Yank the highlighted row                                     |
| 1766 | Visual mode                    | a "                                                          | Extended highlighted region that contains a double-quoted string |
| 1767 | Visual mode                    | a '                                                          | Extended highlighted region, so that the string contains an apostrophe |
| 1768 | Visual mode                    | a (                                                          | Equivalent to ab                                             |
| 1769 | Visual mode                    | a)                                                           | Equivalent to ab                                             |
| 1770 | Visual mode                    | a <                                                          | Extended highlighted region that contains a <> block         |
| 1771 | Visual mode                    | a>                                                           | Equivalent to a <                                            |
| 1772 | Visual mode                    | aB                                                           | Extended highlighted region that comprises a {} block        |
| 1773 | Visual mode                    | aW                                                           | Extended highlighted region that contains "a WORD"           |
| 1774 | Visual mode                    | a [                                                          | Extended highlighted region that contains a [] block         |
| 1775 | Visual mode                    | a]                                                           | Equivalent to a [                                            |
| 1776 | Visual mode                    | a`                                                           | Extended highlighted region that contains a quoted string trans |
| 1777 | Visual mode                    | ab                                                           | Extended highlighted region that comprises a () block        |
| 1778 | Visual mode                    | ap                                                           | Extended highlighted region that contains a paragraph        |
| 1779 | Visual mode                    | as                                                           | Extended highlighted region, so that a sentence comprising   |
| 1780 | Visual mode                    | at                                                           | Extended highlighted region that contains a label block      |
| 1781 | Visual mode                    | aw                                                           | Expand the highlighted area, so with "a word"                |
| 1782 | Visual mode                    | a {                                                          | Equivalent to aB                                             |
| 1783 | Visual mode                    | a}                                                           | Equivalent to aB                                             |
| 1784 | Visual mode                    | c                                                            | Delete the highlighted area and start insert                 |
| 1785 | Visual mode                    | d                                                            | Delete the highlighted area                                  |
| 1786 | Visual mode                    | gJ                                                           | Highlighted line is connected, without intervening spaces    |
| 1787 | Visual mode                    | gq                                                           | Format the highlighted row                                   |
| 1788 | Visual mode                    | gv                                                           | Current and former exchange highlighted area                 |
| 1789 | Visual mode                    | i "                                                          | Extended highlighted region that contains a double-quoted string (but without the quotes) |
| 1790 | Visual mode                    | i '                                                          | Extended highlighted region that contains a single quoted string (but without the quotes) |
| 1791 | Visual mode                    | i (                                                          | Equivalent to ib                                             |
| 1792 | Visual mode                    | i)                                                           | Equivalent to ib                                             |
| 1793 | Visual mode                    | i <                                                          | Extended highlighted region that comprises intron <> block   |
| 1794 | Visual mode                    | i>                                                           | Equivalent to i <                                            |
| 1795 | Visual mode                    | iB                                                           | Extended highlighted region that contains {} block comprising |
| 1796 | Visual mode                    | iW                                                           | Expand the highlighted area, containing the "contents WORD"  |
| 1797 | Visual mode                    | i [                                                          | Extended highlighted region that contains the contents [] Block |
| 1798 | Visual mode                    | i]                                                           | I is equivalent to [                                         |
| 1799 | Visual mode                    | i`                                                           | Extended highlighted region that comprises an anti quoted string (but free of the anti quotes) |
| 1800 | Visual mode                    | ib                                                           | Extended highlighted region that comprises intron () block   |
| 1801 | Visual mode                    | ip                                                           | Extended highlighted region, so that the contents of paragraph comprising |
| 1802 | Visual mode                    | is                                                           | Expand the highlighted area, the sentence that contains the contents |
| 1803 | Visual mode                    | it                                                           | Extended highlighted region that contains the label block comprises |
| 1804 | Visual mode                    | iw                                                           | Expand the highlighted area, the included "contains the word" |
| 1805 | Visual mode                    | i {                                                          | Equivalent to iB                                             |
| 1806 | Visual mode                    | i}                                                           | Equivalent to iB                                             |
| 1807 | Visual mode                    | o                                                            | Move the cursor to the other side of the region              |
| 1808 | Visual mode                    | r                                                            | Delete the highlighted area and start insert                 |
| 1809 | Visual mode                    | s                                                            | Delete the highlighted area and start insert                 |
| 1810 | Visual mode                    | u                                                            | So the whole becomes highlighted area lowercase              |
| 1811 | Visual mode                    | v                                                            | So that the visual character-oriented mode, or visual mode exit |
| 1812 | Visual mode                    | x                                                            | Delete the highlighted area                                  |
| 1813 | Visual mode                    | y                                                            | Yank the highlighted area                                    |
| 1814 | Visual mode                    | ~                                                            | Change the case highlighted region                           |
| 1816 | Command line editing           | CTRL-A                                                       | Using the previous cursor mode for completion, and insert all matches. |
| 1817 | Command line editing           | CTRL-B                                                       | Move the cursor to the beginning of the local command line   |
| 1818 | Command line editing           | CTRL-C                                                       | It is equivalent to <ESC>                                    |
| 1819 | Command line editing           | CTRL-D                                                       | List mode before the cursor all completions                  |
| 1820 | Command line editing           | CTRL-E                                                       | Move the cursor to where the end of the command line         |
| 1821 | Command line editing           | CTRL-F                                                       | 'Cedit' default value: Open a command line window; otherwise do not |
| 1823 | Command line editing           | <BS>                                                         | Delete the character before the cursor                       |
| 1824 | Command line editing           | {Char1} <BS> {char2}                                         | 'Digraph' is opened, to enter a digraph                      |
| 1825 | Command line editing           | CTRL-H                                                       | It is equivalent to <BS>                                     |
| 1826 | Command line editing           | <Tab>                                                        | If 'wildchar' is <Tab>: full complement preceding cursor mode |
| 1827 | Command line editing           | <S-Tab>                                                      | It is equivalent to the CTRL-P                               |
| 1828 | Command line editing           | 'Wildchar'                                                   | Before the cursor up mode (default: <Tab>)                   |
| 1829 | Command line editing           | CTRL-I                                                       | It is equivalent to the <Tab>                                |
| 1830 | Command line editing           | <NL>                                                         | It is equivalent to the <CR>                                 |
| 1831 | Command line editing           | CTRL-J                                                       | It is equivalent to the <CR>                                 |
| 1832 | Command line editing           | CTRL-K {char1} {char2}                                       | Enter the two-letter alphabet                                |
| 1833 | Command line editing           | CTRL-L                                                       | Complement the cursor before the mode, and insert the longest common substring |
| 1834 | Command line editing           | <CR>                                                         | Execute the entered command                                  |
| 1835 | Command line editing           | CTRL-M                                                       | It is equivalent to the <CR>                                 |
| 1836 | Command line editing           | CTRL-N                                                       | Use 'wildchar' with multiple matches: go to next match, otherwise: equivalent to <Down> |
| 1837 | Command line editing           | CTRL-O                                                       | different                                                    |
| 1838 | Command line editing           | CTRL-P                                                       | Use 'wildchar' with multiple matches: Go to previous match, otherwise: Equivalent to <Up> |
| 1839 | Command line editing           | CTRL-Q                                                       | Equivalent to CTRL-V unless used for terminal control flow   |
| 1840 | Command line editing           | CTRL-R {0-9a-z "% # *: = CTRL-F CTRL-P CTRL-W CTRL-A}        | Insert the contents of a register or a special object to where the cursor is, as you type |
| 1841 | Command line editing           | CTRL-R CTRL-R {0-9a-z "% # *: = CTRL-F CTRL-P CTRL-W CTRL-A} | Insert the contents of the register or special object to where the cursor is located |
| 1842 | Command line editing           | CTRL-S                                                       | (For terminal control flow)                                  |
| 1844 | Command line editing           | CTRL-U                                                       | Delete all characters                                        |
| 1845 | Command line editing           | CTRL-V                                                       | Insert the next non-numeric character as it is, or insert the single byte represented by the next three digits. |
| 1846 | Command line editing           | CTRL-W                                                       | Delete the word in front of the cursor                       |
| 1848 | Command line editing           | CTRL-Y                                                       | Copy (extract) modeless selection                            |
| 1850 | Command line editing           | <Esc>                                                        | Give up the command line, do not execute                     |
| 1851 | Command line editing           | CTRL- [                                                      | Equivalent to <Esc>                                          |
| 1852 | Command line editing           | CTRL- CTRL-N                                                 | Go to normal mode, give up the command line                  |
| 1853 | Command line editing           | CTRL- CTRL-G                                                 | Go to the mode specified by 'insertmode' and discard the command line |
| 1854 | Command line editing           | CTRL- a - d                                                  | Reserved for expansion                                       |
| 1855 | Command line editing           | CTRL-e {expr}                                                | Replace the command line with the result of {expr}           |
| 1856 | Command line editing           | CTRL-f - z                                                   | Reserved for expansion                                       |
| 1857 | Command line editing           | CTRL-                                                        | Others do not                                                |
| 1858 | Command line editing           | CTRL-]                                                       | Activate the acronym                                         |
| 1859 | Command line editing           | CTRL- ^                                                      | Switch \|: lmap \| Use of mappings                           |
| 1860 | Command line editing           | CTRL-_                                                       | When 'allowrevins' opens: Change language (Hebrew, Persia)   |
| 1861 | Command line editing           | <Del>                                                        | Delete the cursor character                                  |
| 1862 | Command line editing           | <Left>                                                       | Cursor left                                                  |
| 1863 | Command line editing           | <S-Left>                                                     | Cursor one word                                              |
| 1864 | Command line editing           | <C-Left>                                                     | Cursor one word                                              |
| 1865 | Command line editing           | <Right>                                                      | Cursor right                                                 |
| 1866 | Command line editing           | <S-Right>                                                    | The cursor one word right                                    |
| 1867 | Command line editing           | <C-Right>                                                    | The cursor one word right                                    |
| 1868 | Command line editing           | <Up>                                                         | Transferred before the match cursor mode from the history before a command line |
| 1869 | Command line editing           | <S-Up>                                                       | Former transferred from a command line history               |
| 1870 | Command line editing           | <Down>                                                       | After transferred before the match cursor mode from a command line history |
| 1871 | Command line editing           | <S-Down>                                                     | After transferred from a command line history                |
| 1872 | Command line editing           | <Home>                                                       | Move the cursor to the beginning of the local command line   |
| 1873 | Command line editing           | <End>                                                        | Move the cursor to where the end of the command line         |
| 1874 | Command line editing           | <PageDown>                                                   | Equivalent to <S-Down>                                       |
| 1875 | Command line editing           | <PageUp>                                                     | Equivalent to <S-Up>                                         |
| 1876 | Command line editing           | <Insert>                                                     | Switching insert / replace mode                              |
| 1877 | Command line editing           | <LeftMouse>                                                  | Move the cursor to where the mouse was clicked               |
| 1878 | EX command                     | :!                                                           | Filter rows, or may be performed by the external command     |
| 1879 | EX command                     | : !!                                                         | Repeat the previous ":!" Command                             |
| 1880 | EX command                     | : #                                                          | Equivalent to ": number"                                     |
| 1881 | EX command                     | : &                                                          | Repeat the previous ": substitute"                           |
| 1882 | EX command                     | : *                                                          | The implementation of the contents of the register           |
| 1883 | EX command                     | : <                                                          | A left row 'shiftwidth'                                      |
| 1884 | EX command                     | : =                                                          | Display the line number of the cursor                        |
| 1885 | EX command                     | :>                                                           | A right row 'shiftwidth'                                     |
| 1886 | EX command                     | : @                                                          | The implementation of the contents of the register           |
| 1887 | EX command                     | : @@                                                         | Repeat the previous ": @"                                    |
| 1888 | EX command                     | : N [ext]                                                    | Go on a file parameter list                                  |
| 1889 | EX command                     | : P [rint]                                                   | Display line                                                 |
| 1890 | EX command                     | : X                                                          | Requests an encryption key                                   |
| 1891 | EX command                     | : A [ppend]                                                  | Additional text                                              |
| 1892 | EX command                     | : Ab [breviate]                                              | Enter the abbreviation                                       |
| 1893 | EX command                     | : Abc [lear]                                                 | Remove all abbreviations                                     |
| 1894 | EX command                     | : Abo [veleft]                                               | Such that the window appears in the left or split over       |
| 1895 | EX command                     | : Al [l]                                                     | Open a window for each file in the argument list             |
| 1896 | EX command                     | : Am [enu]                                                   | Input menu items for all modes                               |
| 1897 | EX command                     | : An [oremenu]                                               | Input menu items for all modes will not be remapped          |
| 1898 | EX command                     | : Ar [gs]                                                    | Display parameter list                                       |
| 1899 | EX command                     | : Arga [dd]                                                  | Add items to the list of parameters                          |
| 1900 | EX command                     | : Argd [elete]                                               | Remove items from the argument list                          |
| 1901 | EX command                     | : Arge [dit]                                                 | Add items to the list of parameters and edit it              |
| 1902 | EX command                     | : Argdo                                                      | All items on the argument list execute a command             |
| 1903 | EX command                     | : Argg [lobal]                                               | Define global parameter list                                 |
| 1904 | EX command                     | : Argl [ocal]                                                | Defining a local parameter list                              |
| 1905 | EX command                     | : Argu [ment]                                                | Go to a list of parameters specified file                    |
| 1906 | EX command                     | : As [cii]                                                   | Show ascii value of the character under the cursor           |
| 1907 | EX command                     | : Au [tocmd]                                                 | Command input or automatically displayed                     |
| 1908 | EX command                     | : Aug [roup]                                                 | Select Auto to use the command group                         |
| 1909 | EX command                     | : Aun [menu]                                                 | Under the menu to delete all modes                           |
| 1910 | EX command                     | : B [uffer]                                                  | Go to the buffer list the specific buffer                    |
| 1911 | EX command                     | : BN [ext]                                                   | Go to the buffer list on a buffer                            |
| 1912 | EX command                     | : Ba [ll]                                                    | Open a window for the buffer of each buffer list             |
| 1913 | EX command                     | : Bad [d]                                                    | Increasing the buffer to the buffer list                     |
| 1914 | EX command                     | : Bd [elete]                                                 | Delete the buffer from the buffer list                       |
| 1915 | EX command                     | : Be [have]                                                  | Set the mouse behavior and choices                           |
| 1916 | EX command                     | : Bel [owright]                                              | Such that the window appears at the right split or below     |
| 1917 | EX command                     | : Bf [irst]                                                  | Go to the first buffer list buffer                           |
| 1918 | EX command                     | : Bl [ast]                                                   | Go to the buffer list of the last buffer                     |
| 1919 | EX command                     | : Bm [odified]                                               | Go to the next buffer list in a modified buffers             |
| 1920 | EX command                     | : Bn [ext]                                                   | Go to the buffer list next buffer                            |
| 1921 | EX command                     | : Bo [tright]                                                | Such that the window appears at the far right of the split or below |
| 1922 | EX command                     | : Bp [revious]                                               | Go to the buffer list on a buffer                            |
| 1923 | EX command                     | : Br [ewind]                                                 | Go to the first buffer list buffer                           |
| 1924 | EX command                     | : Brea [k]                                                   | Out of the while loop                                        |
| 1925 | EX command                     | : Breaka [dd]                                                | Increase debugger breakpoints                                |
| 1926 | EX command                     | : Breakd [el]                                                | Delete debugger breakpoints                                  |
| 1927 | EX command                     | : Breakl [ist]                                               | Listed debugger breakpoints                                  |
| 1928 | EX command                     | : Bro [wse]                                                  | Use the file selection dialog                                |
| 1929 | EX command                     | : Bufdo                                                      | Buffer command to execute all list                           |
| 1930 | EX command                     | : Buffers                                                    | List all files in the buffer list                            |
| 1931 | EX command                     | : Bun [load]                                                 | Uninstall specified buffer                                   |
| 1932 | EX command                     | : Bw [ipeout]                                                | Really delete a buffer                                       |
| 1933 | EX command                     | : C [hange]                                                  | Alternatively row or several rows                            |
| 1934 | EX command                     | : CN [ext]                                                   | Jump to a wrong                                              |
| 1935 | EX command                     | : CNf [ile]                                                  | Jump to last error before a file                             |
| 1936 | EX command                     | : Ca [bbrev]                                                 | Like ": abbreviate", but for Command-line mode               |
| 1937 | EX command                     | : Cabc [lear]                                                | Clear all abbreviations for Command Line Mode                |
| 1938 | EX command                     | : Caddb [uffer]                                              | Buffer supplemented by mistake                               |
| 1939 | EX command                     | : Cad [dexpr]                                                | Supplemented by an expression error                          |
| 1940 | EX command                     | : Caddf [ile]                                                | Quickfix added to the current list of error messages         |
| 1941 | EX command                     | : Cal [l]                                                    | Call functions                                               |
| 1942 | EX command                     | : Cat [ch]                                                   | : Part try the command                                       |
| 1943 | EX command                     | : Cb [uffer]                                                 | The error message and jump to first                          |
| 1944 | EX command                     | : Cc                                                         | Jump to a specific error                                     |
| 1945 | EX command                     | : Ccl [ose]                                                  | Close window quickfix                                        |
| 1946 | EX command                     | : Cd                                                         | Change directory                                             |
| 1947 | EX command                     | : Ce [nter]                                                  | Layout line to center alignment                              |
| 1948 | EX command                     | : Cex [pr]                                                   | Read error from expressions and jump to first                |
| 1949 | EX command                     | : Cf [ile]                                                   | Reads the file containing the error message, and jump to first |
| 1950 | EX command                     | : Cfir [st]                                                  | Jump to the specified error, the default for the first       |
| 1951 | EX command                     | : Cgetb [uffer]                                              | Get an error from the buffer                                 |
| 1952 | EX command                     | : Cgete [xpr]                                                | Get an error from the real expression in                     |
| 1953 | EX command                     | : Cg [etfile]                                                | Reads the file containing the error message                  |
| 1954 | EX command                     | : Cha [nges]                                                 | Displays a list of changes                                   |
| 1955 | EX command                     | : Chd [ir]                                                   | Change the current directory                                 |
| 1956 | EX command                     | : Che [ckpath]                                               | Lists the header files included                              |
| 1957 | EX command                     | : Checkt [ime]                                               | Check the label buffer load time                             |
| 1958 | EX command                     | : Cl [ist]                                                   | Lists all errors                                             |
| 1959 | EX command                     | : Cla [st]                                                   | Jump to the specified error, defaults to the last            |
| 1960 | EX command                     | : Clo [se]                                                   | Change the current window                                    |
| 1961 | EX command                     | : Cm [ap]                                                    | Like ": map", but for Command-line mode                      |
| 1962 | EX command                     | : Cmapc [lear]                                               | Clear all mapping for the command-line mode                  |
| 1963 | EX command                     | : Cme [nu]                                                   | Command line mode to add menu                                |
| 1964 | EX command                     | : Cn [ext]                                                   | Jump to the next error                                       |
| 1965 | EX command                     | : Cnew [er]                                                  | Jump to the next newer error list                            |
| 1966 | EX command                     | : Cnf [ile]                                                  | Jump to the first error the next file                        |
| 1967 | EX command                     | : Cno [remap]                                                | Like ": noremap", but for Command-line mode                  |
| 1968 | EX command                     | : Cnorea [bbrev]                                             | Like ": noreabbrev", but for Command-line mode               |
| 1969 | EX command                     | : Cnoreme [nu]                                               | Like ": noremenu", but for Command-line mode                 |
| 1970 | EX command                     | : Co [py]                                                    | Copy Rows                                                    |
| 1971 | EX command                     | : Col [der]                                                  | Jump to an older list of errors                              |
| 1972 | EX command                     | : Colo [rscheme]                                             | Load a specific color scheme                                 |
| 1973 | EX command                     | : Com [mand]                                                 | Establish user-defined commands                              |
| 1974 | EX command                     | : Comc [lear]                                                | Clear all user-defined commands                              |
| 1975 | EX command                     | : Comp [iler]                                                | Set options for a particular compiler                        |
| 1976 | EX command                     | : Con [tinue]                                                | Back: while at the beginning                                 |
| 1977 | EX command                     | : Conf [irm]                                                 | When the need to recognize, the user is prompted             |
| 1978 | EX command                     | : Cope [n]                                                   | Open the window quickfix                                     |
| 1979 | EX command                     | : Cp [revious]                                               | Jump to a wrong                                              |
| 1980 | EX command                     | : Cpf [ile]                                                  | Jump to last error on a file                                 |
| 1981 | EX command                     | : Cq [uit]                                                   | Exit Vim, with an error code                                 |
| 1982 | EX command                     | : Cr [ewind]                                                 | Jump to a specific error, the default for the first          |
| 1983 | EX command                     | : Cs [cope]                                                  | Cscope command execution                                     |
| 1984 | EX command                     | : Cst [ag]                                                   | Use cscope to jump to the label                              |
| 1985 | EX command                     | : Cu [nmap]                                                  | Similar to the ": unmap", but for Command-line mode          |
| 1986 | EX command                     | : Cuna [bbrev]                                               | Like ": unabbrev", but for Command-line mode                 |
| 1987 | EX command                     | : Cunme [nu]                                                 | Delete menu command line                                     |
| 1988 | EX command                     | : Cw [indow]                                                 | Open or close the window quickfix                            |
| 1989 | EX command                     | : D [elete]                                                  | Delete Row                                                   |
| 1990 | EX command                     | : Delm [arks]                                                | Deletes marks                                                |
| 1991 | EX command                     | : Deb [ug]                                                   | Run in debug mode                                            |
| 1992 | EX command                     | : Debugg [reedy]                                             | Where input from the normal reading mode commands            |
| 1993 | EX command                     | : Delc [ommand]                                              | Delete user-defined commands                                 |
| 1994 | EX command                     | : Delf [unction]                                             | Delete User function                                         |
| 1995 | EX command                     | : Dif [fupdate]                                              | Update 'diff' buffer                                         |
| 1996 | EX command                     | : Diffg [et]                                                 | Delete all the difference in the current buffer              |
| 1997 | EX command                     | : Diffo [ff]                                                 | Close diff mode                                              |
| 1998 | EX command                     | : Diffp [atch]                                               | Apply the patch and then displays the difference             |
| 1999 | EX command                     | : Diffpu [t]                                                 | Another difference delete buffer                             |
| 2000 | EX command                     | : Diffs [plit]                                               | Differential display and other documents                     |
| 2001 | EX command                     | : Diffthis                                                   | Make the current window the diff window                      |
| 2002 | EX command                     | : Dig [raphs]                                                | Displayed or to enter a digraph                              |
| 2003 | EX command                     | : Di [splay]                                                 | Display register                                             |
| 2004 | EX command                     | : Dj [ump]                                                   | Jump to #define                                              |
| 2005 | EX command                     | : Dl [ist]                                                   | List all #define                                             |
| 2006 | EX command                     | : Do [autocmd]                                               | In the current application automatically command buffer      |
| 2007 | EX command                     | : Doautoa [ll]                                               | Application automatically command on all loaded buffers      |
| 2008 | EX command                     | : Dr [op]                                                    | Jump to the editing window of a file, edit it if unsuccessful in the current window |
| 2009 | EX command                     | : Ds [earch]                                                 | Lists a #define                                              |
| 2010 | EX command                     | : Dsp [lit]                                                  | Split window and jump to the #define                         |
| 2011 | EX command                     | : E [dit]                                                    | Edit the file                                                |
| 2012 | EX command                     | : Ea [rlier]                                                 | The change back to the old, revoked                          |
| 2013 | EX command                     | : Ec [ho]                                                    | Echo the expression results                                  |
| 2014 | EX command                     | : Echoe [rr]                                                 | Similar to: echo, as if the same error display and usage history |
| 2015 | EX command                     | : Echoh [l]                                                  | Set highlight commands such as echo                          |
| 2016 | EX command                     | : Echom [sg]                                                 | It is equivalent to: echo, putting a message in history      |
| 2017 | EX command                     | : Echon                                                      | It is equivalent to: echo, but without leaving <EOL>         |
| 2018 | EX command                     | : El [se]                                                    | : If part of the command                                     |
| 2019 | EX command                     | : Elsei [f]                                                  | : If part of the command                                     |
| 2020 | EX command                     | : Em [enu]                                                   | Implementation of the menu by name                           |
| 2021 | EX command                     | : En [dif]                                                   | The end of the most recent: if                               |
| 2022 | EX command                     | : Endfo [r]                                                  | The end of the most recent: for                              |
| 2023 | EX command                     | : Endf [unction]                                             | End user functions                                           |
| 2024 | EX command                     | : Endt [ry]                                                  | The end of the most recent: try                              |
| 2025 | EX command                     | : Endw [hile]                                                | The end of the most recent: while                            |
| 2026 | EX command                     | : Ene [w]                                                    | Edit the new unnamed buffer                                  |
| 2027 | EX command                     | : Ex                                                         | Equivalent to ": edit"                                       |
| 2028 | EX command                     | : Exe [cute]                                                 | Result of performing string expressions generated            |
| 2029 | EX command                     | : Exi [t]                                                    | Equivalent to ": xit"                                        |
| 2030 | EX command                     | : Exu [sage]                                                 | Ex command Overview                                          |
| 2031 | EX command                     | : F [ile]                                                    | Display or set the current file name                         |
| 2032 | EX command                     | : Files                                                      | List all files in the buffer list                            |
| 2033 | EX command                     | : Filet [ype]                                                | File type detection switch opening / closing                 |
| 2034 | EX command                     | : Fin [d]                                                    | Find files in 'path' and Editors'                            |
| 2035 | EX command                     | : Fina [lly]                                                 | : Part try the command                                       |
| 2036 | EX command                     | : Fini [sh]                                                  | Exit Vim script execution                                    |
| 2037 | EX command                     | : Fir [st]                                                   | Go to the first file in the argument list                    |
| 2038 | EX command                     | : Fix [del]                                                  | Settings <Del> key code                                      |
| 2039 | EX command                     | : Fo [ld]                                                    | Creating fold                                                |
| 2040 | EX command                     | : Foldc [lose]                                               | Close folding                                                |
| 2041 | EX command                     | : Foldd [oopen]                                              | Close all not collapsed row Run                              |
| 2042 | EX command                     | : Folddoc [losed]                                            | For all rows in the closed collapsed Run                     |
| 2043 | EX command                     | : Foldo [pen]                                                | Open the fold                                                |
| 2044 | EX command                     | : For                                                        | for loop                                                     |
| 2045 | EX command                     | : Fu [nction]                                                | User-defined functions                                       |
| 2046 | EX command                     | : G [lobal]                                                  | Matching command line execution                              |
| 2047 | EX command                     | : Go [to]                                                    | Go to a byte buffer                                          |
| 2048 | EX command                     | : Gr [ep]                                                    | Performing 'grepprg' and go to the first match at            |
| 2049 | EX command                     | : Grepa [dd]                                                 | Similar: grep, but later attached to the current list        |
| 2050 | EX command                     | : Gu [i]                                                     | Start GUI                                                    |
| 2051 | EX command                     | : Gv [im]                                                    | Start GUI                                                    |
| 2052 | EX command                     | : Ha [rdcopy]                                                | Send text to the printer                                     |
| 2053 | EX command                     | : H [elp]                                                    | Open the help window                                         |
| 2054 | EX command                     | : Helpf [ind]                                                | Open dialog box displays the help window                     |
| 2055 | EX command                     | : Helpg [rep]                                                | Similar to the ": grep", but the search help files           |
| 2056 | EX command                     | : Helpt [ags]                                                | Help generate tags for a catalog                             |
| 2057 | EX command                     | : Hi [ghlight]                                               | Specify the method of highlighting                           |
| 2058 | EX command                     | : Hid [e]                                                    | Hide the current buffer as a command                         |
| 2059 | EX command                     | : His [tory]                                                 | Display the history list                                     |
| 2060 | EX command                     | : I [nsert]                                                  | Insert text                                                  |
| 2061 | EX command                     | : Ia [bbrev]                                                 | Like ": abbrev", but for insertion mode                      |
| 2062 | EX command                     | : Iabc [lear]                                                | Like ": abclear", but for insertion mode                     |
| 2063 | EX command                     | : If                                                         | Execute commands when conditions are met                     |
| 2064 | EX command                     | : Ij [ump]                                                   | Jump to the identifier is defined                            |
| 2065 | EX command                     | : Il [ist]                                                   | List matching identifier row                                 |
| 2066 | EX command                     | : Im [ap]                                                    | Like ": map", but for insertion mode                         |
| 2067 | EX command                     | : Imapc [lear]                                               | Like ": map", but for insertion mode                         |
| 2068 | EX command                     | : Ime [nu]                                                   | To insert mode to add menu                                   |
| 2069 | EX command                     | : Ino [remap]                                                | Like ": noremap", but for insertion mode                     |
| 2070 | EX command                     | : Inorea [bbrev]                                             | Like ": noreabbrev", but for insertion mode                  |
| 2071 | EX command                     | : Inoreme [nu]                                               | Like ": noremenu", but for insertion mode                    |
| 2072 | EX command                     | : Int [ro]                                                   | Introductory text display                                    |
| 2073 | EX command                     | : Is [earch]                                                 | Line matching identifier list                                |
| 2074 | EX command                     | : Isp [lit]                                                  | Split window and jump to the identifier is defined           |
| 2075 | EX command                     | : Iu [nmap]                                                  | Like ": unmap", but for insertion mode                       |
| 2076 | EX command                     | : Iuna [bbrev]                                               | Like ": unabbrev", but for insertion mode                    |
| 2077 | EX command                     | : Iunme [nu]                                                 | Delete Insert mode menu                                      |
| 2078 | EX command                     | : J [oin]                                                    | Line connection                                              |
| 2079 | EX command                     | : Ju [mps]                                                   | Show jump table                                              |
| 2080 | EX command                     | : K                                                          | Set marker location                                          |
| 2081 | EX command                     | : Keepa [lt]                                                 | Follow orders remain unchanged alternate file                |
| 2082 | EX command                     | : Kee [pmarks]                                               | Follow commands remain the same position marking             |
| 2083 | EX command                     | : Keepj [jumps]                                              | Follow orders and keep the jump table position unchanged mark |
| 2084 | EX command                     | : LN [ext]                                                   | Position to position on a list of                            |
| 2085 | EX command                     | : LNf [ile]                                                  | Go to a location on a recent file                            |
| 2086 | EX command                     | : L [ist]                                                    | Display line                                                 |
| 2087 | EX command                     | : Lad [dexpr]                                                | By the expression supplementary position                     |
| 2088 | EX command                     | : Laddb [uffer]                                              | Buffer supplemented by position                              |
| 2089 | EX command                     | : Laddf [ile]                                                | The position to the current position of the list             |
| 2090 | EX command                     | : La [st]                                                    | Go to the last file in the argument list                     |
| 2091 | EX command                     | : Lan [guage]                                                | Setting the language (locale)                                |
| 2092 | EX command                     | : Lat [er]                                                   | Go to the new changes, redo                                  |
| 2093 | EX command                     | : Lb [uffer]                                                 | Analysis of position and jump to the first position          |
| 2094 | EX command                     | : Lc [d]                                                     | Change the local directory                                   |
| 2095 | EX command                     | : Lch [dir]                                                  | Change the local directory                                   |
| 2096 | EX command                     | : Lcl [ose]                                                  | Close position window                                        |
| 2097 | EX command                     | : Lcs [cope]                                                 | Similar to the ": cscope", but use the location list         |
| 2098 | EX command                     | : Le [ft]                                                    | Left row                                                     |
| 2099 | EX command                     | : Lefta [bove]                                               | Such that the window appears in the left or split over       |
| 2100 | EX command                     | : Let                                                        | Assignment to a variable or option                           |
| 2101 | EX command                     | : Lex [pr]                                                   | From the expressions read position and jump to first         |
| 2102 | EX command                     | : Lf [ile]                                                   | From the document reading position and jump to first         |
| 2103 | EX command                     | : Lfir [st]                                                  | Go to the location specified, the default first              |
| 2104 | EX command                     | : Lgetb [uffer]                                              | Read from the buffer location                                |
| 2105 | EX command                     | : Lgete [xpr]                                                | Reading position from expressions                            |
| 2106 | EX command                     | : Lg [etfile]                                                | Read from a file location                                    |
| 2107 | EX command                     | : Lgr [ep]                                                   | Run 'grepprg' and go to the first match                      |
| 2108 | EX command                     | : Lgrepa [dd]                                                | Like: grep, but attached to the current list                 |
| 2109 | EX command                     | : Lh [elpgrep]                                               | Similar to ": helpgrep", but uses the location list          |
| 2110 | EX command                     | : ll                                                         | Go to the specified location                                 |
| 2111 | EX command                     | : lla [st]                                                   | Go to the specified location, the default last one           |
| 2112 | EX command                     | : lli [st]                                                   | List all the locations                                       |
| 2113 | EX command                     | : lmak [e]                                                   | Execute the external command 'makeprg' and analyze the error message |
| 2114 | EX command                     | : lm [ap]                                                    | Similar to ": map!", But includes Lang-Arg mode              |
| 2115 | EX command                     | : lmapc [lear]                                               | Similar to ": mapclear!", But includes Lang-Arg mode         |
| 2116 | EX command                     | : lne [xt]                                                   | Jump to the next location                                    |
| 2117 | EX command                     | : lnew [er]                                                  | Jump to the newer list of places                             |
| 2118 | EX command                     | : lnf [ile]                                                  | Jump to the next location of the first file                  |
| 2119 | EX command                     | : ln [oremap]                                                | Similar to ": noremap!", But includes Lang-Arg mode          |
| 2120 | EX command                     | : loadk [eymap]                                              | Load the following keyboard map until EOF                    |
| 2121 | EX command                     | : lo [adview]                                                | Load the view from the file for the current window           |
| 2122 | EX command                     | : loc [kmarks]                                               | Follow commands remain the same position marking             |
| 2123 | EX command                     | : lockv [ar]                                                 | Lock variables                                               |
| 2124 | EX command                     | : lol [der]                                                  | Go to the older location list                                |
| 2125 | EX command                     | : lope [n]                                                   | Open the location window                                     |
| 2126 | EX command                     | : lp [revious]                                               | Go to the previous position                                  |
| 2127 | EX command                     | : lpf [ile]                                                  | Go to the nearest location of the previous file              |
| 2128 | EX command                     | : lr [ewind]                                                 | Go to the specified location, the default first one          |
| 2129 | EX command                     | : ls                                                         | List all the buffers                                         |
| 2130 | EX command                     | : lt [ag]                                                    | Jump to the label, and add the matching label to the list of positions |
| 2131 | EX command                     | : lu [nmap]                                                  | Similar to ": unmap!", But includes Lang-Arg mode            |
| 2132 | EX command                     | : lua                                                        | Execute \| Lua \| command                                    |
| 2133 | EX command                     | : luad [o]                                                   | Run Lua commands on each line                                |
| 2134 | EX command                     | : luaf [ile]                                                 | Execute \| Lua \| script file                                |
| 2135 | EX command                     | : lv [imgrep]                                                | Search patterns in several documents                         |
| 2136 | EX command                     | : lvimgrepa [dd]                                             | Similar to: vimgrep, but attached to the current list        |
| 2137 | EX command                     | : lw [indow]                                                 | Opens or closes the location window                          |
| 2138 | EX command                     | : m [ove]                                                    | Moving line                                                  |
| 2139 | EX command                     | : ma [rk]                                                    | Set marker location                                          |
| 2140 | EX command                     | : mak [e]                                                    | Executes the external command 'makeprg' and analyzes its error message |
| 2141 | EX command                     | : map                                                        | Display or input mapping                                     |
| 2142 | EX command                     | : Mapc [lear]                                                | Clear all common visualization and mapping mode              |
| 2143 | EX command                     | : Marks                                                      | List all the marks                                           |
| 2144 | EX command                     | : Mat [ch]                                                   | Displays matching define highlighting mode                   |
| 2145 | EX command                     | : Me [nu]                                                    | Enter a new menu item                                        |
| 2146 | EX command                     | : Menut [ranslate]                                           | Add a menu translation project                               |
| 2147 | EX command                     | : Mes [sages]                                                | The message previously displayed                             |
| 2148 | EX command                     | : Mk [exrc]                                                  | Write current mappings and settings to a file                |
| 2149 | EX command                     | : Mks [ession]                                               | Session information is written to the file                   |
| 2150 | EX command                     | : Mksp [ell]                                                 | Generate .spl spelling files                                 |
| 2151 | EX command                     | : Mkv [imrc]                                                 | Write current mappings and settings to a file                |
| 2152 | EX command                     | : Mkvie [w]                                                  | Write the current window to view file                        |
| 2153 | EX command                     | : Mod [e]                                                    | Display or change the screen mode                            |
| 2154 | EX command                     | : Mz [scheme]                                                | MzScheme command execution                                   |
| 2155 | EX command                     | : Mzf [ile]                                                  | MzScheme execute the script file                             |
| 2156 | EX command                     | : Nbc [lose]                                                 | Close the current session Netbeans                           |
| 2157 | EX command                     | : Nb [key]                                                   | Passing a key to Netbeans                                    |
| 2158 | EX command                     | : Nbs [art]                                                  | Open a new session Netbeans                                  |
| 2159 | EX command                     | : N [ext]                                                    | Jump to the next file in the argument list                   |
| 2160 | EX command                     | : New                                                        | Create a new blank window                                    |
| 2161 | EX command                     | : Nm [ap]                                                    | Like ": map", but using normal mode                          |
| 2162 | EX command                     | : Nmapc [lear]                                               | Clear all the maps of the normal mode                        |
| 2163 | EX command                     | : Nme [nu]                                                   | Increase the normal mode menu                                |
| 2164 | EX command                     | : Nn [oremap]                                                | Like ": noremap", but using normal mode                      |
| 2165 | EX command                     | : Nnoreme [nu]                                               | Like ": noremenu", but using normal mode                     |
| 2166 | EX command                     | : Noa [utocmd]                                               | The command does not follow automatically activate command   |
| 2167 | EX command                     | : No [remap]                                                 | Input mapping will not be remapped                           |
| 2168 | EX command                     | : Noh [lsearch]                                              | Pause 'hlsearch' highlighted                                 |
| 2169 | EX command                     | : Norea [bbrev]                                              | Enter the abbreviation will not be remapped                  |
| 2170 | EX command                     | : Noreme [nu]                                                | Enter the menu will not be remapped                          |
| 2171 | EX command                     | : Norm [al]                                                  | Normal mode command                                          |
| 2172 | EX command                     | : Nu [mber]                                                  | No trip to the text row                                      |
| 2173 | EX command                     | : Nun [map]                                                  | Similar to the ": unmap", but using normal mode              |
| 2174 | EX command                     | : Nunme [nu]                                                 | Delete the Normal mode menu                                  |
| 2175 | EX command                     | : ol [dfiles]                                                | Lists the files containing the location markers in the viminfo file |
| 2176 | EX command                     | : o [pen]                                                    | Startup open mode (not implemented)                          |
| 2177 | EX command                     | : om [ap]                                                    | Similar to ": map" but uses operator wait mode               |
| 2178 | EX command                     | : omapc [lear]                                               | Removes all mappings of operator wait patterns               |
| 2179 | EX command                     | : ome [nu]                                                   | Add menu for operator wait mode                              |
| 2180 | EX command                     | : on [ly]                                                    | Close the current window, except for the current window      |
| 2181 | EX command                     | : ono [remap]                                                | Similar to ": noremap" but uses operator wait mode           |
| 2182 | EX command                     | : onoreme [nu]                                               | Similar to ": noremenu" but uses operator wait mode          |
| 2183 | EX command                     | : opt [ions]                                                 | Opens the Options window                                     |
| 2184 | EX command                     | : ou [nmap]                                                  | Similar to ": unmap" but uses operator wait mode             |
| 2185 | EX command                     | : ounme [nu]                                                 | Delete operator waiting mode menu                            |
| 2186 | EX command                     | : ow [nsyntax]                                               | Set a new local syntax highlight for this window             |
| 2187 | EX command                     | : p [rint]                                                   | Display line                                                 |
| 2188 | EX command                     | : profd [el]                                                 | Stop the profile function or script                          |
| 2189 | EX command                     | : prof [ile]                                                 | Profile function or script                                   |
| 2190 | EX command                     | : pro [mptfind]                                              | Open the GUI dialog to search                                |
| 2191 | EX command                     | : promptr [epl]                                              | Open the GUI dialog to search / replace                      |
| 2192 | EX command                     | : pc [lose]                                                  | Close the preview window                                     |
| 2193 | EX command                     | : ped [it]                                                   | Edit the file in the preview window                          |
| 2194 | EX command                     | : pe [rl]                                                    | Execute the Perl command                                     |
| 2195 | EX command                     | : perld [o]                                                  | Perl commands are executed on each line                      |
| 2196 | EX command                     | : po [p]                                                     | Jump to the label stack older projects                       |
| 2197 | EX command                     | : pop [up]                                                   | Pop up menu by name                                          |
| 2198 | EX command                     | : pp [op]                                                    | In the preview window ": pop"                                |
| 2199 | EX command                     | : pre [serve]                                                | Write all the text to the swap file                          |
| 2200 | EX command                     | : prev [ious]                                                | Jump to the previous file in the parameter list              |
| 2201 | EX command                     | : ps [earch]                                                 | Similar to ": ijump", but displays a match in the preview window |
| 2202 | EX command                     | : pt [ag]                                                    | Display the label in the preview window                      |
| 2203 | EX command                     | : ptN [ext]                                                  | In the preview window \|: tNext \|                           |
| 2204 | EX command                     | : ptf [irst]                                                 | In the preview window \|: trewind \|                         |
| 2205 | EX command                     | : ptj [ump]                                                  | In the preview window \|: tjump \| and display label         |
| 2206 | EX command                     | : Ptl [ast]                                                  | In the preview window \|: tlast \|                           |
| 2207 | EX command                     | : Ptn [ext]                                                  | In the preview window \|: tnext \|                           |
| 2208 | EX command                     | : Ptp [revious]                                              | In the preview window \|: tprevious \|                       |
| 2209 | EX command                     | : Ptr [ewind]                                                | In the preview window \|: trewind \|                         |
| 2210 | EX command                     | : Pts [elect]                                                | In the preview window \|: tselect \| and display label       |
| 2211 | EX command                     | : Pu [t]                                                     | Inserted into the text contents of register                  |
| 2212 | EX command                     | : Pw [d]                                                     | Displays the current directory                               |
| 2213 | EX command                     | : Py3                                                        | Python 3 command execution                                   |
| 2214 | EX command                     | : Python3                                                    | With: py3                                                    |
| 2215 | EX command                     | : Py3f [ile]                                                 | Python 3 script file execution                               |
| 2216 | EX command                     | : Py [thon]                                                  | Execute Python commands                                      |
| 2217 | EX command                     | : Pyf [ile]                                                  | Execute Python script file                                   |
| 2218 | EX command                     | : Q [uit]                                                    | Exit the current window (if there is only a window, exit Vim) |
| 2219 | EX command                     | : Quita [ll]                                                 | Exit Vim                                                     |
| 2220 | EX command                     | : Qa [ll]                                                    | Exit Vim                                                     |
| 2221 | EX command                     | : R [ead]                                                    | Reading a file into text                                     |
| 2222 | EX command                     | : Rec [over]                                                 | Recover files from the swap file                             |
| 2223 | EX command                     | : Red [o]                                                    | Redo an undo changes                                         |
| 2224 | EX command                     | : Redi [r]                                                   | Redirect message to a file or register                       |
| 2225 | EX command                     | : Redr [aw]                                                  | Forced display redrawing                                     |
| 2226 | EX command                     | : Redraws [tatus]                                            | Forcing the state to redraw lines                            |
| 2227 | EX command                     | : Reg [isters]                                               | Displays the contents of the register                        |
| 2228 | EX command                     | : Res [ize]                                                  | Change the height of the current window                      |
| 2229 | EX command                     | : Ret [ab]                                                   | Change the size of the tab                                   |
| 2230 | EX command                     | : Retu [rn]                                                  | Returned from user functions                                 |
| 2231 | EX command                     | : Rew [ind]                                                  | Go to the first file in the argument list                    |
| 2232 | EX command                     | : Ri [ght]                                                   | Right align text                                             |
| 2233 | EX command                     | : Rightb [elow]                                              | Split window that appears on the right or below              |
| 2234 | EX command                     | : Rub [y]                                                    | Ruby command execution                                       |
| 2235 | EX command                     | : Rubyd [o]                                                  | For each command line execution Ruby                         |
| 2236 | EX command                     | : Rubyf [ile]                                                | Execute Ruby script file                                     |
| 2237 | EX command                     | : Rund [o]                                                   | From the document reads revocation information               |
| 2238 | EX command                     | : Ru [ntime]                                                 | Perform 'runtimepath' in the script vim                      |
| 2239 | EX command                     | : Rv [iminfo]                                                | Viminfo file for reading                                     |
| 2240 | EX command                     | : S [ubstitute]                                              | Find and replace text                                        |
| 2241 | EX command                     | : SN [ext]                                                   | Split window and go to the parameter list of previous file   |
| 2242 | EX command                     | : San [dbox]                                                 | Execute commands in the sandbox                              |
| 2243 | EX command                     | : Sa [rgument]                                               | Split window and go to the parameter list to a document      |
| 2244 | EX command                     | : Sal [l]                                                    | Open the window for each file argument list                  |
| 2245 | EX command                     | : Sav [eas]                                                  | Save the file with another name.                             |
| 2246 | EX command                     | : Sb [uffer]                                                 | Split window and go to the buffer list to a document         |
| 2247 | EX command                     | : SbN [ext]                                                  | Split window and go to the previous file buffer list         |
| 2248 | EX command                     | : Sba [ll]                                                   | Open the window for each file in the buffer list             |
| 2249 | EX command                     | : Sbf [irst]                                                 | Split window and go to the first file in the buffer list     |
| 2250 | EX command                     | : Sbl [ast]                                                  | The last file Split window and go to the buffer list         |
| 2251 | EX command                     | : Sbm [odified]                                              | Split window and go to the buffer list of modified files     |
| 2252 | EX command                     | : Sbn [ext]                                                  | After a file split window and go to the buffer list          |
| 2253 | EX command                     | : Sbp [revious]                                              | Split window and go to the previous file buffer list         |
| 2254 | EX command                     | : Sbr [ewind]                                                | Split window and go to the first file in the buffer list     |
| 2255 | EX command                     | : Scrip [tnames]                                             | Lists the names of all Vim scripts have been executed        |
| 2256 | EX command                     | : Scripte [ncoding]                                          | Encoding performed Vim script used                           |
| 2257 | EX command                     | : Scs [cope]                                                 | Split window and execute the command cscope                  |
| 2258 | EX command                     | : Se [t]                                                     | Display or set options                                       |
| 2259 | EX command                     | : Setf [iletype]                                             | Set 'filetype', unless already set                           |
| 2260 | EX command                     | : Setg [lobal]                                               | Display or set the global option value                       |
| 2261 | EX command                     | : Setl [ocal]                                                | Display or set the local option value                        |
| 2262 | EX command                     | : Sf [ind]                                                   | Split the current window and edit the 'path' file            |
| 2263 | EX command                     | : Sfir [st]                                                  | Split window and go to the first file in the argument list   |
| 2264 | EX command                     | : Sh [ell]                                                   | Shell retreated                                              |
| 2265 | EX command                     | : Sim [alt]                                                  | Win32 GUI: Analog Windows ALT key                            |
| 2266 | EX command                     | : Sig [n]                                                    | Operation label                                              |
| 2267 | EX command                     | : Sil [ent]                                                  | Quiet operation command                                      |
| 2268 | EX command                     | : Sl [eep]                                                   | A few seconds without doing anything                         |
| 2269 | EX command                     | : Sla [st]                                                   | The last file Split window and go to the list of parameters  |
| 2270 | EX command                     | : Sm [agic]                                                  | Band of 'magic': substitute                                  |
| 2271 | EX command                     | : Sma [p]                                                    | Like ": map", but for selecting the mode                     |
| 2272 | EX command                     | : Smapc [lear]                                               | Delete all the selected mode map                             |
| 2273 | EX command                     | : Sme [nu]                                                   | Increase the menu selection mode                             |
| 2274 | EX command                     | : Sn [ext]                                                   | Split the window and go to the next file in the parameter list |
| 2275 | EX command                     | : sni [ff]                                                   | Send the request to sniff                                    |
| 2276 | EX command                     | : sno [magic]                                                | With 'nomagic': substitute                                   |
| 2277 | EX command                     | : snor [emap]                                                | Similar to ": noremap", but for selecting a pattern          |
| 2278 | EX command                     | : snoreme [nu]                                               | Similar to ": noremenu", but for selecting patterns          |
| 2279 | EX command                     | : sor [t]                                                    | Sort the rows                                                |
| 2280 | EX command                     | : so [urce]                                                  | Read the Vim or Ex command from the file                     |
| 2281 | EX command                     | : spelld [ump]                                               | Split the window and fill it with the correct word           |
| 2282 | EX command                     | : spe [llgood]                                               | Increase the spelling of good words                          |
| 2283 | EX command                     | : spelli [nfo]                                               | Display the information of the spelling file loaded          |
| 2284 | EX command                     | : spellr [epall]                                             | Like last \| z = \|, but replace all bad words               |
| 2285 | EX command                     | : spellu [ndo]                                               | Remove good or bad words                                     |
| 2286 | EX command                     | : spellw [rong]                                              | Increase spelling mistakes                                   |
| 2287 | EX command                     | : sp [lit]                                                   | Split the current window                                     |
| 2288 | EX command                     | : spr [evious]                                               | Split window and go to the parameter list of previous file   |
| 2289 | EX command                     | : sre [wind]                                                 | Split window and go to the first file in the argument list   |
| 2290 | EX command                     | : st [op]                                                    | Pause the editor and return the shell                        |
| 2291 | EX command                     | : sta [g]                                                    | Split the window and jump to the label                       |
| 2292 | EX command                     | : startg [replace]                                           | Start the virtual replacement mode                           |
| 2293 | EX command                     | : startr [eplace]                                            | Start replacing mode                                         |
| 2294 | EX command                     | : star [tinsert]                                             | Start inserting mode                                         |
| 2295 | EX command                     | : stopi [nsert]                                              | Exit from insert mode                                        |
| 2296 | EX command                     | : stj [ump]                                                  | Execute ": tjump" and split the window                       |
| 2297 | EX command                     | : sts [elect]                                                | Execute ": tselect" and split the window                     |
| 2298 | EX command                     | : sun [hide]                                                 | Equivalent to ": unhide"                                     |
| 2299 | EX command                     | : sunm [ap]                                                  | Similar to ": unmap", but for selecting a pattern            |
| 2300 | EX command                     | : sunme [nu]                                                 | Delete the menu of the selection mode                        |
| 2301 | EX command                     | : sus [pend]                                                 | Equivalent to ": stop"                                       |
| 2302 | EX command                     | : sv [iew]                                                   | Split the window and edit the file in read-only mode         |
| 2303 | EX command                     | : sw [apname]                                                | Display the name of the current exchange file                |
| 2304 | EX command                     | : sy [ntax]                                                  | Grammatical highlight                                        |
| 2305 | EX command                     | : sync [bind]                                                | Synchronized scrolling binding                               |
| 2306 | EX command                     | : T                                                          | Equivalent to ": copy"                                       |
| 2307 | EX command                     | : TN [ext]                                                   | Jump to a matching tag                                       |
| 2308 | EX command                     | : TabN [ext]                                                 | Skip to previous tab                                         |
| 2309 | EX command                     | : Tabc [lose]                                                | Close current tab                                            |
| 2310 | EX command                     | : Tabdo                                                      | Execute commands for each tab                                |
| 2311 | EX command                     | : Tabe [dit]                                                 | Edit the file in a new tab                                   |
| 2312 | EX command                     | : Tabf [ind]                                                 | Looking for 'path' in the file, edit it in a new tab         |
| 2313 | EX command                     | : Tabfir [st]                                                | Go to the first tab                                          |
| 2314 | EX command                     | : Tabl [ast]                                                 | Go to the last tab                                           |
| 2315 | EX command                     | : Tabm [ove]                                                 | The tab should be relocated                                  |
| 2316 | EX command                     | : Tabnew                                                     | Edit the file in a new tab                                   |
| 2317 | EX command                     | : Tabn [ext]                                                 | Go to the next tab                                           |
| 2318 | EX command                     | : Tabo [nly]                                                 | Close all all tabs except the current tab                    |
| 2319 | EX command                     | : Tabp [revious]                                             | Go to the previous tab page                                  |
| 2320 | EX command                     | : Tabr [ewind]                                               | Go to the first tab                                          |
| 2321 | EX command                     | : Tabs                                                       | Lists the tabs and content contained inside                  |
| 2322 | EX command                     | : Tab                                                        | Create a new tab when you open a new window                  |
| 2323 | EX command                     | : Ta [g]                                                     | Jump to the tag                                              |
| 2324 | EX command                     | : Tags                                                       | Displays the contents of the tag stack                       |
| 2325 | EX command                     | : Tc [l]                                                     | Tcl command execution                                        |
| 2326 | EX command                     | : Tcld [o]                                                   | Tcl command execution for each row                           |
| 2327 | EX command                     | : Tclf [ile]                                                 | Execute Tcl script file                                      |
| 2328 | EX command                     | : Te [aroff]                                                 | Tear off a menu                                              |
| 2329 | EX command                     | : Tf [irst]                                                  | Go to the first matching label                               |
| 2330 | EX command                     | : Th [row]                                                   | Throw an exception                                           |
| 2331 | EX command                     | : Tj [ump]                                                   | Like ": tselect", there is only one jump directly to the match |
| 2332 | EX command                     | : Tl [ast]                                                   | Jump to the last match of the label                          |
| 2333 | EX command                     | : Tm [enu]                                                   | Tools menu definitions tips                                  |
| 2334 | EX command                     | : Tn [ext]                                                   | Jump to the next matching tag                                |
| 2335 | EX command                     | : To [pleft]                                                 | Such that the window appears at the top or dividing the leftmost |
| 2336 | EX command                     | : Tp [revious]                                               | Jump to a matching tag                                       |
| 2337 | EX command                     | : Tr [ewind]                                                 | Jump to the first matching tag                               |
| 2338 | EX command                     | : Try                                                        | Execute commands, error or exception termination             |
| 2339 | EX command                     | : Ts [elect]                                                 | List matching tags and select one                            |
| 2340 | EX command                     | : Tu [nmenu]                                                 | Delete menu tooltip                                          |
| 2341 | EX command                     | : U [ndo]                                                    | Undo recent changes                                          |
| 2342 | EX command                     | : Undoj [oin]                                                | And the next change on a block merging revocation            |
| 2343 | EX command                     | : Undol [ist]                                                | Revocation lists leaf nodes of the tree                      |
| 2344 | EX command                     | : Una [bbreviate]                                            | Delete Abbreviations                                         |
| 2345 | EX command                     | : Unh [ide]                                                  | Open the window for the buffer list for each file loaded     |
| 2346 | EX command                     | : Unl [et]                                                   | Delete variables                                             |
| 2347 | EX command                     | : Unlo [ckvar]                                               | Variables to unlock                                          |
| 2348 | EX command                     | : Unm [ap]                                                   | Delete the mapping                                           |
| 2349 | EX command                     | : Unme [nu]                                                  | Delete menu                                                  |
| 2350 | EX command                     | : Uns [ilent]                                                | Non-quiet mode command execution                             |
| 2351 | EX command                     | : Up [date]                                                  | If there are changes, the write-back buffer                  |
| 2352 | EX command                     | : V [global]                                                 | On the line does not match, run                              |
| 2353 | EX command                     | : Ve [rsion]                                                 | Display the version number and other information             |
| 2354 | EX command                     | : Verb [ose]                                                 | Run, during set 'verbose'                                    |
| 2355 | EX command                     | : Vert [ical]                                                | Vertical dividing such command following the                 |
| 2356 | EX command                     | : Vim [grep]                                                 | Finding patterns in several files                            |
| 2357 | EX command                     | : Vimgrepa [dd]                                              | Similar to: vimgrep, but attached to the current list        |
| 2358 | EX command                     | : Vi [sual]                                                  | Equivalent to ": edit", but turn off the "Ex" mode           |
| 2359 | EX command                     | : Viu [sage]                                                 | Overview Normal mode command                                 |
| 2360 | EX command                     | : Vie [w]                                                    | Edit the file in read-only mode                              |
| 2361 | EX command                     | : Vm [ap]                                                    | Like ": map", but using visual selection mode +              |
| 2362 | EX command                     | : Vmapc [lear]                                               | + Select mode removes the visual mapping of all              |
| 2363 | EX command                     | : Vme [nu]                                                   | A visible increase in the menu select mode +                 |
| 2364 | EX command                     | : Vne [w]                                                    | Create a new blank window, split vertically                  |
| 2365 | EX command                     | : Vn [oremap]                                                | Like ": noremap", but using visual selection mode +          |
| 2366 | EX command                     | : Vnoreme [nu]                                               | Like ": noremenu", but using visual selection mode +         |
| 2367 | EX command                     | : Vs [plit]                                                  | Vertical split current window                                |
| 2368 | EX command                     | : Vu [nmap]                                                  | Like ": unmap", but using visual selection mode +            |
| 2369 | EX command                     | : Vunme [nu]                                                 | Visualization + delete menu selection mode                   |
| 2370 | EX command                     | : Windo                                                      | Execute commands for each window                             |
| 2371 | EX command                     | : W [rite]                                                   | Write the file                                               |
| 2372 | EX command                     | : WN [ext]                                                   | Writing a file, and then jump to the parameter list of previous file |
| 2373 | EX command                     | : Wa [ll]                                                    | All write-back (change) buffer                               |
| 2374 | EX command                     | : Wh [ile]                                                   | As long as the condition is detected, loop                   |
| 2375 | EX command                     | : Wi [nsize]                                                 | Obtain or set the window size (obsolete)                     |
| 2376 | EX command                     | : Winc [md]                                                  | Execution window (CTRL-W) command                            |
| 2377 | EX command                     | : Winp [os]                                                  | Get or set the window position                               |
| 2378 | EX command                     | : Wn [ext]                                                   | Writing a file, and then jump to the next file in the argument list |
| 2379 | EX command                     | : Wp [revious]                                               | Writing a file, and then jump to the parameter list of previous file |
| 2380 | EX command                     | : Wq                                                         | Writing a file, and then exit the window or Vim              |
| 2381 | EX command                     | : Wqa [ll]                                                   | All write-back (change) buffer and then exit Vim             |
| 2382 | EX command                     | : Ws [verb]                                                  | The verb to a workshop by IPC                                |
| 2383 | EX command                     | : Wu [ndo]                                                   | The revocation information is written to the file            |
| 2384 | EX command                     | : Wv [iminfo]                                                | Write viminfo file                                           |
| 2385 | EX command                     | : X [it]                                                     | If the buffer was changed, write it. Then exit window or Vim |
| 2386 | EX command                     | : Xa [ll]                                                    | Equivalent to ": wqall"                                      |
| 2387 | EX command                     | : Xmapc [lear]                                               | Visual mode to delete all mappings                           |
| 2388 | EX command                     | : Xm [ap]                                                    | Like ": map", but use visual mode                            |
| 2389 | EX command                     | : Xme [nu]                                                   | Increase the visual mode menu                                |
| 2390 | EX command                     | : Xn [oremap]                                                | Like ": noremap", but use visual mode                        |
| 2391 | EX command                     | : Xnoreme [nu]                                               | Like ": noremenu", but use visual mode                       |
| 2392 | EX command                     | : Xu [nmap]                                                  | Similar to the ": unmap", but use visual mode                |
| 2393 | EX command                     | : Xunme [nu]                                                 | Delete menu visual mode                                      |
| 2394 | EX command                     | : Y [ank]                                                    | Extracting lines to register                                 |
| 2395 | EX command                     | :z                                                           | Show some lines                                              |