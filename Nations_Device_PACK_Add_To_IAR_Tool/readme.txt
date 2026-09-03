/* Nations Device PACK Add To IAR Tool
   使用说明和版本更新记录
 */
 
/* 1.使用说明 */
/*   i.  以管理员权限运行“Nations Device PACK Add To IAR Tool Vx.x.x.exe”
     ii. IAR安转目录选择，例如C:\Program Files (x86)\IAR Systems\Embedded Workbench 7.5
     iii.点击“安装”
*/

/* 2.用J-Link工具仿真时找不到芯片型号解决办法 */
/*  i.  找到J-Link安装目录，如C:\Program Files (x86)\SEGGER\JLink\
    ii  将J-Link安装目录中的JLinkARM.dll与JLinkConfig.exe这两个文件复制到IAR安装目录中的
        以下路径替换原有文件
            C:\Program Files (x86)\IAR Systems\Embedded Workbench 7.5\arm\bin\
        替换前建议先备份原有文件
    iii 将JLinkDevices.ref复制到IAR安装目录中的以下路径
            C:\Program Files (x86)\IAR Systems\Embedded Workbench 7.5\arm\bin\
        并修改JLinkDevices.ref文件内容为J-Link安装目录，如C:\Program Files (x86)\SEGGER\JLink\
*/

/* 3.版本更新记录 */
/*   
     V1.0.0 初始版本

     V1.1.0 安装时添加删除原有PACK包的弹窗选择

     V1.1.1 更新已知BUG

     V1.1.2 更新已知BUG
     
     V1.1.3 追加N32G435G8Q7型号
     
     V1.1.4 优化FLASH下载算法

     V1.1.5 追加N32G452CEL7型号、增加N32G435GBQ7
     
     V1.1.6 增加N32G452CCT7型号、修改设备寄存器描述错误

     V1.1.7 增加N32G455CEQ7型号

     V1.1.8 更新N32G4FR\G45x\WB452 svd文件
	 
     V1.1.9 增加N32G430系列相关型号，安装软件更新为英文版

     V1.1.10 优化N32G031系列的下载算法
     
     V1.1.11 新增N32A455系列 

     V1.1.12 新增N32G401、N32G401F8S7_1系列 
     
     V1.1.13 优化N32G4FR\G45x\WB452\G43x\L43x\L40x系列mac文件及下载算法； 新增N32A032系列 ；新增N32A430系列；
     
     V1.1.14 新增N32G451系列 ；新增N32G401系列；新增N32L402系列；新增N32G003系列；
	 
     V1.2.0 新增N32G05x、N32H47x、N32H48x系列；优化N32G43X\L40X\L43X系列；新增N32G032F8型号

     V1.3.0 新增N32H76x系列

    V1.4.0 修改N32G43X\L40X\L43X系列SVD文件,新增N32H78x系列，优化76x的系列，新增N32G033系列；

    V1.5.0 增加N32H480、N32H488型号，优化N32H473、N32H474、N32H482、N32H487型号，删除Nations下的N32G033系列，新增Nsing下的N32G033系列
              优化N32G455型号

    V1.6.0 新增N32H49x系列，新增N32H73x系列

    V1.7.0 新增N32A052系列，新增N32A003系列，优化N32G003系列，优化N32G45x系列，优化N32G4FR系列，优化N32WB452系列，优化N32A455系列

    V1.8.0 新增N32G41x、N32MC47x、N32DP47x系列，优化N32H7xx、N32H49x、N32G430、N32G401系列，新增N32H7xxxKx7系列的设备
*/
-------------------------------------------------------------------------------------
/* Nations Device PACK Add To IAR Tool
  Instructions for use and version update record
 */
 
/* 1. Instructions for use */
/*   i. Run "Nations Device PACK Add To IAR Tool Vx.x.x.exe" with administrator rights
      ii. IAR installation directory selection, such as C:\Program Files (x86)\IAR Systems\Embedded Workbench 7.5
      iii. Click "Install"
*/

/* 2. The solution to the chip model that cannot be found when simulating with the J-Link tool */
/* i. Find the J-Link installation directory, such as C:\Program Files (x86)\SEGGER\JLink\
   ii. Copy the JLinkARM.dll and JLinkConfig.exe files in the J-Link installation directory to the 
      following paths in the IAR installation directory and replace the original files:
	C:\Program Files (x86)\IAR Systems\Embedded Workbench 7.5\arm\bin\
      It is recommended to back up the original files before replacing
   iii. Copy the JLinkDevices.ref to the following path in the IAR installation directory:
	C:\Program Files (x86)\IAR Systems\Embedded Workbench 7.5\arm\bin\
       And modify the JLinkDevices.ref file content to the J-Link installation directory, such as C:\Program Files (x86)\SEGGER\JLink\
*/

/* 3.Version update record */
/*   
     V1.0.0 Initial version

     V1.1.0 Add the pop-up window option to delete the original PACK package when installing 

     V1.1.1 Update known BUG

     V1.1.2 Update known BUG
     
     V1.1.3 Added N32G435G8Q7 model
     
     V1.1.4 Optimized FLASH download algorithm

     V1.1.5 Adds N32G452CEL7、N32G435GBQ7
     
     V1.1.6 Adds N32G452CCT7, Modify device register description error

     V1.1.7 Adds N32G455CEQ7

     V1.1.8 Update N32G4FR\G45x\WB452 svd, Update the installation software to the English version
     
     V1.1.9 Added N32G430 series models, Updated them to English versions based on software

     V1.1.10 Optimized N32G031 series download algorithm

     V1.1.11 Adds N32A455 series
    
     V1.1.12 Adds N32G401、N32G401F8S7_1 series

     V1.1.13 Optimized N32G4FR\G45x\WB452\G43x\L43x\L40x series mac and download algorithm; adds N32A032 series; adds N32A430 series; 
	 
     V1.1.14 adds N32G451 series; adds N32G401 series; adds N32L402 series; adds N32G003 series
     
     V1.2.0 adds N32G05x\N32H47x\N32H48x series; Optimize N32G43X\L40X\L43X series; adds N32G032F8

     V1.3.0 adds N32H76x series; 

    V1.4.0 Modified N32G43X\L40X\L43X series SVD files,adds N32H78x series, Optimized N32H76x series，add N32G033 series;

    V1.5.0 adds N32H480 and N32H488 models, optimizes N32H473, N32H474, N32H482, and N32H487 models, removes N32G033 series under Nations, and adds N32G033 series under Nsing
              Optimizes N32G455 models.

    V1.6.0 adds N32H49x series; 

    V1.7.0 adds N32A052 series; adds N32A003 series; optimizes N32G003 series; optimizes N32G45x series; optimizes N32G4FR series; optimizes N32WB452 series; optimizes N32A455 series

    V1.8.0 adds N32G41x, N32MC47x, N32DP47x series;optimizes N32H7xx, N32H49x, N32G430, N32G401 series;
*/