# EMUZ80-68030RAM
68030 with SRAM Single-Board Computer

MC68030のDynamic Bus Sizing機能によって「外部8bitバス」で動作します。

![MEZ68030RAM](https://github.com/satoshiokue/EMUZ80-68030RAM/blob/main/MEZ68030RAM.jpeg)  
68030+SRAM  

電脳伝説さん(@vintagechips)のEMUZ80が出力するZ80 CPU信号をメザニンボードで組み替え、MC68030とSRAMを動作させることができます。  
MC68EC030RP40Bで動作確認しています。  

ソースコードはGazelleさんのEMUZ80用main_cpz.cを元に改変してGPLライセンスに基づいて公開するものです。

https://drive.google.com/drive/folders/1NaIIpzsUY3lptekcrJjwyvWTBNHIjUf1

## メザニンボード
https://github.com/satoshiokue/MEZ68030RAM

## アドレスマップ
```
RAM   0x00000 - 0x1FFFF 128Kbytes

UART  0x40000000   Data REGISTER
      0x40000001   Control REGISTER
```

## ROMデータ
main.cにrom[]イメージを３つ格納しています。  

EhBASIC  
RAMサイズ、ACIAアドレスを調整しています。  
https://github.com/satoshiokue/EhBASIC68k-EMU  

Universal Monitor  
https://github.com/satoshiokue/unimon_EMUZ80-68008  

fig-FORTH  
https://github.com/jefftranter/68000/tree/master/figforth  

