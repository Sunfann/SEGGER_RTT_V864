RTT
===

SEGGER RTT Sources

https://www.segger.com/products/debug-probes/j-link/technology/about-real-time-transfer  
https://wiki.segger.com/RTT

## Included files

  * `RTT/`
    * `SEGGER_RTT.c`               - Main module for RTT.
    * `SEGGER_RTT.h`               - Main header for RTT.
    * `SEGGER_RTT_ASM_ARMv7M.S`    - Assembly-optimized implementation of RTT functions for ARMv7M processors.
    * `SEGGER_RTT_Printf.c`        - Simple implementation of printf (`SEGGER_RTT_Printf()`) to write formatted strings via RTT.
  * `Syscalls/`
    * `SEGGER_RTT_Syscalls_*.c`    - Low-level syscalls to retarget `printf()` to RTT with different toolchains.
  * `Config/`
    * `SEGGER_RTT_Conf.h`          - RTT configuration file.
  * `Examples/`
    * `Main_RTT_InputEchoApp.c`    - Example application which echoes input on Channel 0.
    * `Main_RTT_MenuApp.c`         - Example application to demonstrate RTT bi-directional functionality.
    * `Main_RTT_PrintfTest.c`      - Example application to test RTT's simple printf implementation.
    * `Main_RTT_SpeedTestApp.c`    - Example application to measure RTT performance. (Requires embOS)
	
	
	
## 已修改SEGGER_RTT_Printf.c，适用于浮点数输出

# 附录
	* 基于RTT调试接口的项目适配性的lib库化实现与工程应用
	https://blog.csdn.net/qq_38364548/article/details/154918801
	
	* 嵌入式调试利器：SEGGER RTT 常用函数详解、实战技巧（J-Scope工具）与项目用例
	https://blog.csdn.net/qq_38364548/article/details/154848476
