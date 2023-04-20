# EMUZ80-68030RAM
68030 with SRAM Single-Board Computer

MC68030のDynamic Bus Sizing機能によって「外部8bitバス」で動作します。

![MEZ68030FPU](https://github.com/satoshiokue/EMUZ80-68030FPU/blob/main/IMG_2003.jpeg)  
68030+SRAM  

電脳伝説さん(@vintagechips)のEMUZ80が出力するZ80 CPU信号をメザニンボードで組み替え、MC68030とMC68881を動作させることができます。  
MC68030RC33CとPIC18F47Q43の組み合わせで動作確認しています。  

動作確認で使用したMPU&FPU  
MC68030RC33C  
MC68882RC25A  
MC68881RC16R  

ソースコードはGazelleさんのEMUZ80用main_cpz.cを元に改変してGPLライセンスに基づいて公開するものです。

https://drive.google.com/drive/folders/1NaIIpzsUY3lptekcrJjwyvWTBNHIjUf1

## メザニンボード
https://github.com/satoshiokue/MEZ68030FPU

## アドレスマップ
```
ROM   0x0000 - 0x3FFF 16Kbytes
RAM   0x8000 - 0x8FFF 4Kbytes (0x9FFF 8Kbytes:PIC18F47Q84,PIC18F47Q83)

FPU   0x22000 - 0x2201F

UART  0xE000   Data REGISTER
      0xE001   Control REGISTER
```
