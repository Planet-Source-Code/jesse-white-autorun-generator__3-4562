<div align="center">

## Autorun Generator


</div>

### Description

Generates a autorun.inf
 
### More Info
 
filename


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jesse White](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jesse-white.md)
**Level**          |Beginner
**User Rating**    |4.3 (17 globes from 4 users)
**Compatibility**  |C\+\+ \(general\), Borland C\+\+
**Category**       |[Files](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/files__3-2.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jesse-white-autorun-generator__3-4562/archive/master.zip)

### API Declarations

fstream.h


### Source Code

```
#include <fstream.h>
int main()
{
char filename[80];
cout <<" Welcome To Autorun Maker 1.0 \n \n";
cout <<" Please enter the file name you would like to make autorun\n";
cout <<" ::";
cin.get(filename,79);
ofstream file;      //creates an ofstream object
file.open("autorun.inf"); //creates the autorun.inf file and opens it for writing
file<<"[autorun]\n";       //writes to the file
file<<"open="<<filename<<"\n";
file.close();
   return 0;
}
```

