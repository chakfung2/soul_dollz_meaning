Just my notes on what the data inside a soul doll is (I don't mean to make it complete complete, someone can do it :P)<br/>
**Currently doing all testing on a Talisdam**<br/>


## There are 8 sprites for each legendz.
### Each sprite takes up 96 bytes. (So every 6 rows in a hex editor. (16 × 6 = 96))<br/>
1st sprite: 0 to 5F<br/>
2nd sprite: 60 to BF<br/>
3rd sprite: C0 to 11F<br/>
4th sprite: 120 to 17F<br/>
5th sprite: 180 to 1DF<br/>
6th sprite: 1E0 to 23F<br/>
7th sprite: 240 to 29F<br/>
8th sprite: 2A0 to 2FF<br/>

### Each sprite is 24 pixels wide and 32 pixels high. (different values seem to represents different tiles)<br/>
0 - 0F<br/>
is responsible for the top 24*5 pixel row of a frame<br/>
10 - 1F<br/>
is the next row (6 pixel in height)<br/>
...There are 8 sprites, so until 2FF...<br/>
<br/>
There are 32 pixel is each sprite. Each sprite is seperated into 6 rows.<br/>
1st row, 5 pixels in height<br/>
2nd row, 6 pixels in height<br/>
3rd row, 5 pixels in height<br/>
4th row, 5 pixels in height<br/>
5th row, 5 pixels in height<br/>
6th row, 6 pixels in height<br/>
<br/>

## 302 (Thanks to Shonumi)
This address is how the Talisdam recognises what the soul doll is.<br/><br/>
 **HOWEVER**, the name of the legendz is stored in the chip.(as of writing this, I haven't found where it is, but if you empty the chip, the name does not show.)<br/><br/>
 **ALSO**, it only change the close up sprite. (I tried changing nothing but this address from 3B(Bicorn) to 4B(Jabberwock), the close up sprite changes but everything else stay the exact same.(which seems to suggest the close up sprite is stored in the toy.))<br/><br/>
For example,<br/>
14 is a Manticore (Shares the same value with a Silver Manticore.) <br/>
16 is a Command Blazedragon<br/>
34 is a Command Blazedragon Bulk Armed (B)<br/>
3B is a Bicorn<br/>
4B is a Jabberwock<br/>


## Base stats addresses
317 318 HP (for example, 9990 is stored as 999 in hex, so 03E7) (the highest the toy can show is 9990, anything above 9990 is shown as 4 asterisks) <br/>
319 Magic  (for example, 990 is stored as 99 in hex, so 63)(the highest the toy can show is 990)<br/>
31A Counter (ditto)(ditto)<br/>
31B Attack (ditto)(ditto)<br/>
31C Recovery (ditto)(ditto)<br/>

## Nickname
34D 34E 34F 350 (4 characters)<br/>
For example,<br/>
CF is ?<br/>
50 is ア ('a' in Katakana)<br/>
55 is カ ('ka' in Katakana)<br/>

## Added stats
The 'format' of the values is the same as base stats.<br/>
The max value you can get playing the toy is written in ().<br/>
356 357 HP (5110(decimal), but because this is stored as 511(decimal), the corresponding value is 01 FF.)<br/>
358 Magic (630(decimal), so 3F)<br/>
359 Counter (630(decimal), so 3F)<br/>
35A Attack (630(decimal), so 3F)<br/>
35B Recovery (630(decimal), so 3F)<br/>

## Current Age??
36F<br/>

## The Crystal that the legendz is holding.
370<br/>
4B is Nekuromu no Monsho<br/>

## Skill slots
35F to 36D<br/><br/>
For example, <br/>
01 Small attack <br/>
02 Default Magic Attack<br/>
09 Counter Burisuブリス<br/>
0E Default Attack　<br/>
15 Default Cure<br/>
1F Henka Necrom<br/>
3D Spritual Legion<br/>
3E Necrom Legion<br/>
(In battle, if you use a Legion of a different attribute to your legendz, it will still show the correct Legion for your legendz. For example, Bicorn attribute is Necrom, using Spritual Legion in battle shows Necrom Legion )<br/>




