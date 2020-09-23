<div align="center">

## Create a clock with JScript


</div>

### Description

The following script will create a clock using JavaScript, which will be shown in the status bar.
 
### More Info
 
The user must know JavaScript Basics.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Elio](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/elio.md)
**Level**          |Beginner
**User Rating**    |4.3 (17 globes from 4 users)
**Compatibility**  |
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/elio-create-a-clock-with-jscript__2-1877/archive/master.zip)

### API Declarations

Created by Elio


### Source Code

```
function Time()
{
// first we get date infos.
var d= new Date();
//then we get other detailes.
var m= d.getMinutes();
var h= d.getHours();
var s= d.getSeconds();
var day=d.getDate();
var mon=d.getMonth();
var year=d.getYear();
if (s<10) { s="0"+s; }
if (m<10) { m="0"+m; }
var time= h+":"+m+":"+s;
var res="Today is: "+day+"/"+mon+"/"+year+" | "+"Local Time: "+time;
window.status=res;
// reload the function every one second.
setTimeout('Time()',1000);
}
```

