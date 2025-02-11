SkyrimSE v1.6.1170
trainwreck v1.4.0

Unhandled exception "EXCEPTION_ACCESS_VIOLATION" at 0x7FF6D6E39843 SkyrimSE.exe+0CE9843

SYSTEM SPECS:
    OS: Microsoft Windows 11 Pro 24H2 26100.2894
    CPU: AuthenticAMD AMD Ryzen 5 5600 6-Core Processor              
    GPU #1: NVIDIA GeForce RTX 4060
    GPU #2: NVIDIA GeForce RTX 4060
    GPU #3: Microsoft Basic Render Driver
    RAM: 14.48 GiB/15.91 GiB
    PAGE FILE: 23.37 GiB/26.91 GiB

PROBABLE CALL STACK:
    [0 ] 0x7FF6D6E39843       SkyrimSE.exe+0CE9843
        call qword ptr [rdi+10h]
    [1 ] 0x7FF6D648D8D9       SkyrimSE.exe+033D8D9
        test eax,eax
    [2 ] 0x7FFC229881CB ConsoleUtilSSE.dll+00281CB
        mov rbx,[rsp+38h]
    [3 ] 0x7FFC2297624F ConsoleUtilSSE.dll+001624F
        mov rax,[rdi]
    [4 ] 0x7FFC2297B01C ConsoleUtilSSE.dll+001B01C
        add rsp,48h
    [5 ] 0x7FFC22976D27 ConsoleUtilSSE.dll+0016D27
        nop
    [6 ] 0x7FF6D758DE05       SkyrimSE.exe+143DE05
        test al,al
    [7 ] 0x7FF6D759EAF9       SkyrimSE.exe+144EAF9
        mov r14d,eax
    [8 ] 0x7FF6D759F7B3       SkyrimSE.exe+144F7B3
        call 0FFFFFFFFFF87AA8Dh
    [9 ] 0x7FF6D7594314       SkyrimSE.exe+1444314
        lea r8,[rbp+67h]
    [10] 0x7FF6D6B109E7       SkyrimSE.exe+09C09E7
        test r15b,r15b
    [11] 0x7FF6D6822CF3       SkyrimSE.exe+06D2CF3
        xor ebx,ebx
    [12] 0x7FF6D6E47888       SkyrimSE.exe+0CF7888
        mov ecx,[rbx+0Ch]
    [13] 0x7FF6D6E47E51       SkyrimSE.exe+0CF7E51
        mov r15d,eax
    [14] 0x7FF6D6E461DA       SkyrimSE.exe+0CF61DA
        movzx eax,byte ptr [rbx+0A74h]
    [15] 0x7FF6D6E20DBD       SkyrimSE.exe+0CD0DBD
        mov rcx,[24FB55Bh]
    [16] 0x7FFCCCA0E8D7       KERNEL32.DLL+002E8D7 BaseThreadInitThunk
        mov ecx,eax
    [17] 0x7FFCCDF3FBCC          ntdll.dll+00DFBCC RtlUserThreadStart
        jmp short 000000000000002Ah

REGISTERS:
    RAX 0x70DF0F9670       (void*)
    RBX 0x0                (size_t)
    RCX 0x1EE71A02600      (Script*)
    RDX 0x70DF0F95B0       (void*)
    RSI 0x0                (size_t)
    RDI 0x1EE71A02600      (Script*)
    RBP 0x70DF0F9670       (void*)
    RSP 0x70DF0F9550       (void*)
    R8  0x1                (size_t)
    R9  0x70DF0F95A8       (char*) "\x01"
    R10 0x7FFCB3D20000     (void* -> VCRUNTIME140.dll+0000000)
        pop r10
    R11 0x7FFCB3D31C27     (void* -> VCRUNTIME140.dll+0011C27 memset)
        vmovdqu [rcx+r9-100h],ymm0
    R12 0x0                (size_t)
    R13 0x1EE71A02600      (Script*)
    R14 0x104              (size_t)
    R15 0x70DF0F99B8       (void*)

STACK:
    [RSP+0   ] 0xD9D65ADCAED16A4A (size_t)
    [RSP+8   ] 0x7FFC244639BA     (void* -> EngineFixes.dll+00239BA)
        add rsp,0A0h
    [RSP+10  ] 0xDEBB9EC5A9BCAE53 (size_t)
    [RSP+18  ] 0x30B5FFE947B2CF7F (size_t)
    [RSP+20  ] 0xCABAC28A00000001 (size_t)
    [RSP+28  ] 0x24B4A3A653B39330 (size_t)
    [RSP+30  ] 0x1EE9EC0FDD8      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+38  ] 0x1                (size_t)
    [RSP+40  ] 0x1EE71A02600      (Script*)
    [RSP+48  ] 0x7FF6D648D8D9     (void* -> SkyrimSE.exe+033D8D9)
        test eax,eax
    [RSP+50  ] 0x0                (size_t)
    [RSP+58  ] 0x7FFC00000001     (size_t)
    [RSP+60  ] 0x9ED35D9856C4     (size_t)
    [RSP+68  ] 0x70DF0F96A0       (void*)
    [RSP+70  ] 0x1EE046133D0      (char*) "\x07"
    [RSP+78  ] 0x7FFC2446C5B6     (void* -> EngineFixes.dll+002C5B6)
        mov r10d,eax
    [RSP+80  ] 0x7FFC2453F630     (void* -> EngineFixes.dll+00FF630)
        dec dword ptr [rdi]
    [RSP+88  ] 0x7FF6D6E190CF     (void* -> SkyrimSE.exe+0CC90CF)
        cmp [rdi],eax
    [RSP+90  ] 0x1EC86AA0E40      (void*)
    [RSP+98  ] 0x14               (size_t)
    [RSP+A0  ] 0x70DF0F96D8       (void*)
    [RSP+A8  ] 0x1EE9EC0FDD8      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+B0  ] 0x7FFC2453F908     (char*) "\x01"
    [RSP+B8  ] 0xCC7B97B37757E6E1 (size_t)
    [RSP+C0  ] 0x1EE71A02614      (void*)
    [RSP+C8  ] 0x7FFC244999C0     (void* -> EngineFixes.dll+00599C0)
        nop
    [RSP+D0  ] 0x7FFC00000000     (size_t)
    [RSP+D8  ] 0x7FF6D6150000     (void* -> SkyrimSE.exe+0000000)
        pop r10
    [RSP+E0  ] 0x169D             (size_t)
    [RSP+E8  ] 0x1                (size_t)
    [RSP+F0  ] 0x7FFC2453FB28     (void* -> EngineFixes.dll+00FFB28)
        add [rax],al
    [RSP+F8  ] 0x7FF6D6750900     (void* -> SkyrimSE.exe+0600900)
        test rbx,rbx
    [RSP+100 ] 0x7FFC2453FB28     (void* -> EngineFixes.dll+00FFB28)
        add [rax],al
    [RSP+108 ] 0x1EDEBDCF6C0      (void*)
    [RSP+110 ] 0x0                (size_t)
    [RSP+118 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+120 ] 0x0                (size_t)
    [RSP+128 ] 0x0                (size_t)
    [RSP+130 ] 0x0                (size_t)
    [RSP+138 ] 0x0                (size_t)
    [RSP+140 ] 0x0                (size_t)
    [RSP+148 ] 0x0                (size_t)
    [RSP+150 ] 0x0                (size_t)
    [RSP+158 ] 0x0                (size_t)
    [RSP+160 ] 0x0                (size_t)
    [RSP+168 ] 0x0                (size_t)
    [RSP+170 ] 0x0                (size_t)
    [RSP+178 ] 0x0                (size_t)
    [RSP+180 ] 0x0                (size_t)
    [RSP+188 ] 0x0                (size_t)
    [RSP+190 ] 0x0                (size_t)
    [RSP+198 ] 0x0                (size_t)
    [RSP+1A0 ] 0x0                (size_t)
    [RSP+1A8 ] 0x0                (size_t)
    [RSP+1B0 ] 0x0                (size_t)
    [RSP+1B8 ] 0x0                (size_t)
    [RSP+1C0 ] 0x0                (size_t)
    [RSP+1C8 ] 0x0                (size_t)
    [RSP+1D0 ] 0x0                (size_t)
    [RSP+1D8 ] 0x0                (size_t)
    [RSP+1E0 ] 0x0                (size_t)
    [RSP+1E8 ] 0x0                (size_t)
    [RSP+1F0 ] 0x0                (size_t)
    [RSP+1F8 ] 0x0                (size_t)
    [RSP+200 ] 0x0                (size_t)
    [RSP+208 ] 0x0                (size_t)
    [RSP+210 ] 0x0                (size_t)
    [RSP+218 ] 0x0                (size_t)
    [RSP+220 ] 0x0                (size_t)
    [RSP+228 ] 0x7FFC9C67372E     (void* -> tbbmalloc.dll+001372E scalable_malloc)
        mov rdi,rax
    [RSP+230 ] 0x70DF0F99B8       (void*)
    [RSP+238 ] 0x1EE9EC0FDD8      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+240 ] 0x1EDB02D3420      (RE::NativeFunction<void (RE::StaticFunctionTag *,std::basic_string<char,std::char_traits<char>,std::allocator<char> >),void>*)
    [RSP+248 ] 0xD1788            (size_t)
    [RSP+250 ] 0x1                (size_t)
    [RSP+258 ] 0x1EE71A02600      (Script*)
    [RSP+260 ] 0x70DF0F9929       (void*)
    [RSP+268 ] 0x7FFC229881CB     (void* -> ConsoleUtilSSE.dll+00281CB)
        mov rbx,[rsp+38h]
    [RSP+270 ] 0x0                (size_t)
    [RSP+278 ] 0x70DF0F9800       (char*) "\x1f"
    [RSP+280 ] 0x1                (size_t)
    [RSP+288 ] 0x0                (size_t)
    [RSP+290 ] 0x1EE71A02600      (Script*)
    [RSP+298 ] 0x7FFC2297624F     (void* -> ConsoleUtilSSE.dll+001624F)
        mov rax,[rdi]
    [RSP+2A0 ] 0x5582             (size_t)
    [RSP+2A8 ] 0x70DF0F9870       (void*)
    [RSP+2B0 ] 0x1F               (size_t)
    [RSP+2B8 ] 0x1F               (size_t)
    [RSP+2C0 ] 0x1EDC810CE50      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+2C8 ] 0x1B               (size_t)
    [RSP+2D0 ] 0x70DF0F9870       (void*)
    [RSP+2D8 ] 0x0                (size_t)
    [RSP+2E0 ] 0x770B59B7305F     (size_t)
    [RSP+2E8 ] 0x7FFC229B5A48     (void* -> ConsoleUtilSSE.dll+0055A48)
        test rax,rax
    [RSP+2F0 ] 0x1B               (size_t)
    [RSP+2F8 ] 0x7FFC2297B01C     (void* -> ConsoleUtilSSE.dll+001B01C)
        add rsp,48h
    [RSP+300 ] 0x1EDC810CE50      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+308 ] 0x7FF6D758287A     (void* -> SkyrimSE.exe+143287A)
        cmp dword ptr [rbx+18h],0
    [RSP+310 ] 0x20               (size_t)
    [RSP+318 ] 0x7FFC2299F41F     (void* -> ConsoleUtilSSE.dll+003F41F)
        test rax,rax
    [RSP+320 ] 0x1EDC810CE50      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+328 ] 0x0                (size_t)
    [RSP+330 ] 0x1B               (size_t)
    [RSP+338 ] 0x1F               (size_t)
    [RSP+340 ] 0x1EE9C436344      (void*)
    [RSP+348 ] 0x7FFC22976D27     (void* -> ConsoleUtilSSE.dll+0016D27)
        nop
    [RSP+350 ] 0x40               (size_t)
    [RSP+358 ] 0x1EE9C436344      (void*)
    [RSP+360 ] 0x70DF0F9929       (void*)
    [RSP+368 ] 0x7000000005       (size_t)
    [RSP+370 ] 0x1EDC810CE00      (void*)
    [RSP+378 ] 0x0                (size_t)
    [RSP+380 ] 0x0                (size_t)
    [RSP+388 ] 0xF                (size_t)
    [RSP+390 ] 0x1EDC810CE00      (void*)
    [RSP+398 ] 0x0                (size_t)
    [RSP+3A0 ] 0x0                (size_t)
    [RSP+3A8 ] 0xF                (size_t)
    [RSP+3B0 ] 0x70DF0F98E0       (void*)
    [RSP+3B8 ] 0x1EE9EC0FDD8      (char*) "cast 4C00A4FD 00000014 left"
    [RSP+3C0 ] 0x1B               (size_t)
    [RSP+3C8 ] 0x0                (size_t)
    [RSP+3D0 ] 0x1EDC810CE00      (void*)
    [RSP+3D8 ] 0x0                (size_t)
    [RSP+3E0 ] 0x0                (size_t)
    [RSP+3E8 ] 0xF                (size_t)
    [RSP+3F0 ] 0x770B59B73F0F     (size_t)
    [RSP+3F8 ] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+400 ] 0x1EE9C436344      (void*)
    [RSP+408 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+410 ] 0x4                (size_t)
    [RSP+418 ] 0x1EDB02D3420      (RE::NativeFunction<void (RE::StaticFunctionTag *,std::basic_string<char,std::char_traits<char>,std::allocator<char> >),void>*)
    [RSP+420 ] 0x70DF0F9A80       (void*)
    [RSP+428 ] 0x7FF6D758DE05     (void* -> SkyrimSE.exe+143DE05)
        test al,al
    [RSP+430 ] 0x14               (size_t)
    [RSP+438 ] 0x14               (size_t)
    [RSP+440 ] 0x70DF0FA2A0       (void*)
    [RSP+448 ] 0x14               (size_t)
    [RSP+450 ] 0x70DF0F99B8       (void*)
    [RSP+458 ] 0x1EE9C436344      (void*)
    [RSP+460 ] 0x1EC86AA0E40      (void*)
    [RSP+468 ] 0x0                (size_t)
    [RSP+470 ] 0x0                (size_t)
    [RSP+478 ] 0x0                (size_t)
    [RSP+480 ] 0x0                (size_t)
    [RSP+488 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+490 ] 0x1EC86AA0E00      (void*)
    [RSP+498 ] 0x70DF0FA080       (void*)
    [RSP+4A0 ] 0x2                (size_t)
    [RSP+4A8 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+4B0 ] 0x70DF0F9B10       (char*) "\x04"
    [RSP+4B8 ] 0x7FFC13B64545     (void* -> PapyrusTweaks.dll+0004545 LoggerHooks::ValidationSignaturesHook::thunk)
        [C:\Modding\SKSEDevelopment\PapyrusTweaks\src\LoggerHooks.h:44]
        add rsp,518h
    [RSP+4C0 ] 0x70DF0F9FC0       (void*)
    [RSP+4C8 ] 0x70DF0FA008       (void*)
    [RSP+4D0 ] 0x1ED00000014      (void*)
    [RSP+4D8 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+4E0 ] 0x70DF0F9AF8       (void*)
    [RSP+4E8 ] 0x7FF6D64CCF3F     (void* -> SkyrimSE.exe+037CF3F)
        nop
    [RSP+4F0 ] 0x1ED00000400      (void*)
    [RSP+4F8 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+500 ] 0x1EE71D611AC      (void*)
    [RSP+508 ] 0x7FF6D7575C3C     (void* -> SkyrimSE.exe+1425C3C)
        test eax,eax
    [RSP+510 ] 0x70DF0FA008       (void*)
    [RSP+518 ] 0x70DF0F9FC0       (void*)
    [RSP+520 ] 0x14               (size_t)
    [RSP+528 ] 0x1                (size_t)
    [RSP+530 ] 0x70DF0F9B00       (void*)
    [RSP+538 ] 0x1                (size_t)
    [RSP+540 ] 0x1EE71F456C0      (char*) "\x02"
    [RSP+548 ] 0x70DF0F9AF0       (void*)
    [RSP+550 ] 0x1EE71F45601      (void*)
    [RSP+558 ] 0x7FF6D759F16F     (void* -> SkyrimSE.exe+144F16F)
        nop
    [RSP+560 ] 0x1EDB00115C0      (char*) "\x02"
    [RSP+568 ] 0x70DF0F9AF0       (void*)
    [RSP+570 ] 0x1EDB00115C0      (char*) "\x02"
    [RSP+578 ] 0x1EDB00115C0      (char*) "\x02"
    [RSP+580 ] 0xFED693013608     (size_t)
    [RSP+588 ] 0x0                (size_t)
    [RSP+590 ] 0x1EDB00115C0      (char*) "\x02"
    [RSP+598 ] 0x1EDB0011700      (char*) "\x15"
    [RSP+5A0 ] 0x0                (size_t)
    [RSP+5A8 ] 0x1EDB00115C0      (char*) "\x02"
    [RSP+5B0 ] 0x0                (size_t)
    [RSP+5B8 ] 0xFFFFFFFFFFFFFFFF (size_t)
    [RSP+5C0 ] 0x4                (size_t)
    [RSP+5C8 ] 0x70DF0F9CE0       (void*)
    [RSP+5D0 ] 0x200              (size_t)
    [RSP+5D8 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+5E0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5E8 ] 0x3F00000CBEBE37E9 (size_t)
    [RSP+5F0 ] 0x70DF0F9BA0       (void*)
    [RSP+5F8 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+600 ] 0x200              (size_t)
    [RSP+608 ] 0x66               (size_t)
    [RSP+610 ] 0x6                (size_t)
    [RSP+618 ] 0x7FFCCB269B71     (void* -> ucrtbase.dll+0009B71)
        mov rax,[rdi]
    [RSP+620 ] 0x1                (size_t)
    [RSP+628 ] 0x70DF0F9CE0       (void*)
    [RSP+630 ] 0x8000             (size_t)
    [RSP+638 ] 0x7FFCCB260000     (void* -> ucrtbase.dll+0000000)
        pop r10
    [RSP+640 ] 0x7FFCCB260000     (void* -> ucrtbase.dll+0000000)
        pop r10
    [RSP+648 ] 0x7FFCCB268F8C     (void* -> ucrtbase.dll+0008F8C)
        add rsp,70h
    [RSP+650 ] 0x1EE9C43636C      (void*)
    [RSP+658 ] 0x7FF6D64CCF3F     (void* -> SkyrimSE.exe+037CF3F)
        nop
    [RSP+660 ] 0x1EE046133D0      (char*) "\x07"
    [RSP+668 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+670 ] 0x70DF0F9C20       (void*)
    [RSP+678 ] 0x2                (size_t)
    [RSP+680 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+688 ] 0x20               (size_t)
    [RSP+690 ] 0x14               (size_t)
    [RSP+698 ] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+6A0 ] 0x8000             (size_t)
    [RSP+6A8 ] 0x7FFC9C673911     (void* -> tbbmalloc.dll+0013911 scalable_free)
        xor ecx,ecx
    [RSP+6B0 ] 0x7FF6D92D8658     (BSScript::SimpleAllocMemoryPagePolicy*)
    [RSP+6B8 ] 0x4                (size_t)
    [RSP+6C0 ] 0x7FF6D92FFE20     (void* -> SkyrimSE.exe+31AFE20)
        add [rax],al
    [RSP+6C8 ] 0x7FF6D7575B3D     (void* -> SkyrimSE.exe+1425B3D)
        mov eax,[rdi]
    [RSP+6D0 ] 0x1EC86AA0E40      (void*)
    [RSP+6D8 ] 0x1EE9C43636C      (void*)
    [RSP+6E0 ] 0x70DF0F9CE0       (void*)
    [RSP+6E8 ] 0x70DF0F9D50       (void*)
    [RSP+6F0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+6F8 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+700 ] 0x0                (size_t)
    [RSP+708 ] 0x4                (size_t)
    [RSP+710 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+718 ] 0x14               (size_t)
    [RSP+720 ] 0x0                (size_t)
    [RSP+728 ] 0x7FF6D7587EFF     (void* -> SkyrimSE.exe+1437EFF)
        cmp [rbx],eax
    [RSP+730 ] 0x1                (size_t)
    [RSP+738 ] 0x400              (size_t)
    [RSP+740 ] 0x0                (size_t)
    [RSP+748 ] 0x70DF0FA330       (void*)
    [RSP+750 ] 0x2                (size_t)
    [RSP+758 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+760 ] 0x70DF0F9DC0       (void*)
    [RSP+768 ] 0x7FFC13B64545     (void* -> PapyrusTweaks.dll+0004545 LoggerHooks::ValidationSignaturesHook::thunk)
        [C:\Modding\SKSEDevelopment\PapyrusTweaks\src\LoggerHooks.h:44]
        add rsp,518h
    [RSP+770 ] 0x70DF0FA270       (void*)
    [RSP+778 ] 0x70DF0FA2B8       (void*)
    [RSP+780 ] 0x1ED00000014      (void*)
    [RSP+788 ] 0x1EE9C488400      (char*) "\x03"
    [RSP+790 ] 0x70DF0F9DA8       (void*)
    [RSP+798 ] 0x7FF6D64CCF3F     (void* -> SkyrimSE.exe+037CF3F)
        nop
    [RSP+7A0 ] 0x1EE00000400      (BSLightingShaderProperty*)
    [RSP+7A8 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+7B0 ] 0x1EDCFF88300      (void*)
    [RSP+7B8 ] 0x7FF6D75AF003     (void* -> SkyrimSE.exe+145F003)
        cmp [rbx],eax
    [RSP+7C0 ] 0x70DF0FA2B8       (void*)
    [RSP+7C8 ] 0x70DF0FA270       (void*)
    [RSP+7D0 ] 0x14               (size_t)
    [RSP+7D8 ] 0x1                (size_t)
    [RSP+7E0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+7E8 ] 0x7FF6D78B8440     (void* -> SkyrimSE.exe+1768440)
    [RSP+7F0 ] 0x1EDCFF90360      (void*)
    [RSP+7F8 ] 0x70DF0F9DA0       (void*)
    [RSP+800 ] 0x1EE9C48AC00      (void*)
    [RSP+808 ] 0x7FF6D759F16F     (void* -> SkyrimSE.exe+144F16F)
        nop
    [RSP+810 ] 0x1EDB02A64C0      (char*) "I\x06"
    [RSP+818 ] 0x70DF0F9DA0       (void*)
    [RSP+820 ] 0x70DF0F9DA0       (void*)
    [RSP+828 ] 0x1EDB02A64C0      (char*) "I\x06"
    [RSP+830 ] 0x7FF6D92FFE20     (void* -> SkyrimSE.exe+31AFE20)
        add [rax],al
    [RSP+838 ] 0x7FF6D7575B3D     (void* -> SkyrimSE.exe+1425B3D)
        mov eax,[rdi]
    [RSP+840 ] 0x1EDB02A64C0      (char*) "I\x06"
    [RSP+848 ] 0x1EDB02FFF00      (char*) "xA"
    [RSP+850 ] 0x0                (size_t)
    [RSP+858 ] 0x1EDB02FFF00      (char*) "xA"
    [RSP+860 ] 0x0                (size_t)
    [RSP+868 ] 0x80               (size_t)
    [RSP+870 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+878 ] 0x1EE9C4360C4      (void*)
    [RSP+880 ] 0x70DF0F9EC4       (char*) "p"
    [RSP+888 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+890 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+898 ] 0x7FF6D6E3D9DD     (void* -> SkyrimSE.exe+0CED9DD)
        mov r13,rax
    [RSP+8A0 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+8A8 ] 0x1EE9C4360C4      (void*)
    [RSP+8B0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+8B8 ] 0x1EE9C48ACB8      (char*) "\x06"
    [RSP+8C0 ] 0x0                (size_t)
    [RSP+8C8 ] 0x0                (size_t)
    [RSP+8D0 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+8D8 ] 0x70DF0FA008       (void*)
    [RSP+8E0 ] 0x1EE71E7BD80      (BSScript::Internal::CodeTasklet*)
    [RSP+8E8 ] 0x1EDCFF88101      (void*)
    [RSP+8F0 ] 0x1EDCFF90320      (BSTCommonLLMessageQueue<BSScript::Internal::FunctionMessage>*)
    [RSP+8F8 ] 0x7FF6D75ADE61     (void* -> SkyrimSE.exe+145DE61)
        test sil,sil
    [RSP+900 ] 0x1EDCFF88B20      (char*) "\x01"
    [RSP+908 ] 0x7FF6D6E3C87C     (void* -> SkyrimSE.exe+0CEC87C)
        mov rax,rbx
    [RSP+910 ] 0x14               (size_t)
    [RSP+918 ] 0x7FF6D757953F     (void* -> SkyrimSE.exe+142953F)
        test eax,eax
    [RSP+920 ] 0xFFFFFFFF00000001 (size_t)
    [RSP+928 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+930 ] 0x1EE71E7BD80      (BSScript::Internal::CodeTasklet*)
    [RSP+938 ] 0x7FF600000001     (size_t)
    [RSP+940 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+948 ] 0x1EE71E7BD80      (BSScript::Internal::CodeTasklet*)
    [RSP+950 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+958 ] 0x7FF6D75AEF0D     (void* -> SkyrimSE.exe+145EF0D)
        movzx ecx,al
    [RSP+960 ] 0x70DF0F9FA0       (void*)
    [RSP+968 ] 0x7FF6D6E3D9DD     (void* -> SkyrimSE.exe+0CED9DD)
        mov r13,rax
    [RSP+970 ] 0x70DF0FA070       (void*)
    [RSP+978 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+980 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+988 ] 0x7FF6D759DAAA     (void* -> SkyrimSE.exe+144DAAA)
        cmp [rbx],eax
    [RSP+990 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+998 ] 0x1                (size_t)
    [RSP+9A0 ] 0x0                (size_t)
    [RSP+9A8 ] 0x0                (size_t)
    [RSP+9B0 ] 0x1EC86AA0E00      (void*)
    [RSP+9B8 ] 0x70DF0FFAC0       (void*)
    [RSP+9C0 ] 0x2                (size_t)
    [RSP+9C8 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+9D0 ] 0x70DF0FA070       (void*)
    [RSP+9D8 ] 0x7FFC9C6757C3     (void* -> tbbmalloc.dll+00157C3 scalable_realloc)
        mov rbp,rax
    [RSP+9E0 ] 0x70DF0F9FA0       (void*)
    [RSP+9E8 ] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+9F0 ] 0x1EE046133D0      (char*) "\x07"
    [RSP+9F8 ] 0x1                (size_t)
    [RSP+A00 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+A08 ] 0x700000002        (size_t)
    [RSP+A10 ] 0x2                (size_t)
    [RSP+A18 ] 0x7FF6D759EDD5     (void* -> SkyrimSE.exe+144EDD5)
        nop
    [RSP+A20 ] 0x1EE046133D0      (char*) "\x07"
    [RSP+A28 ] 0x1ED00000083      (void*)
    [RSP+A30 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+A38 ] 0x7FFC9C6757C3     (void* -> tbbmalloc.dll+00157C3 scalable_realloc)
        mov rbp,rax
    [RSP+A40 ] 0x70DF0F9FE8       (void*)
    [RSP+A48 ] 0x70DF0F9FC0       (void*)
    [RSP+A50 ] 0x70DF0FA000       (void*)
    [RSP+A58 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+A60 ] 0x70DF0FA110       (char*) "\x01"
    [RSP+A68 ] 0x0                (size_t)
    [RSP+A70 ] 0x0                (size_t)
    [RSP+A78 ] 0x84               (size_t)
    [RSP+A80 ] 0x80               (size_t)
    [RSP+A88 ] 0x7FFC9C67372E     (void* -> tbbmalloc.dll+001372E scalable_malloc)
        mov rdi,rax
    [RSP+A90 ] 0x1EDB02FFF00      (char*) "xA"
    [RSP+A98 ] 0x1EDB02FFF00      (char*) "xA"
    [RSP+AA0 ] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+AA8 ] 0x1EDB02FFF00      (char*) "xA"
    [RSP+AB0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+AB8 ] 0x7FF6D92D8658     (BSScript::SimpleAllocMemoryPagePolicy*)
    [RSP+AC0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+AC8 ] 0x7FF6D758803B     (void* -> SkyrimSE.exe+143803B)
        jmp short 4
    [RSP+AD0 ] 0x70DF0FA138       (void*)
    [RSP+AD8 ] 0x7FF6D6E3D9DD     (void* -> SkyrimSE.exe+0CED9DD)
        mov r13,rax
    [RSP+AE0 ] 0x7FF6D92FFE20     (void* -> SkyrimSE.exe+31AFE20)
        add [rax],al
    [RSP+AE8 ] 0x7FF6D7575B3D     (void* -> SkyrimSE.exe+1425B3D)
        mov eax,[rdi]
    [RSP+AF0 ] 0x1EC86AA0E40      (void*)
    [RSP+AF8 ] 0x1EE9C436384      (char*) "\x02"
    [RSP+B00 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+B08 ] 0x70DF0FA110       (char*) "\x01"
    [RSP+B10 ] 0x0                (size_t)
    [RSP+B18 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+B20 ] 0x70DF0FA2B8       (void*)
    [RSP+B28 ] 0x70DF0FA201       (void*)
    [RSP+B30 ] 0x1EE71F8AE40      (char*) "\x02"
    [RSP+B38 ] 0x1EE9C436384      (char*) "\x02"
    [RSP+B40 ] 0x5                (size_t)
    [RSP+B48 ] 0x7FF6D6E3C752     (void* -> SkyrimSE.exe+0CEC752)
        nop
    [RSP+B50 ] 0x70DF0FA138       (void*)
    [RSP+B58 ] 0xA                (size_t)
    [RSP+B60 ] 0x1EC86AA0E40      (void*)
    [RSP+B68 ] 0x1EE9C488418      (char*) "\x0c"
    [RSP+B70 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+B78 ] 0x0                (size_t)
    [RSP+B80 ] 0x1EC86AA0E40      (void*)
    [RSP+B88 ] 0x7FF6D7575BCF     (void* -> SkyrimSE.exe+1425BCF)
        jmp 000000000000014Dh
    [RSP+B90 ] 0x1EC86AA0E40      (void*)
    [RSP+B98 ] 0x1EE9C436384      (char*) "\x02"
    [RSP+BA0 ] 0x1EE9C436344      (void*)
    [RSP+BA8 ] 0x1EE9C488400      (char*) "\x03"
    [RSP+BB0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+BB8 ] 0x7FF6D6E3C87C     (void* -> SkyrimSE.exe+0CEC87C)
        mov rax,rbx
    [RSP+BC0 ] 0x1                (size_t)
    [RSP+BC8 ] 0x0                (size_t)
    [RSP+BD0 ] 0x1EE9C436344      (void*)
    [RSP+BD8 ] 0x7FF6D7580C29     (void* -> SkyrimSE.exe+1430C29)
        mov rbx,[rsp+98h]
    [RSP+BE0 ] 0x1EE00000014      (void*)
    [RSP+BE8 ] 0x7FFC2297F37D     (void* -> ConsoleUtilSSE.dll+001F37D)
        lea r11,[rsp+90h]
    [RSP+BF0 ] 0x0                (size_t)
    [RSP+BF8 ] 0x1EE9C488400      (char*) "\x03"
    [RSP+C00 ] 0x70DF0FA1C0       (char*) "\xcb\x98\x01"
    [RSP+C08 ] 0x1                (size_t)
    [RSP+C10 ] 0x1EE71F8AE40      (char*) "\x02"
    [RSP+C18 ] 0x1                (size_t)
    [RSP+C20 ] 0x0                (size_t)
    [RSP+C28 ] 0x1EE9C488400      (char*) "\x03"
    [RSP+C30 ] 0x70DF0FA258       (void*)
    [RSP+C38 ] 0x70DF0FA270       (void*)
    [RSP+C40 ] 0x2                (size_t)
    [RSP+C48 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+C50 ] 0x0                (size_t)
    [RSP+C58 ] 0x7FF6D7582779     (void* -> SkyrimSE.exe+1432779)
        mov rbp,[rsp+78h]
    [RSP+C60 ] 0x1ED00000005      (void*)
    [RSP+C68 ] 0x70DF0FA270       (void*)
    [RSP+C70 ] 0x198CB            (size_t)
    [RSP+C78 ] 0x770B59B706EF     (size_t)
    [RSP+C80 ] 0x7FF6D92D86B8     (SkyrimScript::Logger*)
    [RSP+C88 ] 0x7FFC22988D73     (void* -> ConsoleUtilSSE.dll+0028D73)
        movzx r10d,byte ptr [rsp+60h]
    [RSP+C90 ] 0x1                (size_t)
    [RSP+C98 ] 0x0                (size_t)
    [RSP+CA0 ] 0x0                (size_t)
    [RSP+CA8 ] 0x70DF0FF3A8       (void*)
    [RSP+CB0 ] 0x2                (size_t)
    [RSP+CB8 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+CC0 ] 0x70DF0FA320       (void*)
    [RSP+CC8 ] 0x7FF6D759EAF9     (void* -> SkyrimSE.exe+144EAF9)
        mov r14d,eax
    [RSP+CD0 ] 0x1EE9C488400      (char*) "\x03"
    [RSP+CD8 ] 0x1EE00000014      (void*)
    [RSP+CE0 ] 0x7FF6D92D86B8     (SkyrimScript::Logger*)
    [RSP+CE8 ] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+CF0 ] 0x70DF0FA200       (char*) "\x02"
    [RSP+CF8 ] 0x70DF0FA2B8       (void*)
    [RSP+D00 ] 0x1EDB008E728      (char*) "ExecuteCommand"
    [RSP+D08 ] 0x1EDB02FCA80      (char*) "\x03"
    [RSP+D10 ] 0x0                (size_t)
    [RSP+D18 ] 0x7000000001       (size_t)
    [RSP+D20 ] 0x1EDB02D3420      (RE::NativeFunction<void (RE::StaticFunctionTag *,std::basic_string<char,std::char_traits<char>,std::allocator<char> >),void>*)
    [RSP+D28 ] 0x0                (size_t)
    [RSP+D30 ] 0x0                (size_t)
    [RSP+D38 ] 0x7FF600000014     (size_t)
    [RSP+D40 ] 0x1EDB00115C0      (char*) "\x02"
    [RSP+D48 ] 0x1EDB02FFF00      (char*) "xA"
    [RSP+D50 ] 0x1EE9C488400      (char*) "\x03"
    [RSP+D58 ] 0x1EDB0011700      (char*) "\x15"
    [RSP+D60 ] 0x0                (size_t)
    [RSP+D68 ] 0x1EC86AA1510      (ScrapHeap*)
    [RSP+D70 ] 0x1EE71F8AE40      (char*) "\x02"
    [RSP+D78 ] 0x7FF600000001     (size_t)
    [RSP+D80 ] 0x7000000001       (size_t)
    [RSP+D88 ] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+D90 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+D98 ] 0x1                (size_t)
    [RSP+DA0 ] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+DA8 ] 0x1EE03219300      (void*)
    [RSP+DB0 ] 0x1                (size_t)
    [RSP+DB8 ] 0x7FFCCB2C0DD0     (void* -> ucrtbase.dll+0060DD0 atol)
        mov eax,ebx
    [RSP+DC0 ] 0x0                (size_t)
    [RSP+DC8 ] 0x7FF6D7192377     (void* -> SkyrimSE.exe+1042377)
        mov rsi,[rsp+98h]
    [RSP+DD0 ] 0x1EE72CEB4A0      (void*)
    [RSP+DD8 ] 0x7FF6D72B1BF0     (void* -> SkyrimSE.exe+1161BF0)
        mov rax,[rsp+60h]
    [RSP+DE0 ] 0x0                (size_t)
    [RSP+DE8 ] 0x7FF6D7237E5E     (void* -> SkyrimSE.exe+10E7E5E)
        mov rcx,rbp
    [RSP+DF0 ] 0x1EF38829C30      (void*)
    [RSP+DF8 ] 0x2                (size_t)
    [RSP+E00 ] 0x1ECD8742A30      (char*) "\x10"
    [RSP+E08 ] 0x0                (size_t)
    [RSP+E10 ] 0x1EF3B04C000      (void*)
    [RSP+E18 ] 0x7FF6D72B1D5A     (void* -> SkyrimSE.exe+1161D5A)
        jmp short 000000000000000Bh
    [RSP+E20 ] 0x1EF3B04B7F0      (void*)
    [RSP+E28 ] 0x1EF3B000260      (void*)
    [RSP+E30 ] 0x1EF3B0002A0      (void*)
    [RSP+E38 ] 0x7F               (size_t)
    [RSP+E40 ] 0x70DF0FA301       (void*)
    [RSP+E48 ] 0x70DF0FF3F0       (void*)
    [RSP+E50 ] 0x1ECD8742A30      (char*) "\x10"
    [RSP+E58 ] 0x70DF0FA4B0       (void*)
    [RSP+E60 ] 0x0                (size_t)
    [RSP+E68 ] 0x1                (size_t)
    [RSP+E70 ] 0x1ECE4B4B198      (void*)
    [RSP+E78 ] 0x7FF6D723A35E     (void* -> SkyrimSE.exe+10EA35E)
        sub qword ptr [rsi+20h],1
    [RSP+E80 ] 0x1ECD8742A30      (char*) "\x10"
    [RSP+E88 ] 0x70DF0FA4B0       (void*)
    [RSP+E90 ] 0x1ECE4B4B0C0      (void*)
    [RSP+E98 ] 0x1EF3B04B7F0      (void*)
    [RSP+EA0 ] 0x1EF3B000260      (void*)
    [RSP+EA8 ] 0x7FF6D717E895     (void* -> SkyrimSE.exe+102E895)
        mov rbx,[rsp+30h]
    [RSP+EB0 ] 0x1EE7701E2D0      (char*) "\x01"
    [RSP+EB8 ] 0x70DF0FA4B0       (void*)
    [RSP+EC0 ] 0x1EF3B04B7F0      (void*)
    [RSP+EC8 ] 0x1EE7701E2D0      (char*) "\x01"
    [RSP+ED0 ] 0x8080             (size_t)
    [RSP+ED8 ] 0x7FF6D72620F8     (void* -> SkyrimSE.exe+11120F8)
        lea r11,[rsp+4F20h]
    [RSP+EE0 ] 0x1EE7701E2D0      (char*) "\x01"
    [RSP+EE8 ] 0x70DF0FA530       (void*)
    [RSP+EF0 ] 0x0                (size_t)
    [RSP+EF8 ] 0x0                (size_t)
    [RSP+F00 ] 0x1EE7701E2D0      (char*) "\x01"
    [RSP+F08 ] 0x1EC00000000      (size_t)
    [RSP+F10 ] 0xBA51B717B900B701 (size_t)
    [RSP+F18 ] 0x1EF3B04B7F0      (void*)
    [RSP+F20 ] 0x1A9              (size_t)
    [RSP+F28 ] 0x200              (size_t)
    [RSP+F30 ] 0x200              (size_t)
    [RSP+F38 ] 0x3E2A9D643F0EE900 (size_t)
    [RSP+F40 ] 0x1ECE4B4B0C0      (void*)
    [RSP+F48 ] 0x0                (size_t)
    [RSP+F50 ] 0x0                (size_t)
    [RSP+F58 ] 0x1EE032CED38      (void*)
    [RSP+F60 ] 0x1EE76BC75A0      (void*)
    [RSP+F68 ] 0x0                (size_t)
    [RSP+F70 ] 0x8                (size_t)
    [RSP+F78 ] 0x1EE7701E2D0      (char*) "\x01"
    [RSP+F80 ] 0x1EE7701E9D0      (void*)
    [RSP+F88 ] 0x1EE7701E9D0      (void*)
    [RSP+F90 ] 0x1                (size_t)
    [RSP+F98 ] 0x1EE7701E9B0      (void*)
    [RSP+FA0 ] 0x8                (size_t)
    [RSP+FA8 ] 0x0                (size_t)
    [RSP+FB0 ] 0x0                (size_t)
    [RSP+FB8 ] 0x0                (size_t)
    [RSP+FC0 ] 0x167F7FFFEE       (size_t)
    [RSP+FC8 ] 0x2                (size_t)
    [RSP+FD0 ] 0x2                (size_t)
    [RSP+FD8 ] 0x1ECD8742A30      (char*) "\x10"
    [RSP+FE0 ] 0x1EE032CED20      (void*)
    [RSP+FE8 ] 0x1EE03219380      (char*) "\x07"
    [RSP+FF0 ] 0x2                (size_t)
    [RSP+FF8 ] 0x70DF0FF3F0       (void*)
    [RSP+1000] 0x1EC00000001      (size_t)
    [RSP+1008] 0x70DF0FA468       (void*)
    [RSP+1010] 0x1ECD8742A20      (void*)
    [RSP+1018] 0x7FF600000001     (size_t)
    [RSP+1020] 0x70DF0FA468       (void*)
    [RSP+1028] 0x1ECD8F57E00      (hkCharControllerShape*)
    [RSP+1030] 0x7000000001       (size_t)
    [RSP+1038] 0x70DF0FA468       (void*)
    [RSP+1040] 0x70DF0FA5A0       (void*)
    [RSP+1048] 0x7FF6D6D3B8FF     (void* -> SkyrimSE.exe+0BEB8FF)
        mov r15,[rsp+870h]
    [RSP+1050] 0x8000000000000000 (size_t)
    [RSP+1058] 0x3D61494F3F7FFFFF (size_t)
    [RSP+1060] 0x300000001        (size_t)
    [RSP+1068] 0x30000000F        (size_t)
    [RSP+1070] 0x0                (size_t)
    [RSP+1078] 0x7FF6D6CB0C91     (void* -> SkyrimSE.exe+0B60C91)
        movzx eax,r15w
    [RSP+1080] 0x0                (size_t)
    [RSP+1088] 0x3F000008BF56E2EB (size_t)
    [RSP+1090] 0x0                (size_t)
    [RSP+1098] 0x3F000008BF56E2EB (size_t)
    [RSP+10A0] 0x1ECD873F500      (void*)
    [RSP+10A8] 0x3C2E69123C2E6912 (size_t)
    [RSP+10B0] 0xBF62AC7F3EB0C8A8 (size_t)
    [RSP+10B8] 0x3E44F279BE9F4577 (size_t)
    [RSP+10C0] 0xBEEC96D7BF39BD0D (size_t)
    [RSP+10C8] 0x3EB32CEE3F028D0A (size_t)
    [RSP+10D0] 0x3D4B3C38BF1864F3 (size_t)
    [RSP+10D8] 0x3EE7D30ABF4D4E58 (size_t)
    [RSP+10E0] 0x3DBB56BC3F33D91B (size_t)
    [RSP+10E8] 0xBEEFC71F3EF90A7B (size_t)
    [RSP+10F0] 0xBDC8E00000000001 (size_t)
    [RSP+10F8] 0x70DF0FA468       (void*)
    [RSP+1100] 0x4038498A3F6E3CCB (size_t)
    [RSP+1108] 0x1                (size_t)
    [RSP+1110] 0x70DF0FA468       (void*)
    [RSP+1118] 0xBF64F780         (size_t)
    [RSP+1120] 0xBF66F5FC00000001 (size_t)
    [RSP+1128] 0x70DF0FA468       (void*)
    [RSP+1130] 0x0                (size_t)
    [RSP+1138] 0x1                (size_t)
    [RSP+1140] 0x70DF0FA468       (void*)
    [RSP+1148] 0x3F00000200000000 (size_t)
    [RSP+1150] 0x40DBA5E3         (size_t)
    [RSP+1158] 0x3F00000000000000 (size_t)
    [RSP+1160] 0x40DBA5E300000000 (size_t)
    [RSP+1168] 0x3F00000100000001 (size_t)
    [RSP+1170] 0x70DF0FA468       (void*)
    [RSP+1178] 0x0                (size_t)
    [RSP+1180] 0x8000000000000000 (size_t)
    [RSP+1188] 0x3D61494F3F7FFFFF (size_t)
    [RSP+1190] 0x0                (size_t)
    [RSP+1198] 0x1                (size_t)
    [RSP+11A0] 0x70DF0FA468       (void*)
    [RSP+11A8] 0x0                (size_t)
    [RSP+11B0] 0x300000001        (size_t)
    [RSP+11B8] 0x30000000F        (size_t)
    [RSP+11C0] 0x70DF0FC620       (void*)
    [RSP+11C8] 0x1ECD8742A00      (char*) "P"
    [RSP+11D0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+11D8] 0x300000125        (size_t)
    [RSP+11E0] 0xB                (size_t)
    [RSP+11E8] 0xFFFFFFFFFFFFFFFF (size_t)
    [RSP+11F0] 0x0                (size_t)
    [RSP+11F8] 0x1                (size_t)
    [RSP+1200] 0x70DF0FA468       (void*)
    [RSP+1208] 0x0                (size_t)
    [RSP+1210] 0x3                (size_t)
    [RSP+1218] 0x0                (size_t)
    [RSP+1220] 0x0                (size_t)
    [RSP+1228] 0x0                (size_t)
    [RSP+1230] 0x0                (size_t)
    [RSP+1238] 0x7FF6D7B861C8     (char*) " INDENT=\"{0}\""
    [RSP+1240] 0x9                (size_t)
    [RSP+1248] 0x1EC00000002      (size_t)
    [RSP+1250] 0x70DF0FA908       (void*)
    [RSP+1258] 0x7FF6D7B86101     (void* -> SkyrimSE.exe+1A36101)
    [RSP+1260] 0x0                (size_t)
    [RSP+1268] 0x7FF6D7B861D4     (char*) "\""
    [RSP+1270] 0x7FF6D710C601     (void* -> SkyrimSE.exe+0FBC601)
        mov ecx,[rsp+30h]
    [RSP+1278] 0x4274E14542F8BA0F (size_t)
    [RSP+1280] 0x70DF0FAC30       (void*)
    [RSP+1288] 0x1ECD9340D70      (void*)
    [RSP+1290] 0x1ECD8F57E00      (hkCharControllerShape*)
    [RSP+1298] 0x70DF0FAEA0       (hkpTriangleShape*)
    [RSP+12A0] 0x3DCCCCCD         (size_t)
    [RSP+12A8] 0x3F00000000000000 (size_t)
    [RSP+12B0] 0x40DBA5E300000000 (size_t)
    [RSP+12B8] 0x3F00000100000000 (size_t)
    [RSP+12C0] 0xC2E7CF09438E4ACC (size_t)
    [RSP+12C8] 0x4274E14542FC13C7 (size_t)
    [RSP+12D0] 0xC2E77C25438E56AE (size_t)
    [RSP+12D8] 0x4274E14542F9E99E (size_t)
    [RSP+12E0] 0xC2E77C25438E56AE (size_t)
    [RSP+12E8] 0x4274E14542FC13C7 (size_t)
    [RSP+12F0] 0x3BDFCC49         (size_t)
    [RSP+12F8] 0x7FFC423C753D     (size_t)
    [RSP+1300] 0x70DF0FAAC0       (void*)
    [RSP+1308] 0xB00              (size_t)
    [RSP+1310] 0x7FF6D93DD708     (bhkCollisionFilter*)
    [RSP+1318] 0x7FF6D93DD708     (bhkCollisionFilter*)
    [RSP+1320] 0xBDCB38003D944000 (size_t)
    [RSP+1328] 0x0                (size_t)
    [RSP+1330] 0xBF6FD8463EB300A0 (size_t)
    [RSP+1338] 0x3C4D71CC00000000 (size_t)
    [RSP+1340] 0x0                (size_t)
    [RSP+1348] 0x0                (size_t)
    [RSP+1350] 0x0                (size_t)
    [RSP+1358] 0x0                (size_t)
    [RSP+1360] 0x0                (size_t)
    [RSP+1368] 0x0                (size_t)
    [RSP+1370] 0x0                (size_t)
    [RSP+1378] 0x0                (size_t)
    [RSP+1380] 0x0                (size_t)
    [RSP+1388] 0x0                (size_t)
    [RSP+1390] 0x4274E145         (size_t)
    [RSP+1398] 0x0                (size_t)
    [RSP+13A0] 0x42228781         (size_t)
    [RSP+13A8] 0x0                (size_t)
    [RSP+13B0] 0x0                (size_t)
    [RSP+13B8] 0x7FF6D7B5AB88     (void* -> SkyrimSE.exe+1A0AB88)
        xor [rsi],cl
    [RSP+13C0] 0x70DF0FA720       (void*)
    [RSP+13C8] 0x1                (size_t)
    [RSP+13D0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+13D8] 0x4271002042FA8021 (size_t)
    [RSP+13E0] 0x70DF0FA963       (char*) "0"
    [RSP+13E8] 0x1EDD8742A0A      (void*)
    [RSP+13F0] 0x0                (size_t)
    [RSP+13F8] 0x1ECD8742A3C      (char*) "\x01\x03\x01"
    [RSP+1400] 0x70DF0FAC00       (void*)
    [RSP+1408] 0x0                (size_t)
    [RSP+1410] 0x10030742A30      (size_t)
    [RSP+1418] 0x7FF6D6D64E1D     (void* -> SkyrimSE.exe+0C14E1D)
        mov r15,[rsp+170h]
    [RSP+1420] 0x1EC00000002      (size_t)
    [RSP+1428] 0x1ECD8742A10      (void*)
    [RSP+1430] 0x1ECD8742A30      (char*) "\x10"
    [RSP+1438] 0x1ECD8742A00      (char*) "P"
    [RSP+1440] 0x1ECD8742A3C      (char*) "\x01\x03\x01"
    [RSP+1448] 0x1ECD8742A20      (void*)
    [RSP+1450] 0x7000000000       (size_t)
    [RSP+1458] 0x70DF0FC620       (void*)
    [RSP+1460] 0x7F7FFFEE         (size_t)
    [RSP+1468] 0x0                (size_t)
    [RSP+1470] 0xC2E7CEA7438E4AE5 (size_t)
    [RSP+1478] 0x7FF6D7070161     (void* -> SkyrimSE.exe+0F20161)
        movaps xmm0,[rsi+100h]
    [RSP+1480] 0x70DF0FAEA0       (hkpTriangleShape*)
    [RSP+1488] 0x4274E14542F9E99E (size_t)
    [RSP+1490] 0xC2E77B93438E56E6 (size_t)
    [RSP+1498] 0x4274E14542FC13C7 (size_t)
    [RSP+14A0] 0x703A83126F       (size_t)
    [RSP+14A8] 0x70DF0FAA20       (void*)
    [RSP+14B0] 0x70DF0FAA30       (void*)
    [RSP+14B8] 0x70DF0FAA10       (void*)
    [RSP+14C0] 0x40DBA5E3         (size_t)
    [RSP+14C8] 0x3F80000000000000 (size_t)
    [RSP+14D0] 0x0                (size_t)
    [RSP+14D8] 0x3F80000000000000 (size_t)
    [RSP+14E0] 0x40DBA5E300000000 (size_t)
    [RSP+14E8] 0x3F80000000000000 (size_t)
    [RSP+14F0] 0x0                (size_t)
    [RSP+14F8] 0x3F80000000000000 (size_t)
    [RSP+1500] 0x0                (size_t)
    [RSP+1508] 0x3F80000000000000 (size_t)
    [RSP+1510] 0x3F8000003F800000 (size_t)
    [RSP+1518] 0x3F800000         (size_t)
    [RSP+1520] 0x40DBA5E3         (size_t)
    [RSP+1528] 0x3F00000000000000 (size_t)
    [RSP+1530] 0x0                (size_t)
    [RSP+1538] 0x3F00000200000000 (size_t)
    [RSP+1540] 0x40DBA5E3         (size_t)
    [RSP+1548] 0x3F00000000000000 (size_t)
    [RSP+1550] 0x408B26C2402982DE (size_t)
    [RSP+1558] 0x1584F6EEBC9E0000 (size_t)
    [RSP+1560] 0xBF6FD8463EB300A0 (size_t)
    [RSP+1568] 0x3C4D71CC00000000 (size_t)
    [RSP+1570] 0x3D4CCCCD3D4CCCCD (size_t)
    [RSP+1578] 0x3D23D70B3DCCCCCD (size_t)
    [RSP+1580] 0x7F7FFFEE         (size_t)
    [RSP+1588] 0x0                (size_t)
    [RSP+1590] 0x1ECD8743450      (char*) "\x01"
    [RSP+1598] 0x1ECD8742A10      (void*)
    [RSP+15A0] 0x1ECD8742A10      (void*)
    [RSP+15A8] 0x0                (size_t)
    [RSP+15B0] 0x0                (size_t)
    [RSP+15B8] 0x70DF0FA968       (void*)
    [RSP+15C0] 0x1A0              (size_t)
    [RSP+15C8] 0x7FF6D6DD6497     (void* -> SkyrimSE.exe+0C86497)
        mov r13,[rsp+10F8h]
    [RSP+15D0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+15D8] 0x300000125        (size_t)
    [RSP+15E0] 0xC                (size_t)
    [RSP+15E8] 0xFFFFFFFFFFFFFFFF (size_t)
    [RSP+15F0] 0x0                (size_t)
    [RSP+15F8] 0x7000000001       (size_t)
    [RSP+1600] 0x70DF0FA468       (void*)
    [RSP+1608] 0x70DF0FA5A0       (void*)
    [RSP+1610] 0x3                (size_t)
    [RSP+1618] 0x0                (size_t)
    [RSP+1620] 0x0                (size_t)
    [RSP+1628] 0x0                (size_t)
    [RSP+1630] 0x7000000000       (size_t)
    [RSP+1638] 0x7FF6D7B86220     (char*) " LEADING=\"{0}\""
    [RSP+1640] 0xA                (size_t)
    [RSP+1648] 0x1EC00000002      (size_t)
    [RSP+1650] 0x70DF0FAD08       (void*)
    [RSP+1658] 0x7FF6D7B86201     (void* -> SkyrimSE.exe+1A36201)
        add [rax],al
    [RSP+1660] 0x7000000000       (size_t)
    [RSP+1668] 0x7FF6D7B8622D     (char*) "\""
    [RSP+1670] 0x7FF6D7193201     (void* -> SkyrimSE.exe+1043201)
        adc al,ch
    [RSP+1678] 0x70DF0FAEA0       (hkpTriangleShape*)
    [RSP+1680] 0x7000060005       (size_t)
    [RSP+1688] 0x1ECD8A96970      (void*)
    [RSP+1690] 0x1ECD8A96820      (void*)
    [RSP+1698] 0x0                (size_t)
    [RSP+16A0] 0x1ECD8742C00      (void*)
    [RSP+16A8] 0x1ECD8743460      (void*)
    [RSP+16B0] 0x70DF0FABA8       (void*)
    [RSP+16B8] 0x70DF0FABC8       (void*)
    [RSP+16C0] 0x0                (size_t)
    [RSP+16C8] 0x1ECD8F56FA0      (void*)
    [RSP+16D0] 0x1ECD961C700      (hkpSimpleConstraintContactMgr*)
    [RSP+16D8] 0x1ECD8A96820      (void*)
    [RSP+16E0] 0xBF55A48FBF0D0AAA (size_t)
    [RSP+16E8] 0x0                (size_t)
    [RSP+16F0] 0xBF0D0AAA3F55A48F (size_t)
    [RSP+16F8] 0x0                (size_t)
    [RSP+1700] 0x8000000000000000 (size_t)
    [RSP+1708] 0x3F800000         (size_t)
    [RSP+1710] 0x4038498A3F6E3CCB (size_t)
    [RSP+1718] 0x80000000BF64F780 (size_t)
    [RSP+1720] 0x35D06000         (size_t)
    [RSP+1728] 0x7FF6D6BDCA29     (void* -> SkyrimSE.exe+0A8CA29)
        mov rbx,[rsp+40h]
    [RSP+1730] 0x0                (size_t)
    [RSP+1738] 0x0                (size_t)
    [RSP+1740] 0x70DF0F9B60       (char*) "\x06"
    [RSP+1748] 0x70DF0FAC50       (void*)
    [RSP+1750] 0x70DF0FAB50       (void*)
    [RSP+1758] 0x70DF0FAC40       (void*)
    [RSP+1760] 0x3DEDE985         (size_t)
    [RSP+1768] 0x7FF6D721FFB5     (void* -> SkyrimSE.exe+10CFFB5)
        mov rdi,rax
    [RSP+1770] 0xBF775DF63E83D76D (size_t)
    [RSP+1778] 0x0                (size_t)
    [RSP+1780] 0x70DF0F9B60       (char*) "\x06"
    [RSP+1788] 0x70DF0FACF0       (void*)
    [RSP+1790] 0x70DF0FAC70       (void*)
    [RSP+1798] 0x70DF0FACC0       (void*)
    [RSP+17A0] 0x70DF0F9AE0       (void*)
    [RSP+17A8] 0x70DF0FAD10       (void*)
    [RSP+17B0] 0x0                (size_t)
    [RSP+17B8] 0x7FF6D7B5AB88     (void* -> SkyrimSE.exe+1A0AB88)
        xor [rsi],cl
    [RSP+17C0] 0x70DF0FAB20       (void*)
    [RSP+17C8] 0x70DF0FAC01       (void*)
    [RSP+17D0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+17D8] 0x10020DF0FAC21    (size_t)
    [RSP+17E0] 0x70DF0FAD63       (char*) "3"
    [RSP+17E8] 0x71DF0FACEA       (size_t)
    [RSP+17F0] 0x3                (size_t)
    [RSP+17F8] 0xBF800000         (size_t)
    [RSP+1800] 0x70DF0F9AE0       (void*)
    [RSP+1808] 0x70DF0FAD70       (void*)
    [RSP+1810] 0x330FAAF0         (size_t)
    [RSP+1818] 0x70DF0FAD40       (char*) "\x03"
    [RSP+1820] 0x70DF0F99E0       (void*)
    [RSP+1828] 0x70DF0FAD90       (void*)
    [RSP+1830] 0x70DF0FAE90       (void*)
    [RSP+1838] 0x70DF0FAD40       (char*) "\x03"
    [RSP+1840] 0x70DF0F9B20       (void*)
    [RSP+1848] 0x70DF0FAD50       (void*)
    [RSP+1850] 0x70DF0FAF50       (void*)
    [RSP+1858] 0x70DF0FAD40       (char*) "\x03"
    [RSP+1860] 0x3F8423E4         (size_t)
    [RSP+1868] 0x70DF0FAD70       (void*)
    [RSP+1870] 0xBEE9DB643F62051D (size_t)
    [RSP+1878] 0x3DDF3DC3         (size_t)
    [RSP+1880] 0x70DF0F9A60       (void*)
    [RSP+1888] 0x70DF0FADF0       (void*)
    [RSP+1890] 0x70DF0FABF0       (void*)
    [RSP+1898] 0x70DF0FADC0       (void*)
    [RSP+18A0] 0x70DF0F9AA0       (void*)
    [RSP+18A8] 0x70DF0FAE10       (void*)
    [RSP+18B0] 0x70DF0FAB90       (char*) "\n"
    [RSP+18B8] 0x70DF0FADC0       (void*)
    [RSP+18C0] 0x70DF0F9BA0       (void*)
    [RSP+18C8] 0x70DF0FADD0       (void*)
    [RSP+18D0] 0x70DF0FAEF0       (void*)
    [RSP+18D8] 0x70DF0FADC0       (void*)
    [RSP+18E0] 0x3D098659         (size_t)
    [RSP+18E8] 0x7FF6D7061C80     (void* -> SkyrimSE.exe+0F11C80)
        mov r14,[rsp+30E8h]
    [RSP+18F0] 0xBF004B323F5D885C (size_t)
    [RSP+18F8] 0x0                (size_t)
    [RSP+1900] 0x70DF0F99E0       (void*)
    [RSP+1908] 0x70DF0FAE70       (void*)
    [RSP+1910] 0x70DF0FAC10       (void*)
    [RSP+1918] 0x70DF0FAE40       (void*)
    [RSP+1920] 0x70DF0F9A60       (void*)
    [RSP+1928] 0x70DF0FAE90       (void*)
    [RSP+1930] 0x70DF0FAED0       (void*)
    [RSP+1938] 0x70DF0FAE40       (void*)
    [RSP+1940] 0x70DF0F9B20       (void*)
    [RSP+1948] 0x70DF0FAE50       (void*)
    [RSP+1950] 0x7FF6D7ABA5A0     (void* -> SkyrimSE.exe+196A5A0)
        push rax
    [RSP+1958] 0x700001FFFF       (size_t)
    [RSP+1960] 0x0                (size_t)
    [RSP+1968] 0x4260F54E00000003 (size_t)
    [RSP+1970] 0xBF6C83D43BA3D70A (size_t)
    [RSP+1978] 0x3DEF             (size_t)
    [RSP+1980] 0x40DBA5E3         (size_t)
    [RSP+1988] 0x0                (size_t)
    [RSP+1990] 0x40DBA5E300000000 (size_t)
    [RSP+1998] 0x0                (size_t)
    [RSP+19A0] 0x0                (size_t)
    [RSP+19A8] 0x0                (size_t)
    [RSP+19B0] 0x0                (size_t)
    [RSP+19B8] 0x70DF0FAD68       (void*)
    [RSP+19C0] 0x1A0              (size_t)
    [RSP+19C8] 0x70DF0FAED0       (void*)
    [RSP+19D0] 0x70DF0FAF70       (void*)
    [RSP+19D8] 0x70DF0FAEC0       (void*)
    [RSP+19E0] 0x3CB834B0         (size_t)
    [RSP+19E8] 0x70DF0FAEF0       (void*)
    [RSP+19F0] 0xBF72301F3EA5E11A (size_t)
    [RSP+19F8] 0xBBB48E98         (size_t)
    [RSP+1A00] 0x70DF0F9AE0       (void*)
    [RSP+1A08] 0x70DF0FAF70       (void*)
    [RSP+1A10] 0x70DF0FAD90       (void*)
    [RSP+1A18] 0x70DF0FAF40       (void*)
    [RSP+1A20] 0x70DF0F9B20       (void*)
    [RSP+1A28] 0x70DF0FAF90       (void*)
    [RSP+1A30] 0x70DF0FAF10       (void*)
    [RSP+1A38] 0x70DF0FAF40       (void*)
    [RSP+1A40] 0x70DF0F9BA0       (void*)
    [RSP+1A48] 0x70DF0FAF50       (void*)
    [RSP+1A50] 0x70DF0FACF0       (void*)
    [RSP+1A58] 0x70DF0FAF40       (void*)
    [RSP+1A60] 0x3CDD97C3         (size_t)
    [RSP+1A68] 0x70DF0FAF70       (void*)
    [RSP+1A70] 0x70DF0F9D90       (void*)
    [RSP+1A78] 0x70DF0FAF80       (void*)
    [RSP+1A80] 0x70DF0FAF00       (void*)
    [RSP+1A88] 0x70DF0FAF70       (void*)
    [RSP+1A90] 0x3DF0854F         (size_t)
    [RSP+1A98] 0x0                (size_t)
    [RSP+1AA0] 0x3EC3ECD93F6C83D5 (size_t)
    [RSP+1AA8] 0x80000000         (size_t)
    [RSP+1AB0] 0x70DF0F9D50       (void*)
    [RSP+1AB8] 0x70DF0FB020       (void*)
    [RSP+1AC0] 0x70DF0FB0A0       (void*)
    [RSP+1AC8] 0x7FF6D75CA19C     (void* -> SkyrimSE.exe+147A19C)
        mov eax,[rbx+0F4h]
    [RSP+1AD0] 0x70DF0F9CD0       (char*) "\x14"
    [RSP+1AD8] 0x70DF0FB040       (char*) "\x01"
    [RSP+1AE0] 0x70DF0FB500       (void*)
    [RSP+1AE8] 0x70DF0FAFF0       (void*)
    [RSP+1AF0] 0x1                (size_t)
    [RSP+1AF8] 0x7FF6D6E6E32B     (void* -> SkyrimSE.exe+0D1E32B)
        add rbx,8
    [RSP+1B00] 0xFFFFFFFF         (size_t)
    [RSP+1B08] 0x0                (size_t)
    [RSP+1B10] 0x10               (size_t)
    [RSP+1B18] 0x1EE9ECDCA00      (void*)
    [RSP+1B20] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1B28] 0x7FF6D75CA136     (void* -> SkyrimSE.exe+147A136)
        mov rbx,[rsp+60h]
    [RSP+1B30] 0x1EE9ECDCA00      (void*)
    [RSP+1B38] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1B40] 0x1                (size_t)
    [RSP+1B48] 0xFFFFFFFF         (size_t)
    [RSP+1B50] 0x1ECD98D0160      (hkpListShape*)
    [RSP+1B58] 0x1ECD9746020      (`anonymous namespace'::hkpCompressedMeshShapeShared*)
    [RSP+1B60] 0x1ECA4CC82A0      (void*)
    [RSP+1B68] 0xFFFFFFFFFFFFFFFF (size_t)
    [RSP+1B70] 0x6000500000000    (size_t)
    [RSP+1B78] 0x1ECD8F57E00      (hkCharControllerShape*)
    [RSP+1B80] 0x70DF0FAEA0       (hkpTriangleShape*)
    [RSP+1B88] 0x7FF6D6E8FFE3     (void* -> SkyrimSE.exe+0D3FFE3)
        cmp byte ptr [rbx+11Dh],0
    [RSP+1B90] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1B98] 0x3F               (size_t)
    [RSP+1BA0] 0xBED03580BF19F3DC (size_t)
    [RSP+1BA8] 0x3F2F85333D5C3DDE (size_t)
    [RSP+1BB0] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1BB8] 0x7FF6D6F7860D     (void* -> SkyrimSE.exe+0E2860D)
        jmp short 0000000000000051h
    [RSP+1BC0] 0xFFFFFFFF         (size_t)
    [RSP+1BC8] 0x1EE9ECDCA00      (void*)
    [RSP+1BD0] 0x1ECD8F57000      (void*)
    [RSP+1BD8] 0x7FF6D6DD255F     (void* -> SkyrimSE.exe+0C8255F)
        movaps xmm3,[r14+60h]
    [RSP+1BE0] 0x1                (size_t)
    [RSP+1BE8] 0x70407FFFFE       (size_t)
    [RSP+1BF0] 0x70DF0F9E50       (void*)
    [RSP+1BF8] 0x70DF0FB100       (void*)
    [RSP+1C00] 0x3F066A22         (size_t)
    [RSP+1C08] 0x0                (size_t)
    [RSP+1C10] 0x70DF0FB700       (void*)
    [RSP+1C18] 0x7FF6D6DD2705     (void* -> SkyrimSE.exe+0C82705)
        movaps xmm2,[rsi]
    [RSP+1C20] 0x1                (size_t)
    [RSP+1C28] 0x1ECA4CC8290      (char*) "\x01"
    [RSP+1C30] 0x70DF0FB680       (void*)
    [RSP+1C38] 0x70DF0FB1A0       (void*)
    [RSP+1C40] 0xBF2DD5CEBE96D34E (size_t)
    [RSP+1C48] 0x3DD3EC7CBF2C2269 (size_t)
    [RSP+1C50] 0xBF3A0D7B3E1007DC (size_t)
    [RSP+1C58] 0xBF71F9D93F2C1DA8 (size_t)
    [RSP+1C60] 0x3DD3EC7CBF71F9D9 (size_t)
    [RSP+1C68] 0x3E9E8444         (size_t)
    [RSP+1C70] 0xC2E8726E438DD7B4 (size_t)
    [RSP+1C78] 0x424C8EBB42FB478C (size_t)
    [RSP+1C80] 0x3F10166B3F29D98E (size_t)
    [RSP+1C88] 0x3F47E9973EFC651E (size_t)
    [RSP+1C90] 0x3E8AB4803ED4AC65 (size_t)
    [RSP+1C98] 0xBF1F4F41BF5E4DA1 (size_t)
    [RSP+1CA0] 0x3F47E997BF1F4F41 (size_t)
    [RSP+1CA8] 0xBD5D6488         (size_t)
    [RSP+1CB0] 0xC2E89B27438DAB3C (size_t)
    [RSP+1CB8] 0x424C7B4742FA2085 (size_t)
    [RSP+1CC0] 0x3C809390BF68BB42 (size_t)
    [RSP+1CC8] 0x3D8C9B37BED520D8 (size_t)
    [RSP+1CD0] 0xBF38E8323E8E1DFA (size_t)
    [RSP+1CD8] 0x3D300E8DBF222921 (size_t)
    [RSP+1CE0] 0xBF310030BE9F0809 (size_t)
    [RSP+1CE8] 0xBD83E17D3F26FC2B (size_t)
    [RSP+1CF0] 0xBEC1C7303F0B36B6 (size_t)
    [RSP+1CF8] 0xBD133FF13E1126AE (size_t)
    [RSP+1D00] 0x3F74FEE0BD0AC840 (size_t)
    [RSP+1D08] 0xBEA16138BE937BFC (size_t)
    [RSP+1D10] 0xBEA97CE73F0A22C7 (size_t)
    [RSP+1D18] 0xBCD300903D3C0F4D (size_t)
    [RSP+1D20] 0xBCD912203E8C3E7A (size_t)
    [RSP+1D28] 0xBB81241CBD48C52F (size_t)
    [RSP+1D30] 0xBE4E4FCABE44B551 (size_t)
    [RSP+1D38] 0x3B9DF8BEBC9EF04F (size_t)
    [RSP+1D40] 0x1ECD946921C      (void*)
    [RSP+1D48] 0x1ECD946921D      (void*)
    [RSP+1D50] 0x3F800000         (size_t)
    [RSP+1D58] 0x0                (size_t)
    [RSP+1D60] 0xBEE1A43DBF13D99F (size_t)
    [RSP+1D68] 0x3F2EF7313D926546 (size_t)
    [RSP+1D70] 0x0                (size_t)
    [RSP+1D78] 0x7FF6D6D35C35     (void* -> SkyrimSE.exe+0BE5C35)
        movaps xmm0,[rbx+10h]
    [RSP+1D80] 0x3F800000         (size_t)
    [RSP+1D88] 0x0                (size_t)
    [RSP+1D90] 0x703DF507A1       (size_t)
    [RSP+1D98] 0x7FF6D6CC5CB8     (void* -> SkyrimSE.exe+0B75CB8)
        jmp 0FFFFFFFFFFFFFDA8h
    [RSP+1DA0] 0x0                (size_t)
    [RSP+1DA8] 0x0                (size_t)
    [RSP+1DB0] 0x0                (size_t)
    [RSP+1DB8] 0x0                (size_t)
    [RSP+1DC0] 0x40000000         (size_t)
    [RSP+1DC8] 0x0                (size_t)
    [RSP+1DD0] 0x2F5BE6FF         (size_t)
    [RSP+1DD8] 0x0                (size_t)
    [RSP+1DE0] 0x0                (size_t)
    [RSP+1DE8] 0x0                (size_t)
    [RSP+1DF0] 0x3DBB56BC3F33D91B (size_t)
    [RSP+1DF8] 0xBEEFC71F3EF90A7B (size_t)
    [RSP+1E00] 0x3F800000         (size_t)
    [RSP+1E08] 0x7FF6D6DCBAF1     (void* -> SkyrimSE.exe+0C7BAF1)
        test eax,eax
    [RSP+1E10] 0x3FA76772         (size_t)
    [RSP+1E18] 0x7FF63C81BBF2     (size_t)
    [RSP+1E20] 0x703F608EC9       (size_t)
    [RSP+1E28] 0x1EC3E2D316B      (size_t)
    [RSP+1E30] 0x70DF0FB5F0       (char*) "wCO?"
    [RSP+1E38] 0x1ECA4CC8310      (void*)
    [RSP+1E40] 0x880000009E       (size_t)
    [RSP+1E48] 0x700000000B       (size_t)
    [RSP+1E50] 0xBEC4E9C13DD64288 (size_t)
    [RSP+1E58] 0x3DC4A41CBDCF97F0 (size_t)
    [RSP+1E60] 0x3F9261D2         (size_t)
    [RSP+1E68] 0xB580000000000000 (size_t)
    [RSP+1E70] 0x0                (size_t)
    [RSP+1E78] 0x0                (size_t)
    [RSP+1E80] 0x0                (size_t)
    [RSP+1E88] 0x0                (size_t)
    [RSP+1E90] 0x4274E145         (size_t)
    [RSP+1E98] 0x0                (size_t)
    [RSP+1EA0] 0x4220A244         (size_t)
    [RSP+1EA8] 0x0                (size_t)
    [RSP+1EB0] 0x3F800000         (size_t)
    [RSP+1EB8] 0x0                (size_t)
    [RSP+1EC0] 0x3C85CD7B         (size_t)
    [RSP+1EC8] 0x0                (size_t)
    [RSP+1ED0] 0x7F7FFFEE         (size_t)
    [RSP+1ED8] 0x0                (size_t)
    [RSP+1EE0] 0x70DF0FB400       (void*)
    [RSP+1EE8] 0x1ECD8F93170      (void*)
    [RSP+1EF0] 0x1EE718DD600      (BSTriShape*)
    [RSP+1EF8] 0x7FF6D6F8056F     (void* -> SkyrimSE.exe+0E3056F)
        nop
    [RSP+1F00] 0x1ECD85F3D70      (void*)
    [RSP+1F08] 0x70DF0FB7D0       (void*)
    [RSP+1F10] 0x1ECD8CA5800      (void*)
    [RSP+1F18] 0x1ECD8CDB2C0      (char*) "\x01"
    [RSP+1F20] 0x1EF4308FA00      (BSTriShape*)
    [RSP+1F28] 0x7FF6D6F8056F     (void* -> SkyrimSE.exe+0E3056F)
        nop
    [RSP+1F30] 0x1ECE308F728      (void*)
    [RSP+1F38] 0x1ECD8CA5800      (void*)
    [RSP+1F40] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+1F48] 0x7FF6D6E87F88     (void* -> SkyrimSE.exe+0D37F88)
        nop
    [RSP+1F50] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+1F58] 0x7FF6D78B8440     (void* -> SkyrimSE.exe+1768440)
    [RSP+1F60] 0x1ECE308F728      (void*)
    [RSP+1F68] 0x3ED11211BF778BEA (size_t)
    [RSP+1F70] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+1F78] 0x7FF6D6E87F88     (void* -> SkyrimSE.exe+0D37F88)
        nop
    [RSP+1F80] 0x20               (size_t)
    [RSP+1F88] 0x3F               (size_t)
    [RSP+1F90] 0x20               (size_t)
    [RSP+1F98] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1FA0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+1FA8] 0x3F00000000000000 (size_t)
    [RSP+1FB0] 0x1EF4308FA00      (BSTriShape*)
    [RSP+1FB8] 0x7FF6D6E8FFE3     (void* -> SkyrimSE.exe+0D3FFE3)
        cmp byte ptr [rbx+11Dh],0
    [RSP+1FC0] 0x20               (size_t)
    [RSP+1FC8] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1FD0] 0xBE65223A3F99E588 (size_t)
    [RSP+1FD8] 0xBEEBD35FBD49E0BC (size_t)
    [RSP+1FE0] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+1FE8] 0x7FF6D6F7860D     (void* -> SkyrimSE.exe+0E2860D)
        jmp short 0000000000000051h
    [RSP+1FF0] 0xFFFFFFFF         (size_t)
    [RSP+1FF8] 0x1EF4308FA00      (BSTriShape*)
    [RSP+2000] 0x7F7FFFEE         (size_t)
    [RSP+2008] 0x0                (size_t)
    [RSP+2010] 0x3D5724F23F445BD0 (size_t)
    [RSP+2018] 0xBEF2672B3EDF4C4C (size_t)
    [RSP+2020] 0xBEAA05233F5F2421 (size_t)
    [RSP+2028] 0xBEC13E243EAB6650 (size_t)
    [RSP+2030] 0x70DF0FB680       (void*)
    [RSP+2038] 0x1ECA4CC8310      (void*)
    [RSP+2040] 0x1ECA4CC8310      (void*)
    [RSP+2048] 0x1ECD9746020      (`anonymous namespace'::hkpCompressedMeshShapeShared*)
    [RSP+2050] 0xBD5EF8923D944471 (size_t)
    [RSP+2058] 0x3F000010B63A65DB (size_t)
    [RSP+2060] 0xBB8D71433EF60FD7 (size_t)
    [RSP+2068] 0x3F000000B898BF46 (size_t)
    [RSP+2070] 0x0                (size_t)
    [RSP+2078] 0x0                (size_t)
    [RSP+2080] 0x3EC3123BBE268279 (size_t)
    [RSP+2088] 0x3F4BA714BEE26961 (size_t)
    [RSP+2090] 0x3E827C9400000000 (size_t)
    [RSP+2098] 0x3ED11211BF778BEA (size_t)
    [RSP+20A0] 0x3F4F4377         (size_t)
    [RSP+20A8] 0x3F00000500000000 (size_t)
    [RSP+20B0] 0x3DD521D700000000 (size_t)
    [RSP+20B8] 0x3F6F3184BECA2AB6 (size_t)
    [RSP+20C0] 0x1ECD8F93170      (void*)
    [RSP+20C8] 0x1ECD85F3C20      (void*)
    [RSP+20D0] 0x70DF0FBF50       (void*)
    [RSP+20D8] 0x0                (size_t)
    [RSP+20E0] 0x1ECD8F56FA0      (void*)
    [RSP+20E8] 0x1ECD8CDB2B0      (void*)
    [RSP+20F0] 0x1ECD8CDB280      (void*)
    [RSP+20F8] 0x7FF6D6D3B8FF     (void* -> SkyrimSE.exe+0BEB8FF)
        mov r15,[rsp+870h]
    [RSP+2100] 0x1ECD8CDB280      (void*)
    [RSP+2108] 0x70DF0FB750       (void*)
    [RSP+2110] 0x70DF0FB750       (void*)
    [RSP+2118] 0x1ECD8F56FA0      (void*)
    [RSP+2120] 0x70DF0FBF50       (void*)
    [RSP+2128] 0x3FC06C1BBDF4297E (size_t)
    [RSP+2130] 0x1ECD85F3C20      (void*)
    [RSP+2138] 0x1ECD8F93020      (void*)
    [RSP+2140] 0x0                (size_t)
    [RSP+2148] 0x1ECD8F56FA0      (void*)
    [RSP+2150] 0x1ECD873F500      (void*)
    [RSP+2158] 0x1EF3C080101      (void*)
    [RSP+2160] 0xBF62A78E3EAF3A3A (size_t)
    [RSP+2168] 0x3E474183BEA11746 (size_t)
    [RSP+2170] 0xBEEC1F20BF3B6166 (size_t)
    [RSP+2178] 0x3EB54A283F006603 (size_t)
    [RSP+2180] 0x3D7032B8BF16D359 (size_t)
    [RSP+2188] 0x3EE55AD9BF4E4E5F (size_t)
    [RSP+2190] 0x3DBEA2743F346009 (size_t)
    [RSP+2198] 0xBEF0AD043EFA635A (size_t)
    [RSP+21A0] 0x3DC8A2FF         (size_t)
    [RSP+21A8] 0x0                (size_t)
    [RSP+21B0] 0x39EAC1B4BB2928A7 (size_t)
    [RSP+21B8] 0x3BBD6E9F385CC771 (size_t)
    [RSP+21C0] 0x1ECD8CA5800      (void*)
    [RSP+21C8] 0xFFFFFFFF         (size_t)
    [RSP+21D0] 0x70DF0FB750       (void*)
    [RSP+21D8] 0x1ECD85F3C20      (void*)
    [RSP+21E0] 0x1ECD8A0D260      (hkpCapsuleShape*)
    [RSP+21E8] 0xFFFFFFFF         (size_t)
    [RSP+21F0] 0x70DF0FB790       (void*)
    [RSP+21F8] 0x1ECD8F93020      (void*)
    [RSP+2200] 0xBF247DDFBF41CD2F (size_t)
    [RSP+2208] 0x3F1A8CEFBDF29368 (size_t)
    [RSP+2210] 0x3EF1998ABF03423B (size_t)
    [RSP+2218] 0xBECF58903F379D7B (size_t)
    [RSP+2220] 0x3F1A8CEFBECF5890 (size_t)
    [RSP+2228] 0xBF2FCA28         (size_t)
    [RSP+2230] 0xC2E7BD18438DE94E (size_t)
    [RSP+2238] 0x4260B6B042FA274C (size_t)
    [RSP+2240] 0xBF53D5A33EA31CFD (size_t)
    [RSP+2248] 0xBDA04108BEECBBAE (size_t)
    [RSP+2250] 0x3F0E57333F146505 (size_t)
    [RSP+2258] 0x3F3FFFB3BF187E43 (size_t)
    [RSP+2260] 0xBDA041083F3FFFB3 (size_t)
    [RSP+2268] 0x3F2823EE         (size_t)
    [RSP+2270] 0xC2E7F7C4438D8603 (size_t)
    [RSP+2278] 0x4220DBB442F97346 (size_t)
    [RSP+2280] 0x70DF0FB710       (void*)
    [RSP+2288] 0x70DF0FB730       (void*)
    [RSP+2290] 0x0                (size_t)
    [RSP+2298] 0x1ECD8F56FA0      (void*)
    [RSP+22A0] 0x1ECD873F500      (void*)
    [RSP+22A8] 0x3F0000003E1127A8 (size_t)
    [RSP+22B0] 0xBF62AC7F3EB0C8A8 (size_t)
    [RSP+22B8] 0x3E44F279BE9F4577 (size_t)
    [RSP+22C0] 0xBEEC96D7BF39BD0D (size_t)
    [RSP+22C8] 0x3EB32CEE3F028D0A (size_t)
    [RSP+22D0] 0x3D4B3C38BF1864F3 (size_t)
    [RSP+22D8] 0x3EE7D30ABF4D4E58 (size_t)
    [RSP+22E0] 0x3DBB56BC3F33D91B (size_t)
    [RSP+22E8] 0xBEEFC71F3EF90A7B (size_t)
    [RSP+22F0] 0x3EA000B43F02D09D (size_t)
    [RSP+22F8] 0x3F72FA2E3F4CFEE8 (size_t)
    [RSP+2300] 0x3D1E44303F55DFFA (size_t)
    [RSP+2308] 0xBE4F1CFEBF0C5762 (size_t)
    [RSP+2310] 0x3F72FA2EBE4F1CFE (size_t)
    [RSP+2318] 0xBE772140         (size_t)
    [RSP+2320] 0x3F1FAC1D3FDB2F68 (size_t)
    [RSP+2328] 0x3FA84CF83D8829CC (size_t)
    [RSP+2330] 0xBF478ED53FE70C9D (size_t)
    [RSP+2338] 0x3E06AD583F274E6C (size_t)
    [RSP+2340] 0x0                (size_t)
    [RSP+2348] 0x0                (size_t)
    [RSP+2350] 0x0                (size_t)
    [RSP+2358] 0x0                (size_t)
    [RSP+2360] 0x0                (size_t)
    [RSP+2368] 0x3F00001000000000 (size_t)
    [RSP+2370] 0x3FC30FA2         (size_t)
    [RSP+2378] 0x3F00000000000000 (size_t)
    [RSP+2380] 0x1ED1F33D300      (BSTriShape*)
    [RSP+2388] 0x7FF6D6F8056F     (void* -> SkyrimSE.exe+0E3056F)
        nop
    [RSP+2390] 0x4220A244         (size_t)
    [RSP+2398] 0x0                (size_t)
    [RSP+23A0] 0xBDB91669BF7E80F2 (size_t)
    [RSP+23A8] 0x3FD899EDBD71E8BC (size_t)
    [RSP+23B0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+23B8] 0x7FF6D75CA19C     (void* -> SkyrimSE.exe+147A19C)
        mov eax,[rbx+0F4h]
    [RSP+23C0] 0x1ECE308F728      (void*)
    [RSP+23C8] 0x0                (size_t)
    [RSP+23D0] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+23D8] 0x7FF6D6E87F88     (void* -> SkyrimSE.exe+0D37F88)
        nop
    [RSP+23E0] 0x1                (size_t)
    [RSP+23E8] 0x7FF6D75CA19C     (void* -> SkyrimSE.exe+147A19C)
        mov eax,[rbx+0F4h]
    [RSP+23F0] 0xFFFFFFFF         (size_t)
    [RSP+23F8] 0x0                (size_t)
    [RSP+2400] 0x10               (size_t)
    [RSP+2408] 0x1EE718DDA80      (BSFadeNode*)
    [RSP+2410] 0x1                (size_t)
    [RSP+2418] 0x7FF6D6E6E32B     (void* -> SkyrimSE.exe+0D1E32B)
        add rbx,8
    [RSP+2420] 0xFFFFFFFF         (size_t)
    [RSP+2428] 0x0                (size_t)
    [RSP+2430] 0x8                (size_t)
    [RSP+2438] 0x1EF4308FB80      (BSFadeNode*)
    [RSP+2440] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+2448] 0x7FF6D75CA136     (void* -> SkyrimSE.exe+147A136)
        mov rbx,[rsp+60h]
    [RSP+2450] 0x1EF4308FB80      (BSFadeNode*)
    [RSP+2458] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+2460] 0x1                (size_t)
    [RSP+2468] 0xFFFFFFFF         (size_t)
    [RSP+2470] 0xC5FBCFC3469C3494 (size_t)
    [RSP+2478] 0x3F84CCCD460AD757 (size_t)
    [RSP+2480] 0x3F800000         (size_t)
    [RSP+2488] 0x0                (size_t)
    [RSP+2490] 0x3F800000         (size_t)
    [RSP+2498] 0x0                (size_t)
    [RSP+24A0] 0x1EF4308FB80      (BSFadeNode*)
    [RSP+24A8] 0x7FF6D6E8FFE3     (void* -> SkyrimSE.exe+0D3FFE3)
        cmp byte ptr [rbx+11Dh],0
    [RSP+24B0] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+24B8] 0x3F               (size_t)
    [RSP+24C0] 0x3DCCCCCD         (size_t)
    [RSP+24C8] 0x3F00000000000000 (size_t)
    [RSP+24D0] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+24D8] 0x7FF6D6F7860D     (void* -> SkyrimSE.exe+0E2860D)
        jmp short 0000000000000051h
    [RSP+24E0] 0xFFFFFFFF         (size_t)
    [RSP+24E8] 0x1EF4308FB80      (BSFadeNode*)
    [RSP+24F0] 0x3DDA5250BF7CB473 (size_t)
    [RSP+24F8] 0x3FC06C1BBDF4297E (size_t)
    [RSP+2500] 0x800              (size_t)
    [RSP+2508] 0x7FF6D6CC59F8     (void* -> SkyrimSE.exe+0B759F8)
        add rsp,68h
    [RSP+2510] 0x70DF0FBB20       (void*)
    [RSP+2518] 0x1ECD8ABB170      (void*)
    [RSP+2520] 0x1ECD8F56FA0      (void*)
    [RSP+2528] 0x1ECA4CC8290      (char*) "\x01"
    [RSP+2530] 0x7B00000032       (size_t)
    [RSP+2538] 0x1EC00000008      (size_t)
    [RSP+2540] 0x7400000029       (size_t)
    [RSP+2548] 0x7FF600000002     (size_t)
    [RSP+2550] 0x0                (size_t)
    [RSP+2558] 0x0                (size_t)
    [RSP+2560] 0x0                (size_t)
    [RSP+2568] 0x0                (size_t)
    [RSP+2570] 0x1ECD8FA7800      (hkpRigidBody*)
    [RSP+2578] 0x7FF6D711AA60     (void* -> SkyrimSE.exe+0FCAA60)
        cmp eax,17h
    [RSP+2580] 0x0                (size_t)
    [RSP+2588] 0x7FF6D7122D6B     (void* -> SkyrimSE.exe+0FD2D6B)
        movzx eax,bl
    [RSP+2590] 0x1ECD8F93C00      (hkpRigidBody*)
    [RSP+2598] 0x7FF6D711DA67     (void* -> SkyrimSE.exe+0FCDA67)
        add rsp,0F0h
    [RSP+25A0] 0x1ECA4CC8290      (char*) "\x01"
    [RSP+25A8] 0x8000080000000000 (size_t)
    [RSP+25B0] 0xBF1A2C0DC09F9217 (size_t)
    [RSP+25B8] 0x4989D3FF3DDCA542 (size_t)
    [RSP+25C0] 0x1EDD0CA9690      (void*)
    [RSP+25C8] 0x7FF6D712152F     (void* -> SkyrimSE.exe+0FD152F)
        test rax,rax
    [RSP+25D0] 0x1EF3B0C6188      (void*)
    [RSP+25D8] 0x1EF3B0C6150      (void*)
    [RSP+25E0] 0xC2E94E51438D7EF7 (size_t)
    [RSP+25E8] 0x42740F2242F9CD9B (size_t)
    [RSP+25F0] 0x70DF0FBE18       (void*)
    [RSP+25F8] 0x1EE733E3A30      (void*)
    [RSP+2600] 0x1EDD28EE578      (void*)
    [RSP+2608] 0x1EE73400250      (void*)
    [RSP+2610] 0x1EE733E3A10      (void*)
    [RSP+2618] 0x7FF6D7136643     (void* -> SkyrimSE.exe+0FE6643)
        movzx esi,al
    [RSP+2620] 0x0                (size_t)
    [RSP+2628] 0x1EE73400250      (void*)
    [RSP+2630] 0x1EF38E17E40      (void*)
    [RSP+2638] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+2640] 0x1ECD9469180      (char*) "("
    [RSP+2648] 0x12000000120      (size_t)
    [RSP+2650] 0x1EE73400250      (void*)
    [RSP+2658] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+2660] 0x1EE73400250      (void*)
    [RSP+2668] 0x7FF6D711AA60     (void* -> SkyrimSE.exe+0FCAA60)
        cmp eax,17h
    [RSP+2670] 0x1EF38E17E40      (void*)
    [RSP+2678] 0x7FF6D712B1F1     (void* -> SkyrimSE.exe+0FDB1F1)
        xor ecx,ecx
    [RSP+2680] 0x1EDD0F70200      (void*)
    [RSP+2688] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+2690] 0x0                (size_t)
    [RSP+2698] 0x0                (size_t)
    [RSP+26A0] 0x1EE271E12E0      (void*)
    [RSP+26A8] 0x0                (size_t)
    [RSP+26B0] 0x70DF0FC220       (void*)
    [RSP+26B8] 0x7FF6D7132720     (void* -> SkyrimSE.exe+0FE2720)
        add rsp,310h
    [RSP+26C0] 0x0                (size_t)
    [RSP+26C8] 0x70DF0FBD10       (void*)
    [RSP+26D0] 0x0                (size_t)
    [RSP+26D8] 0x1EE73400290      (char*) "\x02"
    [RSP+26E0] 0x70DF0FBC00       (void*)
    [RSP+26E8] 0x2                (size_t)
    [RSP+26F0] 0x70DF0FBC88       (void*)
    [RSP+26F8] 0x1EDD0CC4F90      (void*)
    [RSP+2700] 0x2                (size_t)
    [RSP+2708] 0x70DF0FC220       (void*)
    [RSP+2710] 0x1ED00000000      (void*)
    [RSP+2718] 0x1EDD0CC8600      (void*)
    [RSP+2720] 0x700100BDF0       (size_t)
    [RSP+2728] 0x0                (size_t)
    [RSP+2730] 0x1EDD28EE578      (void*)
    [RSP+2738] 0x1EDD28EE410      (void*)
    [RSP+2740] 0x1EE05293000      (void*)
    [RSP+2748] 0x0                (size_t)
    [RSP+2750] 0xE3600000E36      (size_t)
    [RSP+2758] 0x1EF00000E36      (void*)
    [RSP+2760] 0x1EDD0F70200      (void*)
    [RSP+2768] 0x1EE271E12E0      (void*)
    [RSP+2770] 0x7FF6D7B55970     (void* -> SkyrimSE.exe+1A05970)
        push rax
    [RSP+2778] 0x1EDD0D1C150      (Scaleform::TrueHUDMenu::Logger*)
    [RSP+2780] 0x1EDD0000100      (void*)
    [RSP+2788] 0x0                (size_t)
    [RSP+2790] 0x700005020F       (size_t)
    [RSP+2798] 0x1EE770F3000      (void*)
    [RSP+27A0] 0x0                (size_t)
    [RSP+27A8] 0x1EDD0CC4F90      (void*)
    [RSP+27B0] 0x1EDD0CC4F70      (void*)
    [RSP+27B8] 0x7FF6D712C719     (void* -> SkyrimSE.exe+0FDC719)
        mov rbx,[rsp+50h]
    [RSP+27C0] 0x70DF0FBDF0       (void*)
    [RSP+27C8] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+27D0] 0x1EDD0CC4F70      (void*)
    [RSP+27D8] 0x1EDD0CC4F70      (void*)
    [RSP+27E0] 0x1EDD0CA9318      (void*)
    [RSP+27E8] 0x70DF0FBDF0       (void*)
    [RSP+27F0] 0x0                (size_t)
    [RSP+27F8] 0x7FF6D7126EA1     (void* -> SkyrimSE.exe+0FD6EA1)
        mov rax,[rsi]
    [RSP+2800] 0x1EF38E17E60      (void*)
    [RSP+2808] 0x1EF38E17E60      (void*)
    [RSP+2810] 0x0                (size_t)
    [RSP+2818] 0x70DF0FBE50       (void*)
    [RSP+2820] 0x0                (size_t)
    [RSP+2828] 0x1ECD8ABB020      (void*)
    [RSP+2830] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+2838] 0x1ECD8F56FA0      (void*)
    [RSP+2840] 0x1EEF498E610      (void*)
    [RSP+2848] 0x7FF6D75B9948     (void* -> SkyrimSE.exe+1469948)
        mov rcx,rax
    [RSP+2850] 0x1EC00000120      (size_t)
    [RSP+2858] 0x1EF3B0C6170      (void*)
    [RSP+2860] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+2868] 0x7FF600000000     (size_t)
    [RSP+2870] 0x1                (size_t)
    [RSP+2878] 0x7FF6D6E6E32B     (void* -> SkyrimSE.exe+0D1E32B)
        add rbx,8
    [RSP+2880] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+2888] 0xC01480CD3FFCDF3A (size_t)
    [RSP+2890] 0x28               (size_t)
    [RSP+2898] 0x1ED1F32F880      (NiNode*)
    [RSP+28A0] 0x1ECE308F606      (void*)
    [RSP+28A8] 0x0                (size_t)
    [RSP+28B0] 0x1ECE308F600      (BSGeometryListCullingProcess*)
    [RSP+28B8] 0x1ED1F32F880      (NiNode*)
    [RSP+28C0] 0x1                (size_t)
    [RSP+28C8] 0x1EE05043870      (void*)
    [RSP+28D0] 0x1                (size_t)
    [RSP+28D8] 0x7FF6D6E6E32B     (void* -> SkyrimSE.exe+0D1E32B)
        add rbx,8
    [RSP+28E0] 0xFFFFFFFF         (size_t)
    [RSP+28E8] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+28F0] 0x1EE770F3000      (void*)
    [RSP+28F8] 0x1EE72023100      (NiNode*)
    [RSP+2900] 0x1EE770F30B0      (void*)
    [RSP+2908] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+2910] 0xFFFFFFFF         (size_t)
    [RSP+2918] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+2920] 0x1EDD0CC4F70      (void*)
    [RSP+2928] 0x1EDD0CC4F90      (void*)
    [RSP+2930] 0x2                (size_t)
    [RSP+2938] 0x1EDD28EE578      (void*)
    [RSP+2940] 0x1EDD0F702D8      (void*)
    [RSP+2948] 0x7FF6D758287A     (void* -> SkyrimSE.exe+143287A)
        cmp dword ptr [rbx+18h],0
    [RSP+2950] 0x1EE71F456C0      (char*) "\x02"
    [RSP+2958] 0x70DF0FEC30       (char*) "\x01"
    [RSP+2960] 0x0                (size_t)
    [RSP+2968] 0x1EDD28EE578      (void*)
    [RSP+2970] 0x70DF0FBEE0       (void*)
    [RSP+2978] 0x7FF6D723A35E     (void* -> SkyrimSE.exe+10EA35E)
        sub qword ptr [rsi+20h],1
    [RSP+2980] 0x1EE71EDE070      (BSScript::Internal::CodeTasklet*)
    [RSP+2988] 0x7FF6D75B9948     (void* -> SkyrimSE.exe+1469948)
        mov rcx,rax
    [RSP+2990] 0x1ED000000A0      (void*)
    [RSP+2998] 0x7FF6D758287A     (void* -> SkyrimSE.exe+143287A)
        cmp dword ptr [rbx+18h],0
    [RSP+29A0] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+29A8] 0x70DF0FEC80       (char*) "\x06"
    [RSP+29B0] 0x0                (size_t)
    [RSP+29B8] 0x1                (size_t)
    [RSP+29C0] 0x70DF0FBF30       (char*) "p"
    [RSP+29C8] 0x3                (size_t)
    [RSP+29D0] 0x1EE71E7BD80      (BSScript::Internal::CodeTasklet*)
    [RSP+29D8] 0x7FF6D75B9948     (void* -> SkyrimSE.exe+1469948)
        mov rcx,rax
    [RSP+29E0] 0x70               (size_t)
    [RSP+29E8] 0xFFFFFFFFFFFFFFFF (size_t)
    [RSP+29F0] 0x0                (size_t)
    [RSP+29F8] 0xBDC8E00000000002 (size_t)
    [RSP+2A00] 0x70DF0FA468       (void*)
    [RSP+2A08] 0x4038498A3F6E3CCB (size_t)
    [RSP+2A10] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+2A18] 0x0                (size_t)
    [RSP+2A20] 0x0                (size_t)
    [RSP+2A28] 0x0                (size_t)
    [RSP+2A30] 0x7000000000       (size_t)
    [RSP+2A38] 0x7FF6D7B86320     (char*) " FACE=\"{0}\""
    [RSP+2A40] 0x7                (size_t)
    [RSP+2A48] 0x1EC00000002      (size_t)
    [RSP+2A50] 0x70DF0FC108       (void*)
    [RSP+2A58] 0x7FF6D7B86301     (void* -> SkyrimSE.exe+1A36301)
        add [rax],al
    [RSP+2A60] 0x7000000000       (size_t)
    [RSP+2A68] 0x7FF6D7B8632A     (char*) "\""
    [RSP+2A70] 0x7FF6D7193201     (void* -> SkyrimSE.exe+1043201)
        adc al,ch
    [RSP+2A78] 0x1EDD28EE410      (void*)
    [RSP+2A80] 0x1EDD0F70200      (void*)
    [RSP+2A88] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+2A90] 0x0                (size_t)
    [RSP+2A98] 0x1EDD0CC4F70      (void*)
    [RSP+2AA0] 0x1EF3AE39AA0      (void*)
    [RSP+2AA8] 0x1                (size_t)
    [RSP+2AB0] 0x70DF0FC620       (void*)
    [RSP+2AB8] 0x7FF6D7132720     (void* -> SkyrimSE.exe+0FE2720)
        add rsp,310h
    [RSP+2AC0] 0x0                (size_t)
    [RSP+2AC8] 0x70DF0FC110       (void*)
    [RSP+2AD0] 0x0                (size_t)
    [RSP+2AD8] 0x0                (size_t)
    [RSP+2AE0] 0x70DF0FC000       (void*)
    [RSP+2AE8] 0x2                (size_t)
    [RSP+2AF0] 0x70DF0FC088       (void*)
    [RSP+2AF8] 0x1EE05051F90      (void*)
    [RSP+2B00] 0x2                (size_t)
    [RSP+2B08] 0x70DF0FC620       (void*)
    [RSP+2B10] 0x1EE00000000      (void*)
    [RSP+2B18] 0x1EDD0CC8640      (void*)
    [RSP+2B20] 0x700100C1F0       (size_t)
    [RSP+2B28] 0x0                (size_t)
    [RSP+2B30] 0x1EDD28EE578      (void*)
    [RSP+2B38] 0x1EDD28EE410      (void*)
    [RSP+2B40] 0x1EDFCC33000      (void*)
    [RSP+2B48] 0x0                (size_t)
    [RSP+2B50] 0x69C0000069C      (size_t)
    [RSP+2B58] 0x1EF0000069C      (void*)
    [RSP+2B60] 0x1EDD0F70200      (void*)
    [RSP+2B68] 0x1EF3AE39AA0      (void*)
    [RSP+2B70] 0x7FF6D7B55970     (void* -> SkyrimSE.exe+1A05970)
        push rax
    [RSP+2B78] 0x1EDD0D1C150      (Scaleform::TrueHUDMenu::Logger*)
    [RSP+2B80] 0x1EE05000100      (void*)
    [RSP+2B88] 0x0                (size_t)
    [RSP+2B90] 0x700005020F       (size_t)
    [RSP+2B98] 0x1EE26EF8C10      (void*)
    [RSP+2BA0] 0x3FF0000000000001 (size_t)
    [RSP+2BA8] 0x1EE05051F90      (void*)
    [RSP+2BB0] 0x0                (size_t)
    [RSP+2BB8] 0x7FF6D7B5AB88     (void* -> SkyrimSE.exe+1A0AB88)
        xor [rsi],cl
    [RSP+2BC0] 0x70DF0FBF20       (void*)
    [RSP+2BC8] 0x7FF6D711B901     (void* -> SkyrimSE.exe+0FCB901)
        add dh,[rbp+1Ah]
    [RSP+2BD0] 0x1EE0515A18C      (char*) "$EverywhereMediumFont"
    [RSP+2BD8] 0x15               (size_t)
    [RSP+2BE0] 0x1EDD0CA9318      (void*)
    [RSP+2BE8] 0x70DF0FC1F0       (void*)
    [RSP+2BF0] 0x0                (size_t)
    [RSP+2BF8] 0x7FF6D7126EA1     (void* -> SkyrimSE.exe+0FD6EA1)
        mov rax,[rsi]
    [RSP+2C00] 0x1EF38E17DE0      (void*)
    [RSP+2C08] 0x1EF38E17DE0      (void*)
    [RSP+2C10] 0x0                (size_t)
    [RSP+2C18] 0x70DF0FC250       (void*)
    [RSP+2C20] 0x70DF0FC1D8       (void*)
    [RSP+2C28] 0x1ECD8C26820      (void*)
    [RSP+2C30] 0x1ECD94876D0      (void*)
    [RSP+2C38] 0x1ECD9362300      (hkpContinuousSimulation*)
    [RSP+2C40] 0x70DF0FF508       (void*)
    [RSP+2C48] 0x7FF6D6CA27DF     (void* -> SkyrimSE.exe+0B527DF)
        add rsp,3280h
    [RSP+2C50] 0x1                (size_t)
    [RSP+2C58] 0x1EE26E4EC60      (void*)
    [RSP+2C60] 0x1ECD8C27400      (char*) "\x02\x03"
    [RSP+2C68] 0x1                (size_t)
    [RSP+2C70] 0x1EDD28EE578      (void*)
    [RSP+2C78] 0x7FF6D7582806     (void* -> SkyrimSE.exe+1432806)
        mov eax,r8d
    [RSP+2C80] 0x0                (size_t)
    [RSP+2C88] 0x70DF0FEFA0       (void*)
    [RSP+2C90] 0x0                (size_t)
    [RSP+2C98] 0x0                (size_t)
    [RSP+2CA0] 0x3FF0000000000000 (size_t)
    [RSP+2CA8] 0x0                (size_t)
    [RSP+2CB0] 0x1EEF498E610      (void*)
    [RSP+2CB8] 0x7FF6D75B9948     (void* -> SkyrimSE.exe+1469948)
        mov rcx,rax
    [RSP+2CC0] 0x7FF600000060     (size_t)
    [RSP+2CC8] 0x1EE05043810      (void*)
    [RSP+2CD0] 0x1EE9ECEF106      (void*)
    [RSP+2CD8] 0x0                (size_t)
    [RSP+2CE0] 0x1ECE7588340      (void*)
    [RSP+2CE8] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+2CF0] 0x70DF0FC3C0       (void*)
    [RSP+2CF8] 0x7FF6D711D2EE     (void* -> SkyrimSE.exe+0FCD2EE)
        jmp 000000000000027Ch
    [RSP+2D00] 0x1EDD28EE578      (void*)
    [RSP+2D08] 0x1EE05097890      (void*)
    [RSP+2D10] 0x70DF0FC3C0       (void*)
    [RSP+2D18] 0x7FF6D711D2EE     (void* -> SkyrimSE.exe+0FCD2EE)
        jmp 000000000000027Ch
    [RSP+2D20] 0x1EDD28EE578      (void*)
    [RSP+2D28] 0x1EE05097870      (void*)
    [RSP+2D30] 0x2                (size_t)
    [RSP+2D38] 0x1EDD28EE578      (void*)
    [RSP+2D40] 0x1EDD0F702D8      (void*)
    [RSP+2D48] 0x7FF6D723A35E     (void* -> SkyrimSE.exe+10EA35E)
        sub qword ptr [rsi+20h],1
    [RSP+2D50] 0x1EE26E4EC60      (void*)
    [RSP+2D58] 0x1EE26E4EC40      (void*)
    [RSP+2D60] 0x2                (size_t)
    [RSP+2D68] 0x1EDD28EE578      (void*)
    [RSP+2D70] 0x1EDD0F702D8      (void*)
    [RSP+2D78] 0x7FF6D711AA60     (void* -> SkyrimSE.exe+0FCAA60)
        cmp eax,17h
    [RSP+2D80] 0x1EE05051F70      (void*)
    [RSP+2D88] 0x1EDD0F75E40      (void*)
    [RSP+2D90] 0x1EDD0F75E40      (void*)
    [RSP+2D98] 0x7FF6D711DA67     (void* -> SkyrimSE.exe+0FCDA67)
        add rsp,0F0h
    [RSP+2DA0] 0x1EDD0F70200      (void*)
    [RSP+2DA8] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+2DB0] 0x1EE05051F70      (void*)
    [RSP+2DB8] 0x70DF0FC130       (void*)
    [RSP+2DC0] 0x1D8              (size_t)
    [RSP+2DC8] 0x7FF6D71215BB     (void* -> SkyrimSE.exe+0FD15BB)
        mov al,1
    [RSP+2DD0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+2DD8] 0x300000125        (size_t)
    [RSP+2DE0] 0x10               (size_t)
    [RSP+2DE8] 0xFFFFFFFFFFFFFFFF (size_t)
    [RSP+2DF0] 0x0                (size_t)
    [RSP+2DF8] 0xBF66F5FC00000001 (size_t)
    [RSP+2E00] 0x70DF0FA468       (void*)
    [RSP+2E08] 0x7FF6D758287A     (void* -> SkyrimSE.exe+143287A)
        cmp dword ptr [rbx+18h],0
    [RSP+2E10] 0x1EE71F456C0      (char*) "\x02"
    [RSP+2E18] 0x70DF0FF100       (void*)
    [RSP+2E20] 0x0                (size_t)
    [RSP+2E28] 0x0                (size_t)
    [RSP+2E30] 0x70DF0FC3A0       (void*)
    [RSP+2E38] 0x7FF6D7B86340     (char*) " COLOR=\"#{0:X:.6}\""
    [RSP+2E40] 0x1EE71EDE070      (BSScript::Internal::CodeTasklet*)
    [RSP+2E48] 0x7FF6D75B9948     (void* -> SkyrimSE.exe+1469948)
        mov rcx,rax
    [RSP+2E50] 0x70000000A0       (size_t)
    [RSP+2E58] 0x7FF6D7B86301     (void* -> SkyrimSE.exe+1A36301)
        add [rax],al
    [RSP+2E60] 0x7000000000       (size_t)
    [RSP+2E68] 0x7FF600000002     (size_t)
    [RSP+2E70] 0x7FF6D7193201     (void* -> SkyrimSE.exe+1043201)
        adc al,ch
    [RSP+2E78] 0x4007C083126E9780 (size_t)
    [RSP+2E80] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+2E88] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+2E90] 0x43F0000000000000 (size_t)
    [RSP+2E98] 0x0                (size_t)
    [RSP+2EA0] 0x1EE7279E0A0      (void*)
    [RSP+2EA8] 0x0                (size_t)
    [RSP+2EB0] 0x70DF0FCA20       (void*)
    [RSP+2EB8] 0x7FF6D7132720     (void* -> SkyrimSE.exe+0FE2720)
        add rsp,310h
    [RSP+2EC0] 0x0                (size_t)
    [RSP+2EC8] 0x70DF0FC510       (void*)
    [RSP+2ED0] 0x0                (size_t)
    [RSP+2ED8] 0x0                (size_t)
    [RSP+2EE0] 0x1ED00000001      (void*)
    [RSP+2EE8] 0x2                (size_t)
    [RSP+2EF0] 0x70DF0FC488       (void*)
    [RSP+2EF8] 0x1EE07255F90      (void*)
    [RSP+2F00] 0x2                (size_t)
    [RSP+2F08] 0x70DF0FCA20       (void*)
    [RSP+2F10] 0x1EE00000000      (void*)
    [RSP+2F18] 0x1EDD0CC8680      (void*)
    [RSP+2F20] 0x70010FC5F0       (size_t)
    [RSP+2F28] 0x0                (size_t)
    [RSP+2F30] 0x1EDD28EE578      (void*)
    [RSP+2F38] 0x1EDD28EE410      (void*)
    [RSP+2F40] 0x1EDFD225000      (void*)
    [RSP+2F48] 0x0                (size_t)
    [RSP+2F50] 0x162800001628     (size_t)
    [RSP+2F58] 0x1EF00001628      (void*)
    [RSP+2F60] 0x1EDD0F70200      (void*)
    [RSP+2F68] 0x1EE7279E0A0      (void*)
    [RSP+2F70] 0x7FF6D7B55970     (void* -> SkyrimSE.exe+1A05970)
        push rax
    [RSP+2F78] 0x1EDD0D1C150      (Scaleform::TrueHUDMenu::Logger*)
    [RSP+2F80] 0x1EE07000100      (void*)
    [RSP+2F88] 0x0                (size_t)
    [RSP+2F90] 0x5020F            (size_t)
    [RSP+2F98] 0x1EE72795C10      (void*)
    [RSP+2FA0] 0x4000000000000002 (size_t)
    [RSP+2FA8] 0x1EE07255F90      (void*)
    [RSP+2FB0] 0x0                (size_t)
    [RSP+2FB8] 0x7FF6D7B5AB88     (void* -> SkyrimSE.exe+1A0AB88)
        xor [rsi],cl
    [RSP+2FC0] 0x70DF0FC320       (void*)
    [RSP+2FC8] 0x7FF6D711B901     (void* -> SkyrimSE.exe+0FCB901)
        add dh,[rbp+1Ah]
    [RSP+2FD0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+2FD8] 0x100A026E4EC26    (size_t)
    [RSP+2FE0] 0x70DF0FC55E       (char*) "FFFFFF"
    [RSP+2FE8] 0x70DF0FC630       (void*)
    [RSP+2FF0] 0xFFFFFF           (size_t)
    [RSP+2FF8] 0x7FF6D7127231     (void* -> SkyrimSE.exe+0FD7231)
        add rsp,1D0h
    [RSP+3000] 0x0                (size_t)
    [RSP+3008] 0x4646000000000000 (size_t)
    [RSP+3010] 0x10046464646      (size_t)
    [RSP+3018] 0x70DF0FC650       (void*)
    [RSP+3020] 0x1EE7713B5C0      (char*) "\x02"
    [RSP+3028] 0x7FF6BF3AF1DE     (size_t)
    [RSP+3030] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3038] 0x3200000036060000 (size_t)
    [RSP+3040] 0x0                (size_t)
    [RSP+3048] 0x0                (size_t)
    [RSP+3050] 0x1EF43184600      (void*)
    [RSP+3058] 0x1EF3B0C6170      (void*)
    [RSP+3060] 0x1EE7713B5B8      (void*)
    [RSP+3068] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+3070] 0x1EE26E4EC40      (void*)
    [RSP+3078] 0x70DF0FC606       (void*)
    [RSP+3080] 0x0                (size_t)
    [RSP+3088] 0x7FF6BEF6F183     (size_t)
    [RSP+3090] 0x1E               (size_t)
    [RSP+3098] 0x0                (size_t)
    [RSP+30A0] 0x1EF3B0C6170      (void*)
    [RSP+30A8] 0x1EDD28EE648      (void*)
    [RSP+30B0] 0x2                (size_t)
    [RSP+30B8] 0x1EDD28EE578      (void*)
    [RSP+30C0] 0x1EDD0F702D8      (void*)
    [RSP+30C8] 0x7FF6D723A35E     (void* -> SkyrimSE.exe+10EA35E)
        sub qword ptr [rsi+20h],1
    [RSP+30D0] 0x1EE26E4EC40      (void*)
    [RSP+30D8] 0x1EE733AE800      (void*)
    [RSP+30E0] 0x1EE733AE800      (void*)
    [RSP+30E8] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+30F0] 0x1EE72795C10      (void*)
    [RSP+30F8] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+3100] 0x1EE26E4EC40      (void*)
    [RSP+3108] 0x1EDD28EE648      (void*)
    [RSP+3110] 0x1EE26E4EC40      (void*)
    [RSP+3118] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+3120] 0x1EE07255F70      (void*)
    [RSP+3128] 0x1EE07255F90      (void*)
    [RSP+3130] 0x2                (size_t)
    [RSP+3138] 0x1EDD28EE578      (void*)
    [RSP+3140] 0x1EE716FD494      (void*)
    [RSP+3148] 0x7FF6D64CCF3F     (void* -> SkyrimSE.exe+037CF3F)
        nop
    [RSP+3150] 0x1EE045AA160      (char*) "\x07"
    [RSP+3158] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+3160] 0x2                (size_t)
    [RSP+3168] 0x1EDD28EE578      (void*)
    [RSP+3170] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3178] 0x7FF6D711AA60     (void* -> SkyrimSE.exe+0FCAA60)
        cmp eax,17h
    [RSP+3180] 0x14               (size_t)
    [RSP+3188] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+3190] 0x70DF0FEC70       (void*)
    [RSP+3198] 0x7FF6D7575B3D     (void* -> SkyrimSE.exe+1425B3D)
        mov eax,[rdi]
    [RSP+31A0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+31A8] 0x1EE716FD4E4      (void*)
    [RSP+31B0] 0x14               (size_t)
    [RSP+31B8] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+31C0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+31C8] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+31D0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+31D8] 0x0                (size_t)
    [RSP+31E0] 0x70DF0FEC90       (void*)
    [RSP+31E8] 0x7FF6D7575B3D     (void* -> SkyrimSE.exe+1425B3D)
        mov eax,[rdi]
    [RSP+31F0] 0x1EC86AA0E40      (void*)
    [RSP+31F8] 0x1EE718A1434      (char*) "\x04"
    [RSP+3200] 0x1EE71EDE001      (void*)
    [RSP+3208] 0x0                (size_t)
    [RSP+3210] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3218] 0x0                (size_t)
    [RSP+3220] 0x0                (size_t)
    [RSP+3228] 0x0                (size_t)
    [RSP+3230] 0x1EE718A1434      (char*) "\x04"
    [RSP+3238] 0x7FF6D75B8B73     (void* -> SkyrimSE.exe+1468B73)
        jmp short 000000000000000Ah
    [RSP+3240] 0x1EE00000015      (void*)
    [RSP+3248] 0x1EC00000003      (size_t)
    [RSP+3250] 0x70DF0FF0F0       (void*)
    [RSP+3258] 0x0                (size_t)
    [RSP+3260] 0x70DF0FC7C8       (void*)
    [RSP+3268] 0x7FF6D7B8636B     (char*) "\""
    [RSP+3270] 0x7FF6D7190000     (void* -> SkyrimSE.exe+1040000)
        mov eax,[rcx]
    [RSP+3278] 0x1EE718A1434      (char*) "\x04"
    [RSP+3280] 0x0                (size_t)
    [RSP+3288] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+3290] 0x0                (size_t)
    [RSP+3298] 0x0                (size_t)
    [RSP+32A0] 0x1ED291CA080      (void*)
    [RSP+32A8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+32B0] 0x70DF0FCE20       (void*)
    [RSP+32B8] 0x7FF6D7132720     (void* -> SkyrimSE.exe+0FE2720)
        add rsp,310h
    [RSP+32C0] 0xC47              (size_t)
    [RSP+32C8] 0x70DF0FC910       (void*)
    [RSP+32D0] 0x0                (size_t)
    [RSP+32D8] 0x0                (size_t)
    [RSP+32E0] 0x1EDD0F70200      (void*)
    [RSP+32E8] 0x2                (size_t)
    [RSP+32F0] 0x70DF0FC888       (void*)
    [RSP+32F8] 0x1EE26A4CF90      (void*)
    [RSP+3300] 0x2                (size_t)
    [RSP+3308] 0x70DF0FCE20       (void*)
    [RSP+3310] 0x1EE00000000      (void*)
    [RSP+3318] 0x1EDD0CC8600      (void*)
    [RSP+3320] 0x70010FC9F0       (size_t)
    [RSP+3328] 0x0                (size_t)
    [RSP+3330] 0x1EDD28EE578      (void*)
    [RSP+3338] 0x1EDD28EE410      (void*)
    [RSP+3340] 0x1EE05293000      (void*)
    [RSP+3348] 0x0                (size_t)
    [RSP+3350] 0xC7400000C74      (size_t)
    [RSP+3358] 0x1EE00000C74      (void*)
    [RSP+3360] 0x1EDD0F70200      (void*)
    [RSP+3368] 0x1ED291CA080      (void*)
    [RSP+3370] 0x7FF6D7B55970     (void* -> SkyrimSE.exe+1A05970)
        push rax
    [RSP+3378] 0x1EDD0D1C150      (Scaleform::TrueHUDMenu::Logger*)
    [RSP+3380] 0x1EE26000100      (void*)
    [RSP+3388] 0x0                (size_t)
    [RSP+3390] 0x700005020F       (size_t)
    [RSP+3398] 0x1ED291D0000      (void*)
    [RSP+33A0] 0x0                (size_t)
    [RSP+33A8] 0x1EE26A4CF90      (void*)
    [RSP+33B0] 0x0                (size_t)
    [RSP+33B8] 0x7FF6D7B5AB88     (void* -> SkyrimSE.exe+1A0AB88)
        xor [rsi],cl
    [RSP+33C0] 0x70DF0FC720       (void*)
    [RSP+33C8] 0x7FF6D711B901     (void* -> SkyrimSE.exe+0FCB901)
        add dh,[rbp+1Ah]
    [RSP+33D0] 0x7FF6D7B54638     (void* -> SkyrimSE.exe+1A04638)
        shl byte ptr [rcx+11h],0D7h
    [RSP+33D8] 0x100A026A4CC26    (size_t)
    [RSP+33E0] 0x70DF0FC950       (char*) "1.000000"
    [RSP+33E8] 0x7000000000       (size_t)
    [RSP+33F0] 0x3FF0000000000000 (size_t)
    [RSP+33F8] 0x8                (size_t)
    [RSP+3400] 0x3030303030302E31 (size_t)
    [RSP+3408] 0x1EF38E17B00      (void*)
    [RSP+3410] 0x0                (size_t)
    [RSP+3418] 0x70DF0FCA50       (void*)
    [RSP+3420] 0x3F800000         (size_t)
    [RSP+3428] 0x70DF0FD548       (void*)
    [RSP+3430] 0x3F00003F3F00003F (size_t)
    [RSP+3438] 0x7FF6D6E6DB00     (void* -> SkyrimSE.exe+0D1DB00)
        mov rax,[rbx]
    [RSP+3440] 0x0                (size_t)
    [RSP+3448] 0x8001F00000000    (size_t)
    [RSP+3450] 0x1EE02FE5200      (void*)
    [RSP+3458] 0x1EE271D7100      (void*)
    [RSP+3460] 0x7FF6D93A80C4     (void* -> SkyrimSE.exe+32580C4)
        add [rax],al
    [RSP+3468] 0x1EE9EC88FC8      (void*)
    [RSP+3470] 0x1EDD28EE578      (void*)
    [RSP+3478] 0x7FF6D6E8F206     (void* -> SkyrimSE.exe+0D3F206)
        add bh,bh
    [RSP+3480] 0x0                (size_t)
    [RSP+3488] 0x0                (size_t)
    [RSP+3490] 0x70DF0FCAD0       (void*)
    [RSP+3498] 0x0                (size_t)
    [RSP+34A0] 0x4000000000000006 (size_t)
    [RSP+34A8] 0x0                (size_t)
    [RSP+34B0] 0x7                (size_t)
    [RSP+34B8] 0x7FF6D7268277     (void* -> SkyrimSE.exe+1118277)
        mov rbx,[rbp-20h]
    [RSP+34C0] 0x70DF0FF060       (void*)
    [RSP+34C8] 0x1EE050438D0      (void*)
    [RSP+34D0] 0x1EC86AA0E01      (void*)
    [RSP+34D8] 0x0                (size_t)
    [RSP+34E0] 0x1EEBECBA9DC      (void*)
    [RSP+34E8] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+34F0] 0x1ED291D0000      (void*)
    [RSP+34F8] 0x0                (size_t)
    [RSP+3500] 0x1ED291D00B0      (void*)
    [RSP+3508] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+3510] 0x1EF3B0C6170      (void*)
    [RSP+3518] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+3520] 0x1EE26A4CF70      (void*)
    [RSP+3528] 0x1EE26A4CF90      (void*)
    [RSP+3530] 0x2                (size_t)
    [RSP+3538] 0x1EDD28EE578      (void*)
    [RSP+3540] 0x1EDD0F702D8      (void*)
    [RSP+3548] 0x7FF6D723A35E     (void* -> SkyrimSE.exe+10EA35E)
        sub qword ptr [rsi+20h],1
    [RSP+3550] 0x1EE271D7100      (void*)
    [RSP+3558] 0x0                (size_t)
    [RSP+3560] 0x2                (size_t)
    [RSP+3568] 0x1EDD28EE578      (void*)
    [RSP+3570] 0x1EDD0F702D8      (void*)
    [RSP+3578] 0x7FF6D723A35E     (void* -> SkyrimSE.exe+10EA35E)
        sub qword ptr [rsi+20h],1
    [RSP+3580] 0x0                (size_t)
    [RSP+3588] 0x7FF6D7122D6B     (void* -> SkyrimSE.exe+0FD2D6B)
        movzx eax,bl
    [RSP+3590] 0x1EE733ACA00      (void*)
    [RSP+3598] 0x7FF6D711DA67     (void* -> SkyrimSE.exe+0FCDA67)
        add rsp,0F0h
    [RSP+35A0] 0x1EDD0F70200      (void*)
    [RSP+35A8] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+35B0] 0x70DF0FCB80       (char*) "\x15"
    [RSP+35B8] 0x70DF0FCAB0       (char*) "\x02"
    [RSP+35C0] 0x58               (size_t)
    [RSP+35C8] 0x7FF6D71215BB     (void* -> SkyrimSE.exe+0FD15BB)
        mov al,1
    [RSP+35D0] 0x1EE05097730      (void*)
    [RSP+35D8] 0x1EE271D70E0      (void*)
    [RSP+35E0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+35E8] 0x0                (size_t)
    [RSP+35F0] 0x14               (size_t)
    [RSP+35F8] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+3600] 0x1EDD28EE578      (void*)
    [RSP+3608] 0x1EE05097710      (char*) "\x03"
    [RSP+3610] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3618] 0x7FF6D7136643     (void* -> SkyrimSE.exe+0FE6643)
        movzx esi,al
    [RSP+3620] 0x14               (size_t)
    [RSP+3628] 0x7FF6D7575ABB     (void* -> SkyrimSE.exe+1425ABB)
        jmp short 000000000000000Bh
    [RSP+3630] 0x15               (size_t)
    [RSP+3638] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+3640] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3648] 0x1EE05097730      (void*)
    [RSP+3650] 0x70DF0FF1A0       (char*) "\x01\x12"
    [RSP+3658] 0x7FF6D7575C3C     (void* -> SkyrimSE.exe+1425C3C)
        test eax,eax
    [RSP+3660] 0x1EE01B10CD0      (char*) "\x07"
    [RSP+3668] 0x1EE71D61224      (void*)
    [RSP+3670] 0x811200000015     (size_t)
    [RSP+3678] 0x1EE716FD514      (void*)
    [RSP+3680] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3688] 0x0                (size_t)
    [RSP+3690] 0x0                (size_t)
    [RSP+3698] 0x0                (size_t)
    [RSP+36A0] 0x1EE71D61224      (void*)
    [RSP+36A8] 0x7FF6D75B8B73     (void* -> SkyrimSE.exe+1468B73)
        jmp short 000000000000000Ah
    [RSP+36B0] 0x15               (size_t)
    [RSP+36B8] 0x7FF600000006     (size_t)
    [RSP+36C0] 0x1EE01B10CD0      (char*) "\x07"
    [RSP+36C8] 0x0                (size_t)
    [RSP+36D0] 0x70DF0FCC38       (void*)
    [RSP+36D8] 0x0                (size_t)
    [RSP+36E0] 0x70DF0F0000       (void*)
    [RSP+36E8] 0x1EE71D61224      (void*)
    [RSP+36F0] 0x70DF0FCC88       (void*)
    [RSP+36F8] 0x1EE733AA430      (void*)
    [RSP+3700] 0x0                (size_t)
    [RSP+3708] 0x7FF6D62E49CE     (void* -> SkyrimSE.exe+01949CE)
        mov ebp,eax
    [RSP+3710] 0x70DF0FCD58       (void*)
    [RSP+3718] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3720] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3728] 0x0                (size_t)
    [RSP+3730] 0x70DF0FCD58       (void*)
    [RSP+3738] 0x7FF6D6E3E2D9     (void* -> SkyrimSE.exe+0CEE2D9)
        cmp [rbx],eax
    [RSP+3740] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3748] 0x70DF0FCD20       (void*)
    [RSP+3750] 0x0                (size_t)
    [RSP+3758] 0x70DF0FF108       (void*)
    [RSP+3760] 0x70DF0FE348       (void*)
    [RSP+3768] 0x70DF0FF118       (void*)
    [RSP+3770] 0x70DF0FF118       (void*)
    [RSP+3778] 0x70DF0FF070       (char*) "\x04"
    [RSP+3780] 0x70DF0FCED0       (void*)
    [RSP+3788] 0x7FF6D6E3C752     (void* -> SkyrimSE.exe+0CEC752)
        nop
    [RSP+3790] 0x70DF0FCD58       (void*)
    [RSP+3798] 0x7FF6D6E3C65E     (void* -> SkyrimSE.exe+0CEC65E)
        mov rax,[rsp+30h]
    [RSP+37A0] 0x1EEF4A1C400      (void*)
    [RSP+37A8] 0x70DF0FCD58       (void*)
    [RSP+37B0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+37B8] 0x7FF6D712C719     (void* -> SkyrimSE.exe+0FDC719)
        mov rbx,[rsp+50h]
    [RSP+37C0] 0x70DF0FF210       (void*)
    [RSP+37C8] 0x7FF6D6D152EA     (void* -> SkyrimSE.exe+0BC52EA)
        mov al,1
    [RSP+37D0] 0x1EDB0235780      (void*)
    [RSP+37D8] 0x70DF0FF070       (char*) "\x04"
    [RSP+37E0] 0x1EDD0CA9318      (void*)
    [RSP+37E8] 0x70DF0FCDF0       (void*)
    [RSP+37F0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+37F8] 0x7FF6D78B8160     (void* -> SkyrimSE.exe+1768160)
        sbb bh,cl
    [RSP+3800] 0x70DF0FF210       (void*)
    [RSP+3808] 0x0                (size_t)
    [RSP+3810] 0x3F8000003F733333 (size_t)
    [RSP+3818] 0x3FA5BB5B3F800000 (size_t)
    [RSP+3820] 0x70DF0FF000       (void*)
    [RSP+3828] 0x8                (size_t)
    [RSP+3830] 0x0                (size_t)
    [RSP+3838] 0x0                (size_t)
    [RSP+3840] 0x0                (size_t)
    [RSP+3848] 0x0                (size_t)
    [RSP+3850] 0x0                (size_t)
    [RSP+3858] 0x0                (size_t)
    [RSP+3860] 0x3F800000         (size_t)
    [RSP+3868] 0x0                (size_t)
    [RSP+3870] 0x1ECD97DFB00      (char*) "p"
    [RSP+3878] 0x7FF6D6D79135     (void* -> SkyrimSE.exe+0C29135)
        movzx edi,al
    [RSP+3880] 0x1ECD9488DC0      (hkbClipGenerator*)
    [RSP+3888] 0x1ECD9488DC0      (hkbClipGenerator*)
    [RSP+3890] 0x70DF0FCED0       (void*)
    [RSP+3898] 0x0                (size_t)
    [RSP+38A0] 0x70DF0FE348       (void*)
    [RSP+38A8] 0x0                (size_t)
    [RSP+38B0] 0x1                (size_t)
    [RSP+38B8] 0x1EDD28EE578      (void*)
    [RSP+38C0] 0x1EDD0F702D8      (void*)
    [RSP+38C8] 0x7FF6D9303BC0     (void* -> SkyrimSE.exe+31B3BC0)
        cwde
    [RSP+38D0] 0x1EE72793F01      (void*)
    [RSP+38D8] 0x1EF38817F00      (void*)
    [RSP+38E0] 0x1EF38817F00      (void*)
    [RSP+38E8] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+38F0] 0x69E2CD9B29039C01 (size_t)
    [RSP+38F8] 0x70DF0FF038       (void*)
    [RSP+3900] 0x1ED29039CC0      (void*)
    [RSP+3908] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+3910] 0x1ECD9488DC0      (hkbClipGenerator*)
    [RSP+3918] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+3920] 0x1EE733AA410      (void*)
    [RSP+3928] 0x1EE733AA430      (void*)
    [RSP+3930] 0x2                (size_t)
    [RSP+3938] 0x1EDD28EE578      (void*)
    [RSP+3940] 0x0                (size_t)
    [RSP+3948] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3950] 0x0                (size_t)
    [RSP+3958] 0x0                (size_t)
    [RSP+3960] 0x0                (size_t)
    [RSP+3968] 0x0                (size_t)
    [RSP+3970] 0x0                (size_t)
    [RSP+3978] 0x0                (size_t)
    [RSP+3980] 0x3F800000         (size_t)
    [RSP+3988] 0x0                (size_t)
    [RSP+3990] 0x0                (size_t)
    [RSP+3998] 0x70DF0FF108       (void*)
    [RSP+39A0] 0x70DF0FE348       (void*)
    [RSP+39A8] 0x70DF0FF118       (void*)
    [RSP+39B0] 0x1ECD97DFB00      (char*) "p"
    [RSP+39B8] 0x70DF0FF070       (char*) "\x04"
    [RSP+39C0] 0x70DF0FD020       (void*)
    [RSP+39C8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+39D0] 0x0                (size_t)
    [RSP+39D8] 0x70DF0FD020       (void*)
    [RSP+39E0] 0x70DF0FF118       (void*)
    [RSP+39E8] 0x1ECD9488DC0      (hkbClipGenerator*)
    [RSP+39F0] 0x70DF0FE348       (void*)
    [RSP+39F8] 0x70DF0FF030       (void*)
    [RSP+3A00] 0x1EDD2000001      (char*) "loat"
    [RSP+3A08] 0x70DF0FCF70       (void*)
    [RSP+3A10] 0x1EE00010000      (void*)
    [RSP+3A18] 0x7FF6D9303E40     (void* -> SkyrimSE.exe+31B3E40)
        fdiv st,st(2)
    [RSP+3A20] 0x1ECA4CC8E10      (void*)
    [RSP+3A28] 0x8000000200000000 (size_t)
    [RSP+3A30] 0x1ECA4CC8E10      (void*)
    [RSP+3A38] 0x1EE00000002      (void*)
    [RSP+3A40] 0x300000001        (size_t)
    [RSP+3A48] 0x70DF0FF038       (void*)
    [RSP+3A50] 0x1EE050976D0      (void*)
    [RSP+3A58] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+3A60] 0x1ECD86E4840      (hkbModifierGenerator*)
    [RSP+3A68] 0x7FF6D711A2F9     (void* -> SkyrimSE.exe+0FCA2F9)
        cmp eax,17h
    [RSP+3A70] 0x81129238DF0E     (size_t)
    [RSP+3A78] 0x1EDD28EE410      (void*)
    [RSP+3A80] 0x1EDD0F70200      (void*)
    [RSP+3A88] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+3A90] 0x0                (size_t)
    [RSP+3A98] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3AA0] 0x0                (size_t)
    [RSP+3AA8] 0x0                (size_t)
    [RSP+3AB0] 0x0                (size_t)
    [RSP+3AB8] 0x0                (size_t)
    [RSP+3AC0] 0x0                (size_t)
    [RSP+3AC8] 0x0                (size_t)
    [RSP+3AD0] 0x3F800000         (size_t)
    [RSP+3AD8] 0x0                (size_t)
    [RSP+3AE0] 0x0                (size_t)
    [RSP+3AE8] 0x70DF0FF108       (void*)
    [RSP+3AF0] 0x70DF0FE348       (void*)
    [RSP+3AF8] 0x70DF0FF118       (void*)
    [RSP+3B00] 0x1ECD97DFB00      (char*) "p"
    [RSP+3B08] 0x70DF0FF070       (char*) "\x04"
    [RSP+3B10] 0x70DF0FD170       (void*)
    [RSP+3B18] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+3B20] 0x0                (size_t)
    [RSP+3B28] 0x1ECD959DB80      (hkbStateMachine*)
    [RSP+3B30] 0x70DF0FF118       (void*)
    [RSP+3B38] 0x0                (size_t)
    [RSP+3B40] 0x70DF0FE348       (void*)
    [RSP+3B48] 0x70DF0FF030       (void*)
    [RSP+3B50] 0x29F900000001     (size_t)
    [RSP+3B58] 0x70DF0FD0C0       (void*)
    [RSP+3B60] 0x1ED00010000      (void*)
    [RSP+3B68] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+3B70] 0x1ECA4CC8D90      (void*)
    [RSP+3B78] 0x8000000100000000 (size_t)
    [RSP+3B80] 0x1ECA4CC8D90      (void*)
    [RSP+3B88] 0x1                (size_t)
    [RSP+3B90] 0x300050201        (size_t)
    [RSP+3B98] 0x70DF0FF038       (void*)
    [RSP+3BA0] 0x4000000000000002 (size_t)
    [RSP+3BA8] 0x1EE26F69F90      (void*)
    [RSP+3BB0] 0x1ECD959DB80      (hkbStateMachine*)
    [RSP+3BB8] 0x7FF6D712C719     (void* -> SkyrimSE.exe+0FDC719)
        mov rbx,[rsp+50h]
    [RSP+3BC0] 0x0                (size_t)
    [RSP+3BC8] 0x7FF6D711B9AA     (void* -> SkyrimSE.exe+0FCB9AA)
        xor edi,edi
    [RSP+3BD0] 0x1EE26F69F70      (void*)
    [RSP+3BD8] 0x1EE72793F60      (void*)
    [RSP+3BE0] 0x0                (size_t)
    [RSP+3BE8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3BF0] 0x0                (size_t)
    [RSP+3BF8] 0x0                (size_t)
    [RSP+3C00] 0x0                (size_t)
    [RSP+3C08] 0x0                (size_t)
    [RSP+3C10] 0x0                (size_t)
    [RSP+3C18] 0x0                (size_t)
    [RSP+3C20] 0x3F800000         (size_t)
    [RSP+3C28] 0x0                (size_t)
    [RSP+3C30] 0x0                (size_t)
    [RSP+3C38] 0x70DF0FF108       (void*)
    [RSP+3C40] 0x70DF0FE348       (void*)
    [RSP+3C48] 0x70DF0FF118       (void*)
    [RSP+3C50] 0x1ECD97DFB00      (char*) "p"
    [RSP+3C58] 0x70DF0FF070       (char*) "\x04"
    [RSP+3C60] 0x70DF0FD2C0       (void*)
    [RSP+3C68] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+3C70] 0x0                (size_t)
    [RSP+3C78] 0x70DF0FD2C0       (void*)
    [RSP+3C80] 0x70DF0FF118       (void*)
    [RSP+3C88] 0x0                (size_t)
    [RSP+3C90] 0x70DF0FE348       (void*)
    [RSP+3C98] 0x70DF0FF030       (void*)
    [RSP+3CA0] 0x1EE27000001      (void*)
    [RSP+3CA8] 0x70DF0FD210       (void*)
    [RSP+3CB0] 0x10000            (size_t)
    [RSP+3CB8] 0x7FF6D9303E40     (void* -> SkyrimSE.exe+31B3E40)
        fdiv st,st(2)
    [RSP+3CC0] 0x1ECA4CC8D10      (void*)
    [RSP+3CC8] 0x8000000200000000 (size_t)
    [RSP+3CD0] 0x1ECA4CC8D10      (void*)
    [RSP+3CD8] 0x1EF00000002      (void*)
    [RSP+3CE0] 0x338817F01        (size_t)
    [RSP+3CE8] 0x70DF0FF038       (void*)
    [RSP+3CF0] 0x1EE733FD950      (void*)
    [RSP+3CF8] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+3D00] 0x1ECD86E4660      (hkbModifierGenerator*)
    [RSP+3D08] 0x1EDD28EE648      (void*)
    [RSP+3D10] 0x70DF0FD3C0       (void*)
    [RSP+3D18] 0x7FF6D711D2EE     (void* -> SkyrimSE.exe+0FCD2EE)
        jmp 000000000000027Ch
    [RSP+3D20] 0x1EDD28EE578      (void*)
    [RSP+3D28] 0x1EE050975F0      (void*)
    [RSP+3D30] 0x0                (size_t)
    [RSP+3D38] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3D40] 0x0                (size_t)
    [RSP+3D48] 0x0                (size_t)
    [RSP+3D50] 0x0                (size_t)
    [RSP+3D58] 0x0                (size_t)
    [RSP+3D60] 0x0                (size_t)
    [RSP+3D68] 0x0                (size_t)
    [RSP+3D70] 0x3F800000         (size_t)
    [RSP+3D78] 0x0                (size_t)
    [RSP+3D80] 0x0                (size_t)
    [RSP+3D88] 0x70DF0FF108       (void*)
    [RSP+3D90] 0x70DF0FE348       (void*)
    [RSP+3D98] 0x70DF0FF118       (void*)
    [RSP+3DA0] 0x1ECD97DFB00      (char*) "p"
    [RSP+3DA8] 0x70DF0FF070       (char*) "\x04"
    [RSP+3DB0] 0x70DF0FD410       (void*)
    [RSP+3DB8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+3DC0] 0x0                (size_t)
    [RSP+3DC8] 0x1ECD8711400      (hkbStateMachine*)
    [RSP+3DD0] 0x70DF0FF118       (void*)
    [RSP+3DD8] 0x0                (size_t)
    [RSP+3DE0] 0x70DF0FE348       (void*)
    [RSP+3DE8] 0x70DF0FF030       (void*)
    [RSP+3DF0] 0x1                (size_t)
    [RSP+3DF8] 0x70DF0FD360       (void*)
    [RSP+3E00] 0x10000            (size_t)
    [RSP+3E08] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+3E10] 0x1ECA4CC8C90      (void*)
    [RSP+3E18] 0x8000000100000000 (size_t)
    [RSP+3E20] 0x1ECA4CC8C90      (void*)
    [RSP+3E28] 0xFFFFFFFF00000001 (size_t)
    [RSP+3E30] 0x3729F1001        (size_t)
    [RSP+3E38] 0x70DF0FF038       (void*)
    [RSP+3E40] 0x58               (size_t)
    [RSP+3E48] 0x1ECE5516F20      (void*)
    [RSP+3E50] 0x1ECD8711400      (hkbStateMachine*)
    [RSP+3E58] 0xEF20             (size_t)
    [RSP+3E60] 0x800              (size_t)
    [RSP+3E68] 0x7FF6D72B085E     (void* -> SkyrimSE.exe+116085E)
        test rax,rax
    [RSP+3E70] 0x800              (size_t)
    [RSP+3E78] 0xEF2              (size_t)
    [RSP+3E80] 0x0                (size_t)
    [RSP+3E88] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3E90] 0x0                (size_t)
    [RSP+3E98] 0x0                (size_t)
    [RSP+3EA0] 0x0                (size_t)
    [RSP+3EA8] 0x0                (size_t)
    [RSP+3EB0] 0x0                (size_t)
    [RSP+3EB8] 0x0                (size_t)
    [RSP+3EC0] 0x3F800000         (size_t)
    [RSP+3EC8] 0x0                (size_t)
    [RSP+3ED0] 0x0                (size_t)
    [RSP+3ED8] 0x70DF0FF108       (void*)
    [RSP+3EE0] 0x70DF0FE348       (void*)
    [RSP+3EE8] 0x70DF0FF118       (void*)
    [RSP+3EF0] 0x1ECD97DFB00      (char*) "p"
    [RSP+3EF8] 0x70DF0FF070       (char*) "\x04"
    [RSP+3F00] 0x70DF0FD560       (void*)
    [RSP+3F08] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+3F10] 0x0                (size_t)
    [RSP+3F18] 0x70DF0FD560       (void*)
    [RSP+3F20] 0x70DF0FF118       (void*)
    [RSP+3F28] 0x0                (size_t)
    [RSP+3F30] 0x70DF0FE348       (void*)
    [RSP+3F38] 0x70DF0FF030       (void*)
    [RSP+3F40] 0x1EF3C000001      (void*)
    [RSP+3F48] 0x70DF0FD4B0       (void*)
    [RSP+3F50] 0x1EF00010000      (void*)
    [RSP+3F58] 0x7FF6D9302900     (void* -> SkyrimSE.exe+31B2900)
        shl cl,1
    [RSP+3F60] 0x1ECA4CC8C10      (void*)
    [RSP+3F68] 0x8000000200000000 (size_t)
    [RSP+3F70] 0x1ECA4CC8C10      (void*)
    [RSP+3F78] 0x7FF600000002     (size_t)
    [RSP+3F80] 0x3DF0FD501        (size_t)
    [RSP+3F88] 0x70DF0FF038       (void*)
    [RSP+3F90] 0x1                (size_t)
    [RSP+3F98] 0x20               (size_t)
    [RSP+3FA0] 0x1EC9A4AEF10      (hkbBehaviorGraph*)
    [RSP+3FA8] 0x7FF6D93E7228     (void* -> SkyrimSE.exe+3297228)
        add [rax],al
    [RSP+3FB0] 0x1ECE7590010      (void*)
    [RSP+3FB8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3FC0] 0xFFFFFFFF         (size_t)
    [RSP+3FC8] 0x1EE0508DF10      (void*)
    [RSP+3FD0] 0x0                (size_t)
    [RSP+3FD8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+3FE0] 0x0                (size_t)
    [RSP+3FE8] 0x0                (size_t)
    [RSP+3FF0] 0x0                (size_t)
    [RSP+3FF8] 0x0                (size_t)
    [RSP+4000] 0x0                (size_t)
    [RSP+4008] 0x0                (size_t)
    [RSP+4010] 0x3F800000         (size_t)
    [RSP+4018] 0x0                (size_t)
    [RSP+4020] 0x0                (size_t)
    [RSP+4028] 0x70DF0FF108       (void*)
    [RSP+4030] 0x70DF0FE348       (void*)
    [RSP+4038] 0x70DF0FF118       (void*)
    [RSP+4040] 0x1ECD97DFB00      (char*) "p"
    [RSP+4048] 0x70DF0FF070       (char*) "\x04"
    [RSP+4050] 0x70DF0FD6B0       (void*)
    [RSP+4058] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+4060] 0x0                (size_t)
    [RSP+4068] 0x1EC9A27F190      (hkbBehaviorReferenceGenerator*)
    [RSP+4070] 0x70DF0FF118       (void*)
    [RSP+4078] 0x0                (size_t)
    [RSP+4080] 0x70DF0FE348       (void*)
    [RSP+4088] 0x70DF0FF030       (void*)
    [RSP+4090] 0x1EDD0000001      (void*)
    [RSP+4098] 0x70DF0FD600       (void*)
    [RSP+40A0] 0x1EE00010000      (void*)
    [RSP+40A8] 0x7FF6D9303850     (void* -> SkyrimSE.exe+31B3850)
        add bl,ch
    [RSP+40B0] 0x1ECA4CC8B90      (void*)
    [RSP+40B8] 0x8000000200000000 (size_t)
    [RSP+40C0] 0x1ECA4CC8B90      (void*)
    [RSP+40C8] 0x1EF00000002      (void*)
    [RSP+40D0] 0x3D0F70201        (size_t)
    [RSP+40D8] 0x70DF0FF038       (void*)
    [RSP+40E0] 0x1EE26A48C00      (void*)
    [RSP+40E8] 0x880              (size_t)
    [RSP+40F0] 0x1EC9A27F190      (hkbBehaviorReferenceGenerator*)
    [RSP+40F8] 0x7FF6D717E8AE     (void* -> SkyrimSE.exe+102E8AE)
        cmp rsi,[rdi+30h]
    [RSP+4100] 0x1EE76CCEF60      (void*)
    [RSP+4108] 0x1EDD28EE648      (void*)
    [RSP+4110] 0x1EE0508DF10      (void*)
    [RSP+4118] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+4120] 0x0                (size_t)
    [RSP+4128] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4130] 0x0                (size_t)
    [RSP+4138] 0x0                (size_t)
    [RSP+4140] 0x0                (size_t)
    [RSP+4148] 0x0                (size_t)
    [RSP+4150] 0x0                (size_t)
    [RSP+4158] 0x0                (size_t)
    [RSP+4160] 0x3F800000         (size_t)
    [RSP+4168] 0x0                (size_t)
    [RSP+4170] 0x0                (size_t)
    [RSP+4178] 0x70DF0FF108       (void*)
    [RSP+4180] 0x70DF0FE348       (void*)
    [RSP+4188] 0x70DF0FF118       (void*)
    [RSP+4190] 0x1ECD97DFB00      (char*) "p"
    [RSP+4198] 0x70DF0FF070       (char*) "\x04"
    [RSP+41A0] 0x70DF0FD800       (void*)
    [RSP+41A8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+41B0] 0x0                (size_t)
    [RSP+41B8] 0x1ECD8710F00      (hkbStateMachine*)
    [RSP+41C0] 0x70DF0FF118       (void*)
    [RSP+41C8] 0x0                (size_t)
    [RSP+41D0] 0x70DF0FE348       (void*)
    [RSP+41D8] 0x70DF0FF030       (void*)
    [RSP+41E0] 0x1                (size_t)
    [RSP+41E8] 0x70DF0FD750       (void*)
    [RSP+41F0] 0x10000            (size_t)
    [RSP+41F8] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+4200] 0x1ECA4CC8B10      (void*)
    [RSP+4208] 0x8000000100000000 (size_t)
    [RSP+4210] 0x1ECA4CC8B10      (void*)
    [RSP+4218] 0x1                (size_t)
    [RSP+4220] 0x300000001        (size_t)
    [RSP+4228] 0x70DF0FF038       (void*)
    [RSP+4230] 0x7000000000       (size_t)
    [RSP+4238] 0x7FF6D7B861F0     (char*) " LEFTMARGIN=\"{0}\""
    [RSP+4240] 0x1ECD8710F00      (hkbStateMachine*)
    [RSP+4248] 0x7FF600000002     (size_t)
    [RSP+4250] 0x70DF0FD908       (void*)
    [RSP+4258] 0x1                (size_t)
    [RSP+4260] 0x7000000000       (size_t)
    [RSP+4268] 0x7FF6D7B86200     (char*) "\""
    [RSP+4270] 0x0                (size_t)
    [RSP+4278] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4280] 0x0                (size_t)
    [RSP+4288] 0x0                (size_t)
    [RSP+4290] 0x0                (size_t)
    [RSP+4298] 0x0                (size_t)
    [RSP+42A0] 0x0                (size_t)
    [RSP+42A8] 0x0                (size_t)
    [RSP+42B0] 0x3F800000         (size_t)
    [RSP+42B8] 0x0                (size_t)
    [RSP+42C0] 0x0                (size_t)
    [RSP+42C8] 0x70DF0FF108       (void*)
    [RSP+42D0] 0x70DF0FE348       (void*)
    [RSP+42D8] 0x70DF0FF118       (void*)
    [RSP+42E0] 0x1ECD97DFB00      (char*) "p"
    [RSP+42E8] 0x70DF0FF070       (char*) "\x04"
    [RSP+42F0] 0x70DF0FD950       (void*)
    [RSP+42F8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+4300] 0x0                (size_t)
    [RSP+4308] 0x1ECD86D3540      (hkbStateMachine*)
    [RSP+4310] 0x70DF0FF118       (void*)
    [RSP+4318] 0x0                (size_t)
    [RSP+4320] 0x70DF0FE348       (void*)
    [RSP+4328] 0x70DF0FF030       (void*)
    [RSP+4330] 0x1EDD2000001      (char*) "loat"
    [RSP+4338] 0x70DF0FD8A0       (void*)
    [RSP+4340] 0x1EE00010000      (void*)
    [RSP+4348] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+4350] 0x1ECA4CC8A90      (void*)
    [RSP+4358] 0x8000000100000000 (size_t)
    [RSP+4360] 0x1ECA4CC8A90      (void*)
    [RSP+4368] 0x1EE00000001      (void*)
    [RSP+4370] 0x3D7B55901        (size_t)
    [RSP+4378] 0x70DF0FF038       (void*)
    [RSP+4380] 0x1EDD2000100      (char*) "float4"
    [RSP+4388] 0x0                (size_t)
    [RSP+4390] 0x1ECD86D3540      (hkbStateMachine*)
    [RSP+4398] 0x1EE769127B0      (void*)
    [RSP+43A0] 0x4014000000000005 (size_t)
    [RSP+43A8] 0x1EDD28E3F90      (void*)
    [RSP+43B0] 0x0                (size_t)
    [RSP+43B8] 0x7FF6D7B5AB88     (void* -> SkyrimSE.exe+1A0AB88)
        xor [rsi],cl
    [RSP+43C0] 0x0                (size_t)
    [RSP+43C8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+43D0] 0x0                (size_t)
    [RSP+43D8] 0x0                (size_t)
    [RSP+43E0] 0x0                (size_t)
    [RSP+43E8] 0x0                (size_t)
    [RSP+43F0] 0x0                (size_t)
    [RSP+43F8] 0x0                (size_t)
    [RSP+4400] 0x3F800000         (size_t)
    [RSP+4408] 0x0                (size_t)
    [RSP+4410] 0x0                (size_t)
    [RSP+4418] 0x70DF0FF108       (void*)
    [RSP+4420] 0x70DF0FE348       (void*)
    [RSP+4428] 0x70DF0FF118       (void*)
    [RSP+4430] 0x1ECD97DFB00      (char*) "p"
    [RSP+4438] 0x70DF0FF070       (char*) "\x04"
    [RSP+4440] 0x70DF0FDAA0       (void*)
    [RSP+4448] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+4450] 0x0                (size_t)
    [RSP+4458] 0x1ECD8CAE4E0      (hkbManualSelectorGenerator*)
    [RSP+4460] 0x70DF0FF118       (void*)
    [RSP+4468] 0x0                (size_t)
    [RSP+4470] 0x70DF0FE348       (void*)
    [RSP+4478] 0x70DF0FF030       (void*)
    [RSP+4480] 0x1                (size_t)
    [RSP+4488] 0x70DF0FD9F0       (void*)
    [RSP+4490] 0x1ED00000000      (void*)
    [RSP+4498] 0x7FF6D9303D40     (void* -> SkyrimSE.exe+31B3D40)
        push 0FFFFFFFFF6D7AAF0h
    [RSP+44A0] 0x1ECA4CC8A10      (void*)
    [RSP+44A8] 0x8000000100000000 (size_t)
    [RSP+44B0] 0x1ECA4CC8A10      (void*)
    [RSP+44B8] 0x1EE00000001      (void*)
    [RSP+44C0] 0x300000001        (size_t)
    [RSP+44C8] 0x70DF0FF038       (void*)
    [RSP+44D0] 0x1ED2E49BF18      (void*)
    [RSP+44D8] 0x7FF6D712275C     (void* -> SkyrimSE.exe+0FD275C)
        mov rbx,[rsp+40h]
    [RSP+44E0] 0x1ECD8CAE4E0      (hkbManualSelectorGenerator*)
    [RSP+44E8] 0x7FF6D72B1D65     (void* -> SkyrimSE.exe+1161D65)
        mov rbx,[rsp+60h]
    [RSP+44F0] 0x1EE769127B0      (void*)
    [RSP+44F8] 0x1EE050493D0      (void*)
    [RSP+4500] 0x70DF0FDE18       (void*)
    [RSP+4508] 0x70DF0FDA90       (void*)
    [RSP+4510] 0x0                (size_t)
    [RSP+4518] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4520] 0x0                (size_t)
    [RSP+4528] 0x0                (size_t)
    [RSP+4530] 0x0                (size_t)
    [RSP+4538] 0x0                (size_t)
    [RSP+4540] 0x0                (size_t)
    [RSP+4548] 0x0                (size_t)
    [RSP+4550] 0x3F800000         (size_t)
    [RSP+4558] 0x0                (size_t)
    [RSP+4560] 0x0                (size_t)
    [RSP+4568] 0x70DF0FF108       (void*)
    [RSP+4570] 0x70DF0FE348       (void*)
    [RSP+4578] 0x70DF0FF118       (void*)
    [RSP+4580] 0x1ECD97DFB00      (char*) "p"
    [RSP+4588] 0x70DF0FF070       (char*) "\x04"
    [RSP+4590] 0x70DF0FDBF0       (void*)
    [RSP+4598] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+45A0] 0x0                (size_t)
    [RSP+45A8] 0x70DF0FDBF0       (void*)
    [RSP+45B0] 0x70DF0FF118       (void*)
    [RSP+45B8] 0x0                (size_t)
    [RSP+45C0] 0x70DF0FE348       (void*)
    [RSP+45C8] 0x70DF0FF030       (void*)
    [RSP+45D0] 0x7FF6D7000001     (void* -> SkyrimSE.exe+0EB0001)
        mov eax,esp
    [RSP+45D8] 0x70DF0FDB40       (void*)
    [RSP+45E0] 0x10000            (size_t)
    [RSP+45E8] 0x7FF6D9303E40     (void* -> SkyrimSE.exe+31B3E40)
        fdiv st,st(2)
    [RSP+45F0] 0x1ECA4CC8990      (void*)
    [RSP+45F8] 0x8000000200000000 (size_t)
    [RSP+4600] 0x1ECA4CC8990      (void*)
    [RSP+4608] 0x1EC00000002      (size_t)
    [RSP+4610] 0x300000001        (size_t)
    [RSP+4618] 0x70DF0FF038       (void*)
    [RSP+4620] 0x0                (size_t)
    [RSP+4628] 0x0                (size_t)
    [RSP+4630] 0x1ECD8CAF620      (hkbModifierGenerator*)
    [RSP+4638] 0x7FF6D7B86208     (char*) " RIGHTMARGIN=\"{0}\""
    [RSP+4640] 0xE                (size_t)
    [RSP+4648] 0x7FF600000002     (size_t)
    [RSP+4650] 0x70DF0FDD08       (void*)
    [RSP+4658] 0x1                (size_t)
    [RSP+4660] 0x3E04C5613F28B796 (size_t)
    [RSP+4668] 0x3E37E5533ECFD036 (size_t)
    [RSP+4670] 0x418C000041080000 (size_t)
    [RSP+4678] 0x4178000040200000 (size_t)
    [RSP+4680] 0x40000000         (size_t)
    [RSP+4688] 0x0                (size_t)
    [RSP+4690] 0x2FDBE6FF         (size_t)
    [RSP+4698] 0x0                (size_t)
    [RSP+46A0] 0x7FFFFFFF         (size_t)
    [RSP+46A8] 0x0                (size_t)
    [RSP+46B0] 0x2FB240E7         (size_t)
    [RSP+46B8] 0x0                (size_t)
    [RSP+46C0] 0x0                (size_t)
    [RSP+46C8] 0x3F800000         (size_t)
    [RSP+46D0] 0x1ECD97DFB00      (char*) "p"
    [RSP+46D8] 0x7FF6D6DCC4A5     (void* -> SkyrimSE.exe+0C7C4A5)
        movsxd rdx,[rbx]
    [RSP+46E0] 0x422C537100000000 (size_t)
    [RSP+46E8] 0x421416F4C1E32F55 (size_t)
    [RSP+46F0] 0xBF800000         (size_t)
    [RSP+46F8] 0x0                (size_t)
    [RSP+4700] 0x3F800000         (size_t)
    [RSP+4708] 0x0                (size_t)
    [RSP+4710] 0x40000000         (size_t)
    [RSP+4718] 0x0                (size_t)
    [RSP+4720] 0x2FDBE6FF         (size_t)
    [RSP+4728] 0x0                (size_t)
    [RSP+4730] 0x7FFFFFFF         (size_t)
    [RSP+4738] 0x0                (size_t)
    [RSP+4740] 0x34EE46F2         (size_t)
    [RSP+4748] 0x0                (size_t)
    [RSP+4750] 0x0                (size_t)
    [RSP+4758] 0x3F0000093F6A161D (size_t)
    [RSP+4760] 0xC153B130         (size_t)
    [RSP+4768] 0x7FF6D6DCE513     (void* -> SkyrimSE.exe+0C7E513)
        cmp eax,7
    [RSP+4770] 0x4395C875         (size_t)
    [RSP+4778] 0x0                (size_t)
    [RSP+4780] 0x42FB3F14432DF160 (size_t)
    [RSP+4788] 0xCB94692D419364C2 (size_t)
    [RSP+4790] 0x42FB4636432DF81A (size_t)
    [RSP+4798] 0xCB94692D419364C2 (size_t)
    [RSP+47A0] 0xC1CB55C5C4A404FF (size_t)
    [RSP+47A8] 0xC45C6394         (size_t)
    [RSP+47B0] 0xC0840429BEA481AE (size_t)
    [RSP+47B8] 0x70DF0FE180       (void*)
    [RSP+47C0] 0x1ECD9463860      (hkCharControllerShape*)
    [RSP+47C8] 0x0                (size_t)
    [RSP+47D0] 0x70DF0FE220       (hkpClosestCdPointCollector*)
    [RSP+47D8] 0x70DF0FE450       (char*) "\x01"
    [RSP+47E0] 0x1ECA4CC8290      (char*) "\x01"
    [RSP+47E8] 0x70DF0FE930       (void*)
    [RSP+47F0] 0x418C02F3422C4D04 (size_t)
    [RSP+47F8] 0x418C02F3418C02F3 (size_t)
    [RSP+4800] 0x418C000041080000 (size_t)
    [RSP+4808] 0x4178000040200000 (size_t)
    [RSP+4810] 0x40000000         (size_t)
    [RSP+4818] 0x0                (size_t)
    [RSP+4820] 0x2F5BE6FF         (size_t)
    [RSP+4828] 0x0                (size_t)
    [RSP+4830] 0x7FFFFFFF         (size_t)
    [RSP+4838] 0x0                (size_t)
    [RSP+4840] 0x402D35D23EAEE170 (size_t)
    [RSP+4848] 0xBF827BC0         (size_t)
    [RSP+4850] 0x5                (size_t)
    [RSP+4858] 0x70DF0FE0F0       (void*)
    [RSP+4860] 0x70DF0FDE81       (void*)
    [RSP+4868] 0x7FF6D6DCBAA2     (void* -> SkyrimSE.exe+0C7BAA2)
        sub eax,1
    [RSP+4870] 0x70DF0FE050       (void*)
    [RSP+4878] 0x1ECA4CC8290      (char*) "\x01"
    [RSP+4880] 0x70DF0FE054       (char*) "p"
    [RSP+4888] 0x4060000040200000 (size_t)
    [RSP+4890] 0x70DF0FE054       (char*) "p"
    [RSP+4898] 0x0                (size_t)
    [RSP+48A0] 0x1                (size_t)
    [RSP+48A8] 0x0                (size_t)
    [RSP+48B0] 0x42FB3F14432DF160 (size_t)
    [RSP+48B8] 0x7FF6D757225A     (void* -> SkyrimSE.exe+142225A)
        xor ebx,ebx
    [RSP+48C0] 0x8000000000000000 (size_t)
    [RSP+48C8] 0x80000000C23C6E36 (size_t)
    [RSP+48D0] 0xC153EA40         (size_t)
    [RSP+48D8] 0x0                (size_t)
    [RSP+48E0] 0x1EE01B10CD0      (char*) "\x07"
    [RSP+48E8] 0x7FF6D7596CC4     (void* -> SkyrimSE.exe+1446CC4)
        mov rdi,rax
    [RSP+48F0] 0x70DF0FEC68       (void*)
    [RSP+48F8] 0x7FF6D757496B     (void* -> SkyrimSE.exe+142496B)
        nop
    [RSP+4900] 0x15               (size_t)
    [RSP+4908] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+4910] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4918] 0xCB94692D419364C2 (size_t)
    [RSP+4920] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4928] 0x70DF0FF1B0       (void*)
    [RSP+4930] 0x1EE71EDE070      (BSScript::Internal::CodeTasklet*)
    [RSP+4938] 0x70DF0FF1B0       (void*)
    [RSP+4940] 0x1EDB02A64C0      (char*) "I\x06"
    [RSP+4948] 0x7FF6D75B90D7     (void* -> SkyrimSE.exe+14690D7)
        test eax,eax
    [RSP+4950] 0x1EE01B10CD0      (char*) "\x07"
    [RSP+4958] 0x70DF0FEC90       (void*)
    [RSP+4960] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4968] 0x7FF6D62E49CE     (void* -> SkyrimSE.exe+01949CE)
        mov ebp,eax
    [RSP+4970] 0x70DF0FDFB8       (void*)
    [RSP+4978] 0x7FF6D6E3D9DD     (void* -> SkyrimSE.exe+0CED9DD)
        mov r13,rax
    [RSP+4980] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4988] 0x7FF6D6DF8CE6     (void* -> SkyrimSE.exe+0CA8CE6)
        mov r15,[rsp+310h]
    [RSP+4990] 0x70DF0FDFB8       (void*)
    [RSP+4998] 0x7FF6D6E3E2D9     (void* -> SkyrimSE.exe+0CEE2D9)
        cmp [rbx],eax
    [RSP+49A0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+49A8] 0x70DF0FDF80       (void*)
    [RSP+49B0] 0x0                (size_t)
    [RSP+49B8] 0x70DF0FF108       (void*)
    [RSP+49C0] 0x70DF0FF020       (void*)
    [RSP+49C8] 0x70DF0FF118       (void*)
    [RSP+49D0] 0x70DF0FF118       (void*)
    [RSP+49D8] 0x70DF0FF070       (char*) "\x04"
    [RSP+49E0] 0x70DF0FE130       (char*) "{\xcd\x85<"
    [RSP+49E8] 0x7FF6D6E3C752     (void* -> SkyrimSE.exe+0CEC752)
        nop
    [RSP+49F0] 0x70DF0FDFB8       (void*)
    [RSP+49F8] 0x7FF6D6E3C65E     (void* -> SkyrimSE.exe+0CEC65E)
        mov rax,[rsp+30h]
    [RSP+4A00] 0x1EEF4A1C400      (void*)
    [RSP+4A08] 0x70DF0FDFB8       (void*)
    [RSP+4A10] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4A18] 0x70DF0FE930       (void*)
    [RSP+4A20] 0x70DF0FF210       (void*)
    [RSP+4A28] 0x7FF6D6D152EA     (void* -> SkyrimSE.exe+0BC52EA)
        mov al,1
    [RSP+4A30] 0x1EDB01B4F70      (void*)
    [RSP+4A38] 0x70DF0FF070       (char*) "\x04"
    [RSP+4A40] 0x0                (size_t)
    [RSP+4A48] 0x3F7FFFFF         (size_t)
    [RSP+4A50] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4A58] 0x7FF6D78B8160     (void* -> SkyrimSE.exe+1768160)
        sbb bh,cl
    [RSP+4A60] 0x70DF0FF210       (void*)
    [RSP+4A68] 0x0                (size_t)
    [RSP+4A70] 0x3F8000003F800000 (size_t)
    [RSP+4A78] 0x3F9AC0863F800000 (size_t)
    [RSP+4A80] 0x70DF0FF000       (void*)
    [RSP+4A88] 0x0                (size_t)
    [RSP+4A90] 0x0                (size_t)
    [RSP+4A98] 0x0                (size_t)
    [RSP+4AA0] 0x0                (size_t)
    [RSP+4AA8] 0x0                (size_t)
    [RSP+4AB0] 0x7FFFFFFF         (size_t)
    [RSP+4AB8] 0x0                (size_t)
    [RSP+4AC0] 0x3C85CD7B         (size_t)
    [RSP+4AC8] 0x0                (size_t)
    [RSP+4AD0] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+4AD8] 0x7FF6D6D79135     (void* -> SkyrimSE.exe+0C29135)
        movzx edi,al
    [RSP+4AE0] 0x1ECD978C3C0      (hkbClipGenerator*)
    [RSP+4AE8] 0x1ECD978C3C0      (hkbClipGenerator*)
    [RSP+4AF0] 0x70DF0FE130       (char*) "{\xcd\x85<"
    [RSP+4AF8] 0x70DF0FE5E0       (void*)
    [RSP+4B00] 0x70DF0FF020       (void*)
    [RSP+4B08] 0x3F7FFFFF         (size_t)
    [RSP+4B10] 0x1                (size_t)
    [RSP+4B18] 0x3F7FFFFF         (size_t)
    [RSP+4B20] 0x60017            (size_t)
    [RSP+4B28] 0x7FF6D9303BC0     (void* -> SkyrimSE.exe+31B3BC0)
        cwde
    [RSP+4B30] 0x1ECD8A96820      (void*)
    [RSP+4B38] 0x7FF6D7067ABB     (void* -> SkyrimSE.exe+0F17ABB)
        nop
    [RSP+4B40] 0x7FF6D7A28328     (void* -> SkyrimSE.exe+18D8328)
        test [rdx+7FF6D6h],bl
    [RSP+4B48] 0x36               (size_t)
    [RSP+4B50] 0x79ACC41200000001 (size_t)
    [RSP+4B58] 0x70DF0FF038       (void*)
    [RSP+4B60] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4B68] 0x42F8B98D         (size_t)
    [RSP+4B70] 0x1ECD978C3C0      (hkbClipGenerator*)
    [RSP+4B78] 0x42F8B98D         (size_t)
    [RSP+4B80] 0x0                (size_t)
    [RSP+4B88] 0x3D4CCE803F7FFFFF (size_t)
    [RSP+4B90] 0xC2A7D99C         (size_t)
    [RSP+4B98] 0x0                (size_t)
    [RSP+4BA0] 0x0                (size_t)
    [RSP+4BA8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4BB0] 0x0                (size_t)
    [RSP+4BB8] 0x0                (size_t)
    [RSP+4BC0] 0x0                (size_t)
    [RSP+4BC8] 0x0                (size_t)
    [RSP+4BD0] 0x7FFFFFFF         (size_t)
    [RSP+4BD8] 0x0                (size_t)
    [RSP+4BE0] 0x3C85CD7B         (size_t)
    [RSP+4BE8] 0x0                (size_t)
    [RSP+4BF0] 0x0                (size_t)
    [RSP+4BF8] 0x70DF0FF108       (void*)
    [RSP+4C00] 0x70DF0FF020       (void*)
    [RSP+4C08] 0x70DF0FF118       (void*)
    [RSP+4C10] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+4C18] 0x70DF0FF070       (char*) "\x04"
    [RSP+4C20] 0x70DF0FE280       (char*) "{\xcd\x85<"
    [RSP+4C28] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+4C30] 0x0                (size_t)
    [RSP+4C38] 0x1ECD9358DC0      (hkbStateMachine*)
    [RSP+4C40] 0x70DF0FF118       (void*)
    [RSP+4C48] 0x1ECD978C3C0      (hkbClipGenerator*)
    [RSP+4C50] 0x70DF0FF020       (void*)
    [RSP+4C58] 0x70DF0FF030       (void*)
    [RSP+4C60] 0xC1CB55C5C4000001 (size_t)
    [RSP+4C68] 0x70DF0FE1D0       (void*)
    [RSP+4C70] 0xC2E8DF3700010000 (size_t)
    [RSP+4C78] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+4C80] 0x1ECA4CC8790      (void*)
    [RSP+4C88] 0x8000000100000000 (size_t)
    [RSP+4C90] 0x1ECA4CC8790      (void*)
    [RSP+4C98] 0x3D4CCE8000000001 (size_t)
    [RSP+4CA0] 0x3DF0FE501        (size_t)
    [RSP+4CA8] 0x70DF0FF038       (void*)
    [RSP+4CB0] 0x70DF0FEC10       (void*)
    [RSP+4CB8] 0x7FF6D6DF8108     (void* -> SkyrimSE.exe+0CA8108)
        movaps xmm1,[rbp+0F0h]
    [RSP+4CC0] 0x1ECD9358DC0      (hkbStateMachine*)
    [RSP+4CC8] 0x70DF0FEBB0       (char*) "{\xcd\x85<"
    [RSP+4CD0] 0x7FF6D7A28328     (void* -> SkyrimSE.exe+18D8328)
        test [rdx+7FF6D6h],bl
    [RSP+4CD8] 0x7FF6D6DF8980     (void* -> SkyrimSE.exe+0CA8980)
        mov rax,rsp
    [RSP+4CE0] 0xC2E8B886438E2E54 (size_t)
    [RSP+4CE8] 0x42F8B98D         (size_t)
    [RSP+4CF0] 0x0                (size_t)
    [RSP+4CF8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4D00] 0x0                (size_t)
    [RSP+4D08] 0x0                (size_t)
    [RSP+4D10] 0x0                (size_t)
    [RSP+4D18] 0x0                (size_t)
    [RSP+4D20] 0x7FFFFFFF         (size_t)
    [RSP+4D28] 0x0                (size_t)
    [RSP+4D30] 0x3C85CD7B         (size_t)
    [RSP+4D38] 0x0                (size_t)
    [RSP+4D40] 0x0                (size_t)
    [RSP+4D48] 0x70DF0FF108       (void*)
    [RSP+4D50] 0x70DF0FF020       (void*)
    [RSP+4D58] 0x70DF0FF118       (void*)
    [RSP+4D60] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+4D68] 0x70DF0FF070       (char*) "\x04"
    [RSP+4D70] 0x70DF0FE3D0       (char*) "{\xcd\x85<"
    [RSP+4D78] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+4D80] 0x0                (size_t)
    [RSP+4D88] 0x70DF0FE3D0       (char*) "{\xcd\x85<"
    [RSP+4D90] 0x70DF0FF118       (void*)
    [RSP+4D98] 0x0                (size_t)
    [RSP+4DA0] 0x70DF0FF020       (void*)
    [RSP+4DA8] 0x70DF0FF030       (void*)
    [RSP+4DB0] 0x3C000001         (size_t)
    [RSP+4DB8] 0x70DF0FE320       (void*)
    [RSP+4DC0] 0x1EC00010000      (size_t)
    [RSP+4DC8] 0x7FF6D9303E40     (void* -> SkyrimSE.exe+31B3E40)
        fdiv st,st(2)
    [RSP+4DD0] 0x1ECA4CC8710      (void*)
    [RSP+4DD8] 0x8000000200000000 (size_t)
    [RSP+4DE0] 0x1ECA4CC8710      (void*)
    [RSP+4DE8] 0x7000000002       (size_t)
    [RSP+4DF0] 0x371F45601        (size_t)
    [RSP+4DF8] 0x70DF0FF038       (void*)
    [RSP+4E00] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4E08] 0x3F7FFFFF44BC9B38 (size_t)
    [RSP+4E10] 0x1ECD89C6720      (hkbModifierGenerator*)
    [RSP+4E18] 0x0                (size_t)
    [RSP+4E20] 0x0                (size_t)
    [RSP+4E28] 0x7FF6D75B969E     (void* -> SkyrimSE.exe+146969E)
        nop
    [RSP+4E30] 0x1EE71EDE070      (BSScript::Internal::CodeTasklet*)
    [RSP+4E38] 0x70DF0FEC80       (char*) "\x06"
    [RSP+4E40] 0x0                (size_t)
    [RSP+4E48] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4E50] 0x0                (size_t)
    [RSP+4E58] 0x0                (size_t)
    [RSP+4E60] 0x0                (size_t)
    [RSP+4E68] 0x0                (size_t)
    [RSP+4E70] 0x7FFFFFFF         (size_t)
    [RSP+4E78] 0x0                (size_t)
    [RSP+4E80] 0x3C85CD7B         (size_t)
    [RSP+4E88] 0x0                (size_t)
    [RSP+4E90] 0x0                (size_t)
    [RSP+4E98] 0x70DF0FF108       (void*)
    [RSP+4EA0] 0x70DF0FF020       (void*)
    [RSP+4EA8] 0x70DF0FF118       (void*)
    [RSP+4EB0] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+4EB8] 0x70DF0FF070       (char*) "\x04"
    [RSP+4EC0] 0x70DF0FE520       (char*) "{\xcd\x85<"
    [RSP+4EC8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+4ED0] 0x0                (size_t)
    [RSP+4ED8] 0x1ECD9488780      (hkbStateMachine*)
    [RSP+4EE0] 0x70DF0FF118       (void*)
    [RSP+4EE8] 0x0                (size_t)
    [RSP+4EF0] 0x70DF0FF020       (void*)
    [RSP+4EF8] 0x70DF0FF030       (void*)
    [RSP+4F00] 0x1                (size_t)
    [RSP+4F08] 0x70DF0FE470       (void*)
    [RSP+4F10] 0x10000            (size_t)
    [RSP+4F18] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+4F20] 0x1ECA4CC8690      (void*)
    [RSP+4F28] 0x8000000100000000 (size_t)
    [RSP+4F30] 0x1ECA4CC8690      (void*)
    [RSP+4F38] 0x1                (size_t)
    [RSP+4F40] 0x3437F0001        (size_t)
    [RSP+4F48] 0x70DF0FF038       (void*)
    [RSP+4F50] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4F58] 0x7FF6D92D8768     (SkyrimScript::HandlePolicy*)
    [RSP+4F60] 0x1ECD9488780      (hkbStateMachine*)
    [RSP+4F68] 0x7FF6D6AF402E     (void* -> SkyrimSE.exe+09A402E)
        xor r13d,r13d
    [RSP+4F70] 0x42414758         (size_t)
    [RSP+4F78] 0x0                (size_t)
    [RSP+4F80] 0x42FB3F14432DF160 (size_t)
    [RSP+4F88] 0xCB94692D419364C2 (size_t)
    [RSP+4F90] 0x0                (size_t)
    [RSP+4F98] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+4FA0] 0x0                (size_t)
    [RSP+4FA8] 0x0                (size_t)
    [RSP+4FB0] 0x0                (size_t)
    [RSP+4FB8] 0x0                (size_t)
    [RSP+4FC0] 0x7FFFFFFF         (size_t)
    [RSP+4FC8] 0x0                (size_t)
    [RSP+4FD0] 0x3C85CD7B         (size_t)
    [RSP+4FD8] 0x0                (size_t)
    [RSP+4FE0] 0x0                (size_t)
    [RSP+4FE8] 0x70DF0FF108       (void*)
    [RSP+4FF0] 0x70DF0FF020       (void*)
    [RSP+4FF8] 0x70DF0FF118       (void*)
    [RSP+5000] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+5008] 0x70DF0FF070       (char*) "\x04"
    [RSP+5010] 0x70DF0FE670       (char*) "{\xcd\x85<"
    [RSP+5018] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+5020] 0x0                (size_t)
    [RSP+5028] 0x1ECD95B83C0      (hkbStateMachine*)
    [RSP+5030] 0x70DF0FF118       (void*)
    [RSP+5038] 0x0                (size_t)
    [RSP+5040] 0x70DF0FF020       (void*)
    [RSP+5048] 0x70DF0FF030       (void*)
    [RSP+5050] 0xE990FA8EE9000001 (size_t)
    [RSP+5058] 0x70DF0FE5C0       (void*)
    [RSP+5060] 0x10000            (size_t)
    [RSP+5068] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+5070] 0x1ECA4CC8610      (char*) "\x01"
    [RSP+5078] 0x8000000100000000 (size_t)
    [RSP+5080] 0x1ECA4CC8610      (char*) "\x01"
    [RSP+5088] 0x1                (size_t)
    [RSP+5090] 0x3A4CC8201        (size_t)
    [RSP+5098] 0x70DF0FF038       (void*)
    [RSP+50A0] 0x1ECD8A96970      (void*)
    [RSP+50A8] 0x1ECD8A96820      (void*)
    [RSP+50B0] 0x1ECD95B83C0      (hkbStateMachine*)
    [RSP+50B8] 0x0                (size_t)
    [RSP+50C0] 0x3C85CD7B         (size_t)
    [RSP+50C8] 0x0                (size_t)
    [RSP+50D0] 0x3D4CCCCD         (size_t)
    [RSP+50D8] 0x0                (size_t)
    [RSP+50E0] 0x0                (size_t)
    [RSP+50E8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+50F0] 0x0                (size_t)
    [RSP+50F8] 0x0                (size_t)
    [RSP+5100] 0x0                (size_t)
    [RSP+5108] 0x0                (size_t)
    [RSP+5110] 0x7FFFFFFF         (size_t)
    [RSP+5118] 0x0                (size_t)
    [RSP+5120] 0x3C85CD7B         (size_t)
    [RSP+5128] 0x0                (size_t)
    [RSP+5130] 0x0                (size_t)
    [RSP+5138] 0x70DF0FF108       (void*)
    [RSP+5140] 0x70DF0FF020       (void*)
    [RSP+5148] 0x70DF0FF118       (void*)
    [RSP+5150] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+5158] 0x70DF0FF070       (char*) "\x04"
    [RSP+5160] 0x70DF0FE7C0       (char*) "{\xcd\x85<"
    [RSP+5168] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+5170] 0x0                (size_t)
    [RSP+5178] 0x1ECD86E5C80      (hkbManualSelectorGenerator*)
    [RSP+5180] 0x70DF0FF118       (void*)
    [RSP+5188] 0x0                (size_t)
    [RSP+5190] 0x70DF0FF020       (void*)
    [RSP+5198] 0x70DF0FF030       (void*)
    [RSP+51A0] 0x7FF642000001     (size_t)
    [RSP+51A8] 0x70DF0FE710       (void*)
    [RSP+51B0] 0x42FB463600000000 (size_t)
    [RSP+51B8] 0x7FF6D9303D40     (void* -> SkyrimSE.exe+31B3D40)
        push 0FFFFFFFFF6D7AAF0h
    [RSP+51C0] 0x1ECA4CC8590      (void*)
    [RSP+51C8] 0x8000000100000000 (size_t)
    [RSP+51D0] 0x1ECA4CC8590      (void*)
    [RSP+51D8] 0x1                (size_t)
    [RSP+51E0] 0x386AA1501        (size_t)
    [RSP+51E8] 0x70DF0FF038       (void*)
    [RSP+51F0] 0x20               (size_t)
    [RSP+51F8] 0x3F               (size_t)
    [RSP+5200] 0x1ECD86E5C80      (hkbManualSelectorGenerator*)
    [RSP+5208] 0x0                (size_t)
    [RSP+5210] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5218] 0x7FF6D6DB66D3     (void* -> SkyrimSE.exe+0C666D3)
        mov r8,rax
    [RSP+5220] 0x1EE9ECA5C00      (BSTriShape*)
    [RSP+5228] 0x7FF6D6E8FFE3     (void* -> SkyrimSE.exe+0D3FFE3)
        cmp byte ptr [rbx+11Dh],0
    [RSP+5230] 0x0                (size_t)
    [RSP+5238] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5240] 0x0                (size_t)
    [RSP+5248] 0x0                (size_t)
    [RSP+5250] 0x0                (size_t)
    [RSP+5258] 0x0                (size_t)
    [RSP+5260] 0x7FFFFFFF         (size_t)
    [RSP+5268] 0x0                (size_t)
    [RSP+5270] 0x3C85CD7B         (size_t)
    [RSP+5278] 0x0                (size_t)
    [RSP+5280] 0x0                (size_t)
    [RSP+5288] 0x70DF0FF108       (void*)
    [RSP+5290] 0x70DF0FF020       (void*)
    [RSP+5298] 0x70DF0FF118       (void*)
    [RSP+52A0] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+52A8] 0x70DF0FF070       (char*) "\x04"
    [RSP+52B0] 0x70DF0FE910       (char*) "{\xcd\x85<"
    [RSP+52B8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+52C0] 0x0                (size_t)
    [RSP+52C8] 0x70DF0FE910       (char*) "{\xcd\x85<"
    [RSP+52D0] 0x70DF0FF118       (void*)
    [RSP+52D8] 0x0                (size_t)
    [RSP+52E0] 0x70DF0FF020       (void*)
    [RSP+52E8] 0x70DF0FF030       (void*)
    [RSP+52F0] 0x7000000001       (size_t)
    [RSP+52F8] 0x70DF0FE860       (void*)
    [RSP+5300] 0x10000            (size_t)
    [RSP+5308] 0x7FF6D9303E40     (void* -> SkyrimSE.exe+31B3E40)
        fdiv st,st(2)
    [RSP+5310] 0x1ECA4CC8510      (void*)
    [RSP+5318] 0x8000000200000000 (size_t)
    [RSP+5320] 0x1ECA4CC8510      (void*)
    [RSP+5328] 0x7000000002       (size_t)
    [RSP+5330] 0x3DF0FE701        (size_t)
    [RSP+5338] 0x70DF0FF038       (void*)
    [RSP+5340] 0x3A83126F         (size_t)
    [RSP+5348] 0x70DF0FE8C0       (void*)
    [RSP+5350] 0x1ECD86E4AE0      (hkbModifierGenerator*)
    [RSP+5358] 0x70DF0FE8B0       (void*)
    [RSP+5360] 0x40DBA5E3         (size_t)
    [RSP+5368] 0x3F80000000000000 (size_t)
    [RSP+5370] 0x0                (size_t)
    [RSP+5378] 0x3F80000000000000 (size_t)
    [RSP+5380] 0x0                (size_t)
    [RSP+5388] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5390] 0x0                (size_t)
    [RSP+5398] 0x0                (size_t)
    [RSP+53A0] 0x0                (size_t)
    [RSP+53A8] 0x0                (size_t)
    [RSP+53B0] 0x7FFFFFFF         (size_t)
    [RSP+53B8] 0x0                (size_t)
    [RSP+53C0] 0x3C85CD7B         (size_t)
    [RSP+53C8] 0x0                (size_t)
    [RSP+53D0] 0x0                (size_t)
    [RSP+53D8] 0x70DF0FF108       (void*)
    [RSP+53E0] 0x70DF0FF020       (void*)
    [RSP+53E8] 0x70DF0FF118       (void*)
    [RSP+53F0] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+53F8] 0x70DF0FF070       (char*) "\x04"
    [RSP+5400] 0x70DF0FEA60       (char*) "{\xcd\x85<"
    [RSP+5408] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+5410] 0x0                (size_t)
    [RSP+5418] 0x1ECD8CDC000      (hkbStateMachine*)
    [RSP+5420] 0x70DF0FF118       (void*)
    [RSP+5428] 0x0                (size_t)
    [RSP+5430] 0x70DF0FF020       (void*)
    [RSP+5438] 0x70DF0FF030       (void*)
    [RSP+5440] 0x43000001         (size_t)
    [RSP+5448] 0x70DF0FE9B0       (void*)
    [RSP+5450] 0x10000            (size_t)
    [RSP+5458] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+5460] 0x1ECA4CC8490      (void*)
    [RSP+5468] 0x8000000100000000 (size_t)
    [RSP+5470] 0x1ECA4CC8490      (void*)
    [RSP+5478] 0x7000000001       (size_t)
    [RSP+5480] 0x300000001        (size_t)
    [RSP+5488] 0x70DF0FF038       (void*)
    [RSP+5490] 0xC                (size_t)
    [RSP+5498] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+54A0] 0x1ECD8CDC000      (hkbStateMachine*)
    [RSP+54A8] 0x1EE000003E7      (void*)
    [RSP+54B0] 0x80000002         (size_t)
    [RSP+54B8] 0x0                (size_t)
    [RSP+54C0] 0x1EC86AA3848      (void*)
    [RSP+54C8] 0x7FF6D7572FB9     (void* -> SkyrimSE.exe+1422FB9)
        mfence
    [RSP+54D0] 0x0                (size_t)
    [RSP+54D8] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+54E0] 0x0                (size_t)
    [RSP+54E8] 0x0                (size_t)
    [RSP+54F0] 0x0                (size_t)
    [RSP+54F8] 0x0                (size_t)
    [RSP+5500] 0x7FFFFFFF         (size_t)
    [RSP+5508] 0x0                (size_t)
    [RSP+5510] 0x3C85CD7B         (size_t)
    [RSP+5518] 0x0                (size_t)
    [RSP+5520] 0x0                (size_t)
    [RSP+5528] 0x70DF0FF108       (void*)
    [RSP+5530] 0x70DF0FF020       (void*)
    [RSP+5538] 0x70DF0FF118       (void*)
    [RSP+5540] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+5548] 0x70DF0FF070       (char*) "\x04"
    [RSP+5550] 0x70DF0FEBB0       (char*) "{\xcd\x85<"
    [RSP+5558] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+5560] 0x0                (size_t)
    [RSP+5568] 0x1ECD93748C0      (hkbStateMachine*)
    [RSP+5570] 0x70DF0FF118       (void*)
    [RSP+5578] 0x0                (size_t)
    [RSP+5580] 0x70DF0FF020       (void*)
    [RSP+5588] 0x70DF0FF030       (void*)
    [RSP+5590] 0xFFFFFFFFFF000001 (size_t)
    [RSP+5598] 0x70DF0FEB00       (void*)
    [RSP+55A0] 0x10000            (size_t)
    [RSP+55A8] 0x7FF6D9307010     (void* -> SkyrimSE.exe+31B7010)
        pop rax
    [RSP+55B0] 0x1ECA4CC8410      (void*)
    [RSP+55B8] 0x8000000100000000 (size_t)
    [RSP+55C0] 0x1ECA4CC8410      (void*)
    [RSP+55C8] 0x7FF600000001     (size_t)
    [RSP+55D0] 0x3D92D8601        (size_t)
    [RSP+55D8] 0x70DF0FF038       (void*)
    [RSP+55E0] 0x0                (size_t)
    [RSP+55E8] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+55F0] 0x1ECD93748C0      (hkbStateMachine*)
    [RSP+55F8] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+5600] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5608] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+5610] 0x1EE9C48ACA0      (char*) "\x02"
    [RSP+5618] 0x7FF6D75825E4     (void* -> SkyrimSE.exe+14325E4)
        dec esi
    [RSP+5620] 0x0                (size_t)
    [RSP+5628] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5630] 0x0                (size_t)
    [RSP+5638] 0x0                (size_t)
    [RSP+5640] 0x0                (size_t)
    [RSP+5648] 0x0                (size_t)
    [RSP+5650] 0x7FFFFFFF         (size_t)
    [RSP+5658] 0x0                (size_t)
    [RSP+5660] 0x3C85CD7B         (size_t)
    [RSP+5668] 0x0                (size_t)
    [RSP+5670] 0x0                (size_t)
    [RSP+5678] 0x70DF0FF108       (void*)
    [RSP+5680] 0x70DF0FF020       (void*)
    [RSP+5688] 0x70DF0FF118       (void*)
    [RSP+5690] 0x1ECD89F0500      (hkbBehaviorGraph*)
    [RSP+5698] 0x70DF0FF070       (char*) "\x04"
    [RSP+56A0] 0x70DF0FED00       (void*)
    [RSP+56A8] 0x7FF6D6D79F1D     (void* -> SkyrimSE.exe+0C29F1D)
        mov rcx,rax
    [RSP+56B0] 0x0                (size_t)
    [RSP+56B8] 0x70DF0FED00       (void*)
    [RSP+56C0] 0x70DF0FF118       (void*)
    [RSP+56C8] 0x0                (size_t)
    [RSP+56D0] 0x70DF0FF020       (void*)
    [RSP+56D8] 0x70DF0FF030       (void*)
    [RSP+56E0] 0x1                (size_t)
    [RSP+56E8] 0x70DF0FEC50       (void*)
    [RSP+56F0] 0x10000            (size_t)
    [RSP+56F8] 0x7FF6D9303E40     (void* -> SkyrimSE.exe+31B3E40)
        fdiv st,st(2)
    [RSP+5700] 0x1ECA4CC8390      (void*)
    [RSP+5708] 0x8000000200000000 (size_t)
    [RSP+5710] 0x3C85CD7B         (size_t)
    [RSP+5718] 0x0                (size_t)
    [RSP+5720] 0x70DF0FF190       (void*)
    [RSP+5728] 0x7FF6D6BD5C5D     (void* -> SkyrimSE.exe+0A85C5D)
        mov rax,[rbx+28h]
    [RSP+5730] 0x300000006        (size_t)
    [RSP+5738] 0x7FFC00000000     (size_t)
    [RSP+5740] 0x1ECD89C7EC0      (hkbModifierGenerator*)
    [RSP+5748] 0x0                (size_t)
    [RSP+5750] 0x0                (size_t)
    [RSP+5758] 0x0                (size_t)
    [RSP+5760] 0x0                (size_t)
    [RSP+5768] 0x0                (size_t)
    [RSP+5770] 0x0                (size_t)
    [RSP+5778] 0x0                (size_t)
    [RSP+5780] 0x3C8EFA35         (size_t)
    [RSP+5788] 0x0                (size_t)
    [RSP+5790] 0x0                (size_t)
    [RSP+5798] 0x0                (size_t)
    [RSP+57A0] 0x3C85CD7B         (size_t)
    [RSP+57A8] 0x0                (size_t)
    [RSP+57B0] 0xBD743E303F7F82F6 (size_t)
    [RSP+57B8] 0x3CACC7C13C832DAE (size_t)
    [RSP+57C0] 0x1ECD900B100      (BSLookAtModifier*)
    [RSP+57C8] 0x7FF6D6CF31F8     (void* -> SkyrimSE.exe+0BA31F8)
        movaps xmm9,xmm0
    [RSP+57D0] 0x70DF0FEF10       (void*)
    [RSP+57D8] 0x0                (size_t)
    [RSP+57E0] 0x63               (size_t)
    [RSP+57E8] 0x0                (size_t)
    [RSP+57F0] 0x3F7F82F73C832DAE (size_t)
    [RSP+57F8] 0x3CAC66A4BD743E30 (size_t)
    [RSP+5800] 0xB98024373D00EB6F (size_t)
    [RSP+5808] 0x3F7FD804BC77FDAA (size_t)
    [RSP+5810] 0xBBE54F763F66B3F7 (size_t)
    [RSP+5818] 0xBEDDE41C         (size_t)
    [RSP+5820] 0x0                (size_t)
    [RSP+5828] 0x0                (size_t)
    [RSP+5830] 0x0                (size_t)
    [RSP+5838] 0x0                (size_t)
    [RSP+5840] 0x0                (size_t)
    [RSP+5848] 0x0                (size_t)
    [RSP+5850] 0x0                (size_t)
    [RSP+5858] 0x0                (size_t)
    [RSP+5860] 0x3C85CD7B         (size_t)
    [RSP+5868] 0x0                (size_t)
    [RSP+5870] 0x3C85CD7B         (size_t)
    [RSP+5878] 0x0                (size_t)
    [RSP+5880] 0x70DF0FF190       (void*)
    [RSP+5888] 0x7FF6D6BD4D1E     (void* -> SkyrimSE.exe+0A84D1E)
        lea rax,[rbx+8]
    [RSP+5890] 0x70DF0FEF10       (void*)
    [RSP+5898] 0x1                (size_t)
    [RSP+58A0] 0x1ECD9DC18C0      (void*)
    [RSP+58A8] 0x63               (size_t)
    [RSP+58B0] 0x40               (size_t)
    [RSP+58B8] 0x7FF6D6CF2B2F     (void* -> SkyrimSE.exe+0BA2B2F)
        mov r15,[rsp+320h]
    [RSP+58C0] 0x0                (size_t)
    [RSP+58C8] 0x3F7FFFFF         (size_t)
    [RSP+58D0] 0x0                (size_t)
    [RSP+58D8] 0x0                (size_t)
    [RSP+58E0] 0x70DF0FEEA0       (void*)
    [RSP+58E8] 0x703F9C61AA       (size_t)
    [RSP+58F0] 0x1E8D07D01        (size_t)
    [RSP+58F8] 0x1ECED6B0000      (void*)
    [RSP+5900] 0x1EDB01B4F88      (char*) "1HMShieldPowerBash"
    [RSP+5908] 0x5F               (size_t)
    [RSP+5910] 0xB2               (size_t)
    [RSP+5918] 0x1300             (size_t)
    [RSP+5920] 0x0                (size_t)
    [RSP+5928] 0x7FF6D6D83682     (void* -> SkyrimSE.exe+0C33682)
        mov eax,[rbp+90h]
    [RSP+5930] 0xC5FDF594469B041D (size_t)
    [RSP+5938] 0x460900D1         (size_t)
    [RSP+5940] 0x70               (size_t)
    [RSP+5948] 0x70DF0FF0D0       (void*)
    [RSP+5950] 0x1ECA4CDA3D0      (char*) "\x0c"
    [RSP+5958] 0x70DF0FEEC0       (void*)
    [RSP+5960] 0x0                (size_t)
    [RSP+5968] 0x0                (size_t)
    [RSP+5970] 0x40BEEEF040BDDDDF (size_t)
    [RSP+5978] 0x0                (size_t)
    [RSP+5980] 0x40000001         (size_t)
    [RSP+5988] 0x7FF6D7070161     (void* -> SkyrimSE.exe+0F20161)
        movaps xmm0,[rsi+100h]
    [RSP+5990] 0x0                (size_t)
    [RSP+5998] 0x0                (size_t)
    [RSP+59A0] 0x0                (size_t)
    [RSP+59A8] 0x0                (size_t)
    [RSP+59B0] 0x3F8000003F800000 (size_t)
    [RSP+59B8] 0x7FFCCB28F8B1     (void* -> ucrtbase.dll+002F8B1)
        jmp 0FFFFFFFFFFFFFF5Ah
    [RSP+59C0] 0x1FBF             (size_t)
    [RSP+59C8] 0x7FF6D6D06C42     (void* -> SkyrimSE.exe+0BB6C42)
        test rax,rax
    [RSP+59D0] 0x0                (size_t)
    [RSP+59D8] 0x3F80000000000000 (size_t)
    [RSP+59E0] 0x0                (size_t)
    [RSP+59E8] 0x0                (size_t)
    [RSP+59F0] 0x0                (size_t)
    [RSP+59F8] 0x7FF6D669E17E     (void* -> SkyrimSE.exe+054E17E)
        test al,al
    [RSP+5A00] 0x63               (size_t)
    [RSP+5A08] 0x1ECA4CDB530      (void*)
    [RSP+5A10] 0x0                (size_t)
    [RSP+5A18] 0x0                (size_t)
    [RSP+5A20] 0x1EF42E91F00      (BSAnimationGraphManager*)
    [RSP+5A28] 0x7FF6D67F527B     (void* -> SkyrimSE.exe+06A527B)
        cmp [rbx],eax
    [RSP+5A30] 0x80000000         (size_t)
    [RSP+5A38] 0x0                (size_t)
    [RSP+5A40] 0x0                (size_t)
    [RSP+5A48] 0x70DF0FF1A0       (char*) "\x01\x12"
    [RSP+5A50] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5A58] 0x7FF6D67C5171     (void* -> SkyrimSE.exe+0675171)
        test al,al
    [RSP+5A60] 0x70DF0FF348       (void*)
    [RSP+5A68] 0x1EE718C7200      (bhkCharRigidBodyController*)
    [RSP+5A70] 0x1ED0E239C00      (Character*)
    [RSP+5A78] 0x70DF0FF0E0       (void*)
    [RSP+5A80] 0x1ED0E239CD0      (Character*)
    [RSP+5A88] 0x7FF6D67EF22D     (void* -> SkyrimSE.exe+069F22D)
        test al,al
    [RSP+5A90] 0x1ED0000003A      (void*)
    [RSP+5A98] 0x70DF0FF0E0       (void*)
    [RSP+5AA0] 0x1EF42E91F00      (BSAnimationGraphManager*)
    [RSP+5AA8] 0x1EF42E91FA0      (void*)
    [RSP+5AB0] 0x3F0C171EBF56448F (size_t)
    [RSP+5AB8] 0xBF0C171E00000000 (size_t)
    [RSP+5AC0] 0xBF56448F         (size_t)
    [RSP+5AC8] 0x0                (size_t)
    [RSP+5AD0] 0x1EC3F800000      (size_t)
    [RSP+5AD8] 0x8000000080000000 (size_t)
    [RSP+5AE0] 0x1EC80000000      (char*) "\x01"
    [RSP+5AE8] 0x7FF6D6C23D00     (void* -> SkyrimSE.exe+0AD3D00)
        cmovno eax,[rbx+483BF0E0h]
    [RSP+5AF0] 0x0                (size_t)
    [RSP+5AF8] 0x0                (size_t)
    [RSP+5B00] 0x1EC00000000      (size_t)
    [RSP+5B08] 0x0                (size_t)
    [RSP+5B10] 0x1ECD8C1BCC0      (hkbTwistModifier*)
    [RSP+5B18] 0x7FF6D6C22ADA     (void* -> SkyrimSE.exe+0AD2ADA)
        test ebp,ebp
    [RSP+5B20] 0x80000004         (size_t)
    [RSP+5B28] 0x7FF6D6BDA33A     (void* -> SkyrimSE.exe+0A8A33A)
        mov rbx,[rsp+40h]
    [RSP+5B30] 0x1EC00000004      (size_t)
    [RSP+5B38] 0x3BC              (size_t)
    [RSP+5B40] 0x1ECD85FF460      (void*)
    [RSP+5B48] 0x8000000400000004 (size_t)
    [RSP+5B50] 0x3C30BC9F3F7FCE5C (size_t)
    [RSP+5B58] 0x3EB0F27C3D1923AF (size_t)
    [RSP+5B60] 0x1                (size_t)
    [RSP+5B68] 0x7FF6D6C5F6B7     (void* -> SkyrimSE.exe+0B0F6B7)
        mov rax,[rbx+70h]
    [RSP+5B70] 0x1ECD8C1BCC0      (hkbTwistModifier*)
    [RSP+5B78] 0x1EC9A015DD0      (hkbVariableBindingSet*)
    [RSP+5B80] 0x0                (size_t)
    [RSP+5B88] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5B90] 0x0                (size_t)
    [RSP+5B98] 0x3EB0F27C3D1923AF (size_t)
    [RSP+5BA0] 0x3F800000         (size_t)
    [RSP+5BA8] 0x0                (size_t)
    [RSP+5BB0] 0x3F800000         (size_t)
    [RSP+5BB8] 0x0                (size_t)
    [RSP+5BC0] 0x0                (size_t)
    [RSP+5BC8] 0x0                (size_t)
    [RSP+5BD0] 0x0                (size_t)
    [RSP+5BD8] 0x0                (size_t)
    [RSP+5BE0] 0x3F800000         (size_t)
    [RSP+5BE8] 0x0                (size_t)
    [RSP+5BF0] 0x0                (size_t)
    [RSP+5BF8] 0x0                (size_t)
    [RSP+5C00] 0x0                (size_t)
    [RSP+5C08] 0x0                (size_t)
    [RSP+5C10] 0x0                (size_t)
    [RSP+5C18] 0x0                (size_t)
    [RSP+5C20] 0x70DF0FF348       (void*)
    [RSP+5C28] 0x1EF42E8A210      (void*)
    [RSP+5C30] 0x1EF42E98508      (void*)
    [RSP+5C38] 0x1EF42E98500      (void*)
    [RSP+5C40] 0x70DF0FF330       (void*)
    [RSP+5C48] 0x7FF6D6D0DC25     (void* -> SkyrimSE.exe+0BBDC25)
        cmp [rbx],eax
    [RSP+5C50] 0x1201             (size_t)
    [RSP+5C58] 0x0                (size_t)
    [RSP+5C60] 0x70DF0FF330       (void*)
    [RSP+5C68] 0x0                (size_t)
    [RSP+5C70] 0x0                (size_t)
    [RSP+5C78] 0x0                (size_t)
    [RSP+5C80] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5C88] 0x0                (size_t)
    [RSP+5C90] 0x3F8000003F800000 (size_t)
    [RSP+5C98] 0x3F8000003F800000 (size_t)
    [RSP+5CA0] 0x1ECD9304000      (ahkpWorld*)
    [RSP+5CA8] 0x0                (size_t)
    [RSP+5CB0] 0x0                (size_t)
    [RSP+5CB8] 0x1EF42E8A2C0      (hkbCharacter*)
    [RSP+5CC0] 0x1EE9C450201      (void*)
    [RSP+5CC8] 0x1EF42E8A200      (BShkbAnimationGraph*)
    [RSP+5CD0] 0x70DF0FF330       (void*)
    [RSP+5CD8] 0x7FF6D6CFF2CE     (void* -> SkyrimSE.exe+0BAF2CE)
        lea r11,[rsp+208h]
    [RSP+5CE0] 0x1EF42E8A258      (void*)
    [RSP+5CE8] 0x70DF0FF348       (void*)
    [RSP+5CF0] 0x1290             (size_t)
    [RSP+5CF8] 0x70DF0FF670       (void*)
    [RSP+5D00] 0xBF564492BF0C171F (size_t)
    [RSP+5D08] 0x3F0C171F         (size_t)
    [RSP+5D10] 0xBF564492BF0C171F (size_t)
    [RSP+5D18] 0x0                (size_t)
    [RSP+5D20] 0x3F80000000000000 (size_t)
    [RSP+5D28] 0x0                (size_t)
    [RSP+5D30] 0x3F80000000000000 (size_t)
    [RSP+5D38] 0x7000000000       (size_t)
    [RSP+5D40] 0x3E922C92         (size_t)
    [RSP+5D48] 0x3F75586100000000 (size_t)
    [RSP+5D50] 0x1EDCFF88C20      (char*) "\x01"
    [RSP+5D58] 0x7FF6D75ADC68     (void* -> SkyrimSE.exe+145DC68)
        mov edx,1
    [RSP+5D60] 0x1EDCFF88308      (BSTStaticFreeList<BSScript::Internal::FunctionMessage,1024>*)
    [RSP+5D68] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+5D70] 0x1EDCFF88C20      (char*) "\x01"
    [RSP+5D78] 0x0                (size_t)
    [RSP+5D80] 0x1                (size_t)
    [RSP+5D88] 0x7FF6D75B18AB     (void* -> SkyrimSE.exe+14618AB)
        movzx ecx,al
    [RSP+5D90] 0x1EDCFF90320      (BSTCommonLLMessageQueue<BSScript::Internal::FunctionMessage>*)
    [RSP+5D98] 0xBF564490         (size_t)
    [RSP+5DA0] 0x0                (size_t)
    [RSP+5DA8] 0x469F27553F800000 (size_t)
    [RSP+5DB0] 0x70DF0FF398       (char*) "\x01"
    [RSP+5DB8] 0x7FF6D75A19BD     (void* -> SkyrimSE.exe+14519BD)
        movzx r12d,al
    [RSP+5DC0] 0x14               (size_t)
    [RSP+5DC8] 0x1                (size_t)
    [RSP+5DD0] 0x1AD99D20498      (size_t)
    [RSP+5DD8] 0x7FF6D759E392     (void* -> SkyrimSE.exe+144E392)
        sub rsp,rax
    [RSP+5DE0] 0x1EC86AA0E40      (void*)
    [RSP+5DE8] 0x70DF0FF500       (char*) "\x03"
    [RSP+5DF0] 0x0                (size_t)
    [RSP+5DF8] 0x2617796E8E7      (size_t)
    [RSP+5E00] 0x1                (size_t)
    [RSP+5E08] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+5E10] 0x221A             (size_t)
    [RSP+5E18] 0x7FF6D759F7B3     (void* -> SkyrimSE.exe+144F7B3)
        call 0FFFFFFFFFF87AA8Dh
    [RSP+5E20] 0x1EDCFF88300      (void*)
    [RSP+5E28] 0x1EDCFF88300      (void*)
    [RSP+5E30] 0x221A             (size_t)
    [RSP+5E38] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+5E40] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5E48] 0x7FF600000001     (size_t)
    [RSP+5E50] 0x1EE9C488400      (char*) "\x03"
    [RSP+5E58] 0x1EE71E788B0      (BSScript::Internal::CodeTasklet*)
    [RSP+5E60] 0x3DC6AB57         (size_t)
    [RSP+5E68] 0x0                (size_t)
    [RSP+5E70] 0x0                (size_t)
    [RSP+5E78] 0x1                (size_t)
    [RSP+5E80] 0x5460             (size_t)
    [RSP+5E88] 0x2617796E8AC      (size_t)
    [RSP+5E90] 0x7FF6D92D8400     (SkyrimSpeechRecognition*)
    [RSP+5E98] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+5EA0] 0x70DF0FF489       (void*)
    [RSP+5EA8] 0x7FF6D7594314     (void* -> SkyrimSE.exe+1444314)
        lea r8,[rbp+67h]
    [RSP+5EB0] 0x1EDCFF88300      (void*)
    [RSP+5EB8] 0x2                (size_t)
    [RSP+5EC0] 0x1EDCFF88300      (void*)
    [RSP+5EC8] 0x0                (size_t)
    [RSP+5ED0] 0x1ECD9304000      (ahkpWorld*)
    [RSP+5ED8] 0x1EE9C450201      (void*)
    [RSP+5EE0] 0x1290             (size_t)
    [RSP+5EE8] 0x1EF42E8A200      (BShkbAnimationGraph*)
    [RSP+5EF0] 0x70DF0FF550       (void*)
    [RSP+5EF8] 0x1EDCFF91484      (void*)
    [RSP+5F00] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+5F08] 0x70BF564492       (size_t)
    [RSP+5F10] 0x7000000000       (size_t)
    [RSP+5F18] 0xBF564492         (size_t)
    [RSP+5F20] 0x0                (size_t)
    [RSP+5F28] 0x0                (size_t)
    [RSP+5F30] 0x3F666666         (size_t)
    [RSP+5F38] 0x0                (size_t)
    [RSP+5F40] 0x400A3D71         (size_t)
    [RSP+5F48] 0x0                (size_t)
    [RSP+5F50] 0x1ECD9304000      (ahkpWorld*)
    [RSP+5F58] 0x0                (size_t)
    [RSP+5F60] 0x1E00             (size_t)
    [RSP+5F68] 0x5460             (size_t)
    [RSP+5F70] 0x2617796E8AC      (size_t)
    [RSP+5F78] 0x7FF6D92D8440     (SkyrimVM*)
    [RSP+5F80] 0xA                (size_t)
    [RSP+5F88] 0x1EE71C93580      (char*) "\x01"
    [RSP+5F90] 0x70DF0FF5F0       (void*)
    [RSP+5F98] 0x7FF6D6B109E7     (void* -> SkyrimSE.exe+09C09E7)
        test r15b,r15b
    [RSP+5FA0] 0x26100000000      (size_t)
    [RSP+5FA8] 0xD                (size_t)
    [RSP+5FB0] 0x7000000003       (size_t)
    [RSP+5FB8] 0x0                (size_t)
    [RSP+5FC0] 0x0                (size_t)
    [RSP+5FC8] 0x0                (size_t)
    [RSP+5FD0] 0x1EE71C93580      (char*) "\x01"
    [RSP+5FD8] 0xCFDC3000050CD    (size_t)
    [RSP+5FE0] 0x1EDCFF88100      (BSScript::Internal::VirtualMachine*)
    [RSP+5FE8] 0x0                (size_t)
    [RSP+5FF0] 0x2                (size_t)
    [RSP+5FF8] 0x0                (size_t)
    [RSP+6000] 0x0                (size_t)
    [RSP+6008] 0x7FF6D92D8B54     (void* -> SkyrimSE.exe+3188B54)
        add [rax],al
    [RSP+6010] 0x3C85CD7B         (size_t)
    [RSP+6018] 0x7FF6D92D8B54     (void* -> SkyrimSE.exe+3188B54)
        add [rax],al
    [RSP+6020] 0x3C85CD7B         (size_t)
    [RSP+6028] 0x88               (size_t)
    [RSP+6030] 0x1E00000038C9     (size_t)
    [RSP+6038] 0x2617796E8AC      (size_t)
    [RSP+6040] 0x5460             (size_t)
    [RSP+6048] 0x1EF42E91F50      (char*) "\x01"
    [RSP+6050] 0x0                (size_t)
    [RSP+6058] 0x43B808E842A03333 (size_t)
    [RSP+6060] 0x0                (size_t)
    [RSP+6068] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+6070] 0x7FF6D92D8AC4     (void* -> SkyrimSE.exe+3188AC4)
        add [rax],al
    [RSP+6078] 0x7FF6D92D8B30     (void* -> SkyrimSE.exe+3188B30)
        add [rax],al
    [RSP+6080] 0x0                (size_t)
    [RSP+6088] 0x43B808E842A02E00 (size_t)
    [RSP+6090] 0x1ED0E239C00      (Character*)
    [RSP+6098] 0x1EC86AA0E40      (void*)
    [RSP+60A0] 0x0                (size_t)
    [RSP+60A8] 0x70DF0FF788       (void*)
    [RSP+60B0] 0x1EF42E8A200      (BShkbAnimationGraph*)
    [RSP+60B8] 0x70DF0FF868       (void*)
    [RSP+60C0] 0x7FF6D67EF770     (void* -> SkyrimSE.exe+069F770)
        jmp 0000000000002F20h
    [RSP+60C8] 0x7FF6D6D028C4     (void* -> SkyrimSE.exe+0BB28C4)
        cmp byte ptr [rsi+2Eh],0
    [RSP+60D0] 0x3A               (size_t)
    [RSP+60D8] 0x7FF6D6E190CF     (void* -> SkyrimSE.exe+0CC90CF)
        cmp [rdi],eax
    [RSP+60E0] 0x3A               (size_t)
    [RSP+60E8] 0x70DF0FF868       (void*)
    [RSP+60F0] 0x0                (size_t)
    [RSP+60F8] 0x7FFC135B071A     (void* -> Precision.dll+00E071A)
        add rsp,98h
    [RSP+6100] 0x1EE9EC33D28      (MovementAgentPathFollowerStandard*)
    [RSP+6108] 0x7FF6D73022B6     (void* -> SkyrimSE.exe+11B22B6)
        nop
    [RSP+6110] 0x1EE9EC33E10      (void*)
    [RSP+6118] 0x7FF6D6E190CF     (void* -> SkyrimSE.exe+0CC90CF)
        cmp [rdi],eax
    [RSP+6120] 0x1EF42E8A2C0      (hkbCharacter*)
    [RSP+6128] 0x0                (size_t)
    [RSP+6130] 0x0                (size_t)
    [RSP+6138] 0x7FFC9C679251     (void* -> tbbmalloc.dll+0019251 scalable_aligned_free)
        xor ecx,ecx
    [RSP+6140] 0x1EE9EC33D28      (MovementAgentPathFollowerStandard*)
    [RSP+6148] 0x7FF6D730269E     (void* -> SkyrimSE.exe+11B269E)
        nop
    [RSP+6150] 0x1EE9EC33E10      (void*)
    [RSP+6158] 0x1ECD9304000      (ahkpWorld*)
    [RSP+6160] 0x43200000         (size_t)
    [RSP+6168] 0x0                (size_t)
    [RSP+6170] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+6178] 0x1ED0E239C00      (Character*)
    [RSP+6180] 0x1EE9EC33D28      (MovementAgentPathFollowerStandard*)
    [RSP+6188] 0x7FF6D67E48A5     (void* -> SkyrimSE.exe+06948A5)
        test al,al
    [RSP+6190] 0x1EE9EC33E10      (void*)
    [RSP+6198] 0x1ED0E239C00      (Character*)
    [RSP+61A0] 0x70DF0FF798       (void*)
    [RSP+61A8] 0x0                (size_t)
    [RSP+61B0] 0x70DF0FF7B8       (void*)
    [RSP+61B8] 0x7FF6D6E1707A     (void* -> SkyrimSE.exe+0CC707A)
        xor eax,eax
    [RSP+61C0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+61C8] 0x0                (size_t)
    [RSP+61D0] 0x44000000         (size_t)
    [RSP+61D8] 0x0                (size_t)
    [RSP+61E0] 0x1ED0E239C00      (Character*)
    [RSP+61E8] 0x7FF6D656D475     (void* -> SkyrimSE.exe+041D475)
        nop
    [RSP+61F0] 0x0                (size_t)
    [RSP+61F8] 0x1EE2FC11800      (BSFaceGenAnimationData*)
    [RSP+6200] 0x0                (size_t)
    [RSP+6208] 0x7FF6D67F1B51     (void* -> SkyrimSE.exe+06A1B51)
        nop
    [RSP+6210] 0x0                (size_t)
    [RSP+6218] 0x70DF0FF819       (void*)
    [RSP+6220] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+6228] 0x1ED0E239C00      (Character*)
    [RSP+6230] 0x7FF6D93A80C4     (void* -> SkyrimSE.exe+32580C4)
        add [rax],al
    [RSP+6238] 0xFFFFFFFC         (size_t)
    [RSP+6240] 0x1ED0E239C00      (Character*)
    [RSP+6248] 0x0                (size_t)
    [RSP+6250] 0x1EE2FC11800      (BSFaceGenAnimationData*)
    [RSP+6258] 0x7FF6D656D5A7     (void* -> SkyrimSE.exe+041D5A7)
        add rsp,78h
    [RSP+6260] 0x2                (size_t)
    [RSP+6268] 0x0                (size_t)
    [RSP+6270] 0x1EC86AA0E40      (void*)
    [RSP+6278] 0x7FF6D6826EDE     (void* -> SkyrimSE.exe+06D6EDE)
        test rax,rax
    [RSP+6280] 0x0                (size_t)
    [RSP+6288] 0x0                (size_t)
    [RSP+6290] 0x0                (size_t)
    [RSP+6298] 0x0                (size_t)
    [RSP+62A0] 0x0                (size_t)
    [RSP+62A8] 0x0                (size_t)
    [RSP+62B0] 0x0                (size_t)
    [RSP+62B8] 0x0                (size_t)
    [RSP+62C0] 0x0                (size_t)
    [RSP+62C8] 0x0                (size_t)
    [RSP+62D0] 0x1ED0E239C00      (Character*)
    [RSP+62D8] 0x7FF6D67F1E30     (void* -> SkyrimSE.exe+06A1E30)
        jmp short 0FFFFFFFFFFFFFFC0h
    [RSP+62E0] 0x3C85CD7B         (size_t)
    [RSP+62E8] 0x0                (size_t)
    [RSP+62F0] 0x7FF6D93A80C4     (void* -> SkyrimSE.exe+32580C4)
        add [rax],al
    [RSP+62F8] 0xFFFFFFFC         (size_t)
    [RSP+6300] 0x7FF6D93A80C0     (void* -> SkyrimSE.exe+32580C0)
        add [rax],al
    [RSP+6308] 0x7FF6D93A80C8     (void* -> SkyrimSE.exe+32580C8)
        add [rax],al
    [RSP+6310] 0x3C85CD7B         (size_t)
    [RSP+6318] 0x0                (size_t)
    [RSP+6320] 0x1EDB0359D01      (void*)
    [RSP+6328] 0x7FF6D67BAF75     (void* -> SkyrimSE.exe+066AF75)
        mov rcx,rbx
    [RSP+6330] 0x1EC00000032      (size_t)
    [RSP+6338] 0x1ED0E239C00      (Character*)
    [RSP+6340] 0x1                (size_t)
    [RSP+6348] 0x0                (size_t)
    [RSP+6350] 0x3C85CD7B         (size_t)
    [RSP+6358] 0x0                (size_t)
    [RSP+6360] 0x1EDB0359DE0      (void*)
    [RSP+6368] 0x7FF6D68C6B23     (void* -> SkyrimSE.exe+0776B23)
        nop
    [RSP+6370] 0x1ED0E239C00      (Character*)
    [RSP+6378] 0x1ED0E239C00      (Character*)
    [RSP+6380] 0x1ED0E239C00      (Character*)
    [RSP+6388] 0x0                (size_t)
    [RSP+6390] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+6398] 0x7FFCCB70081D     (char*) "\x0f\x1fD"
    [RSP+63A0] 0x0                (size_t)
    [RSP+63A8] 0x0                (size_t)
    [RSP+63B0] 0x0                (size_t)
    [RSP+63B8] 0x0                (size_t)
    [RSP+63C0] 0x7FF6D93AB5B8     (void* -> SkyrimSE.exe+325B5B8)
        add [rax],al
    [RSP+63C8] 0x7FF6D6E478D1     (void* -> SkyrimSE.exe+0CF78D1)
        mov eax,[rdi+0C8h]
    [RSP+63D0] 0x112DC7           (size_t)
    [RSP+63D8] 0x1ED0E239C00      (Character*)
    [RSP+63E0] 0x1ED10DA2B00      (TESObjectCELL*)
    [RSP+63E8] 0x7FFCCB70081D     (char*) "\x0f\x1fD"
    [RSP+63F0] 0x7FF6D93A80C4     (void* -> SkyrimSE.exe+32580C4)
        add [rax],al
    [RSP+63F8] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+6400] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+6408] 0x1EDB0359DE0      (void*)
    [RSP+6410] 0x7FF6D93BEF00     (void* -> SkyrimSE.exe+326EF00)
        push rsp
    [RSP+6418] 0x7FF6D6E4813E     (void* -> SkyrimSE.exe+0CF813E)
        mov r11d,[r14+0A6Ch]
    [RSP+6420] 0x0                (size_t)
    [RSP+6428] 0x0                (size_t)
    [RSP+6430] 0x1EDB0359DE0      (void*)
    [RSP+6438] 0x7000005DD5       (size_t)
    [RSP+6440] 0x1EDB0359DE0      (void*)
    [RSP+6448] 0x0                (size_t)
    [RSP+6450] 0x1EC86AA15A8      (char*) "\x14"
    [RSP+6458] 0x1EDB0359DF8      (void*)
    [RSP+6460] 0x1EDB0359DE0      (void*)
    [RSP+6468] 0x0                (size_t)
    [RSP+6470] 0x0                (size_t)
    [RSP+6478] 0x7FF6D6E47668     (void* -> SkyrimSE.exe+0CF7668)
        jmp short 0000000000000017h
    [RSP+6480] 0x0                (size_t)
    [RSP+6488] 0x7FFCCB71092B     (char*) "\x0f\x1fD"
    [RSP+6490] 0x0                (size_t)
    [RSP+6498] 0x2                (size_t)
    [RSP+64A0] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+64A8] 0x7FF6D93A80C4     (void* -> SkyrimSE.exe+32580C4)
        add [rax],al
    [RSP+64B0] 0x0                (size_t)
    [RSP+64B8] 0x0                (size_t)
    [RSP+64C0] 0x0                (size_t)
    [RSP+64C8] 0x0                (size_t)
    [RSP+64D0] 0x0                (size_t)
    [RSP+64D8] 0x7FF6D93A80C4     (void* -> SkyrimSE.exe+32580C4)
        add [rax],al
    [RSP+64E0] 0x1                (size_t)
    [RSP+64E8] 0x7FF6D93A80C0     (void* -> SkyrimSE.exe+32580C0)
        add [rax],al
    [RSP+64F0] 0x7FF6D93A80C8     (void* -> SkyrimSE.exe+32580C8)
        add [rax],al
    [RSP+64F8] 0x1EDB035A5C0      (void*)
    [RSP+6500] 0x0                (size_t)
    [RSP+6508] 0x7FF6D93AB5D8     (void* -> SkyrimSE.exe+325B5D8)
        shl byte ptr [rbp+1EDB035h],0
    [RSP+6510] 0x0                (size_t)
    [RSP+6518] 0x7FF6D6822CF3     (void* -> SkyrimSE.exe+06D2CF3)
        xor ebx,ebx
    [RSP+6520] 0x1ED00000088      (void*)
    [RSP+6528] 0x0                (size_t)
    [RSP+6530] 0x7FF600004F22     (size_t)
    [RSP+6538] 0x6B2A9            (size_t)
    [RSP+6540] 0xFFFFFFFFFFFFFFFE (size_t)
    [RSP+6548] 0x0                (size_t)
    [RSP+6550] 0x1EDB035A5C0      (void*)
    [RSP+6558] 0x7FF6D6E47888     (void* -> SkyrimSE.exe+0CF7888)
        mov ecx,[rbx+0Ch]
    [RSP+6560] 0x7FF6D93AB5D8     (void* -> SkyrimSE.exe+325B5D8)
        shl byte ptr [rbp+1EDB035h],0
    [RSP+6568] 0x7FF6D93AB5D8     (void* -> SkyrimSE.exe+325B5D8)
        shl byte ptr [rbp+1EDB035h],0
    [RSP+6570] 0x0                (size_t)
    [RSP+6578] 0x7FFCCB7162BB     (char*) "\x0f\x1fD"
    [RSP+6580] 0x11               (size_t)
    [RSP+6588] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+6590] 0x7FF6D93AB588     (void* -> SkyrimSE.exe+325B588)
        add [rax],al
    [RSP+6598] 0x1EDB035A5C0      (void*)
    [RSP+65A0] 0x0                (size_t)
    [RSP+65A8] 0x7FF6D6E47E51     (void* -> SkyrimSE.exe+0CF7E51)
        mov r15d,eax
    [RSP+65B0] 0x1                (size_t)
    [RSP+65B8] 0x1                (size_t)
    [RSP+65C0] 0x0                (size_t)
    [RSP+65C8] 0x7FFC244564B9     (void* -> EngineFixes.dll+00164B9)
        cmp dword ptr [0C597Fh],0FFFFFFFFh
    [RSP+65D0] 0x1EDB035A5C0      (void*)
    [RSP+65D8] 0x1                (size_t)
    [RSP+65E0] 0x9ED35D983DD4     (size_t)
    [RSP+65E8] 0x0                (size_t)
    [RSP+65F0] 0x1EDB035A5C0      (void*)
    [RSP+65F8] 0x30000000F        (size_t)
    [RSP+6600] 0x7FF600005DD5     (size_t)
    [RSP+6608] 0x1EDB035A5C0      (void*)
    [RSP+6610] 0x30000000F        (size_t)
    [RSP+6618] 0x7FF600005DD5     (size_t)
    [RSP+6620] 0x500000005        (size_t)
    [RSP+6628] 0x0                (size_t)
    [RSP+6630] 0x0                (size_t)
    [RSP+6638] 0x0                (size_t)
    [RSP+6640] 0x0                (size_t)
    [RSP+6648] 0x0                (size_t)
    [RSP+6650] 0x0                (size_t)
    [RSP+6658] 0x0                (size_t)
    [RSP+6660] 0x0                (size_t)
    [RSP+6668] 0x0                (size_t)
    [RSP+6670] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+6678] 0x7FF6D6E461DA     (void* -> SkyrimSE.exe+0CF61DA)
        movzx eax,byte ptr [rbx+0A74h]
    [RSP+6680] 0x7FF6D93AB501     (void* -> SkyrimSE.exe+325B501)
        add [rax],al
    [RSP+6688] 0x0                (size_t)
    [RSP+6690] 0x1                (size_t)
    [RSP+6698] 0x11               (size_t)
    [RSP+66A0] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+66A8] 0x7FF6D6E20DBD     (void* -> SkyrimSE.exe+0CD0DBD)
        mov rcx,[24FB55Bh]
    [RSP+66B0] 0x7FF6D931C370     (void* -> SkyrimSE.exe+31CC370)
        add [rax],al
    [RSP+66B8] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+66C0] 0x0                (size_t)
    [RSP+66C8] 0x0                (size_t)
    [RSP+66D0] 0x7FF6D93AB568     (BSJobs::JobThread*)
    [RSP+66D8] 0x0                (size_t)
    [RSP+66E0] 0x0                (size_t)
    [RSP+66E8] 0x7FFCCCA0E8D7     (void* -> KERNEL32.DLL+002E8D7 BaseThreadInitThunk)
        mov ecx,eax
    [RSP+66F0] 0x0                (size_t)
    [RSP+66F8] 0x0                (size_t)
    [RSP+6700] 0x0                (size_t)
    [RSP+6708] 0x0                (size_t)
    [RSP+6710] 0x0                (size_t)
    [RSP+6718] 0x7FFCCDF3FBCC     (void* -> ntdll.dll+00DFBCC RtlUserThreadStart)
        jmp short 000000000000002Ah
    [RSP+6720] 0x0                (size_t)
    [RSP+6728] 0x0                (size_t)
    [RSP+6730] 0x4F0FFFFFB30      (size_t)
    [RSP+6738] 0x4D0FFFFFB30      (size_t)
    [RSP+6740] 0x21               (size_t)
    [RSP+6748] 0x7FFCCB76D2E0     (void* -> KERNELBASE.dll+011D2E0 UnhandledExceptionFilter)
        mov [rsp+10h],rbx
    [RSP+6750] 0x70DF0F8680       (void*)
    [RSP+6758] 0x70DF0F8680       (void*)
    [RSP+6760] 0x0                (size_t)
    [RSP+6768] 0x0                (size_t)
    [RSP+6770] 0x0                (size_t)
    [RSP+6778] 0x0                (size_t)
    [RSP+6780] 0x0                (size_t)
    [RSP+6788] 0x0                (size_t)
    [RSP+6790] 0x0                (size_t)
    [RSP+6798] 0x0                (size_t)
    [RSP+67A0] 0x0                (size_t)
    [RSP+67A8] 0x0                (size_t)
    [RSP+67B0] 0x0                (size_t)
    [RSP+67B8] 0x0                (size_t)
    [RSP+67C0] 0x0                (size_t)
    [RSP+67C8] 0x0                (size_t)
    [RSP+67D0] 0x0                (size_t)
    [RSP+67D8] 0x0                (size_t)
    [RSP+67E0] 0x0                (size_t)
    [RSP+67E8] 0x0                (size_t)
    [RSP+67F0] 0x0                (size_t)
    [RSP+67F8] 0x0                (size_t)
    [RSP+6800] 0x0                (size_t)
    [RSP+6808] 0x0                (size_t)
    [RSP+6810] 0x0                (size_t)
    [RSP+6818] 0x0                (size_t)
    [RSP+6820] 0x0                (size_t)
    [RSP+6828] 0x0                (size_t)
    [RSP+6830] 0x0                (size_t)
    [RSP+6838] 0x0                (size_t)
    [RSP+6840] 0x0                (size_t)
    [RSP+6848] 0x0                (size_t)
    [RSP+6850] 0x0                (size_t)
    [RSP+6858] 0x0                (size_t)
    [RSP+6860] 0x0                (size_t)
    [RSP+6868] 0x0                (size_t)
    [RSP+6870] 0x0                (size_t)
    [RSP+6878] 0x0                (size_t)
    [RSP+6880] 0x0                (size_t)
    [RSP+6888] 0x0                (size_t)
    [RSP+6890] 0x0                (size_t)
    [RSP+6898] 0x0                (size_t)
    [RSP+68A0] 0x0                (size_t)
    [RSP+68A8] 0x0                (size_t)
    [RSP+68B0] 0x0                (size_t)
    [RSP+68B8] 0x0                (size_t)
    [RSP+68C0] 0x0                (size_t)
    [RSP+68C8] 0x0                (size_t)
    [RSP+68D0] 0x0                (size_t)
    [RSP+68D8] 0x0                (size_t)
    [RSP+68E0] 0x0                (size_t)
    [RSP+68E8] 0x0                (size_t)
    [RSP+68F0] 0x0                (size_t)
    [RSP+68F8] 0x0                (size_t)
    [RSP+6900] 0x0                (size_t)
    [RSP+6908] 0x0                (size_t)
    [RSP+6910] 0x0                (size_t)
    [RSP+6918] 0x0                (size_t)
    [RSP+6920] 0x0                (size_t)
    [RSP+6928] 0x0                (size_t)
    [RSP+6930] 0x0                (size_t)
    [RSP+6938] 0x0                (size_t)
    [RSP+6940] 0x0                (size_t)
    [RSP+6948] 0x0                (size_t)
    [RSP+6950] 0x0                (size_t)
    [RSP+6958] 0x0                (size_t)
    [RSP+6960] 0x0                (size_t)
    [RSP+6968] 0x0                (size_t)
    [RSP+6970] 0x0                (size_t)
    [RSP+6978] 0x0                (size_t)
    [RSP+6980] 0x0                (size_t)
    [RSP+6988] 0x0                (size_t)
    [RSP+6990] 0x0                (size_t)
    [RSP+6998] 0x0                (size_t)
    [RSP+69A0] 0x0                (size_t)
    [RSP+69A8] 0x0                (size_t)
    [RSP+69B0] 0x0                (size_t)
    [RSP+69B8] 0x0                (size_t)
    [RSP+69C0] 0x0                (size_t)
    [RSP+69C8] 0x0                (size_t)
    [RSP+69D0] 0x0                (size_t)
    [RSP+69D8] 0x0                (size_t)
    [RSP+69E0] 0x0                (size_t)
    [RSP+69E8] 0x0                (size_t)
    [RSP+69F0] 0x0                (size_t)
    [RSP+69F8] 0x0                (size_t)
    [RSP+6A00] 0x0                (size_t)
    [RSP+6A08] 0x0                (size_t)
    [RSP+6A10] 0x0                (size_t)
    [RSP+6A18] 0x0                (size_t)
    [RSP+6A20] 0x0                (size_t)
    [RSP+6A28] 0x0                (size_t)
    [RSP+6A30] 0x0                (size_t)
    [RSP+6A38] 0x0                (size_t)
    [RSP+6A40] 0x0                (size_t)
    [RSP+6A48] 0x0                (size_t)
    [RSP+6A50] 0x0                (size_t)
    [RSP+6A58] 0x0                (size_t)
    [RSP+6A60] 0x0                (size_t)
    [RSP+6A68] 0x0                (size_t)
    [RSP+6A70] 0x0                (size_t)
    [RSP+6A78] 0x0                (size_t)
    [RSP+6A80] 0x0                (size_t)
    [RSP+6A88] 0x0                (size_t)
    [RSP+6A90] 0x0                (size_t)
    [RSP+6A98] 0x0                (size_t)
    [RSP+6AA0] 0x0                (size_t)
    [RSP+6AA8] 0x0                (size_t)

MODULES:
    AchievementsModsEnabler.dll
        Address: 0x7FFCA0CE0000
        SHA: D79E3518F8791F7A61ECC76936ED346CA9D951602B611856BC8B16C6AA4F3E923B042F4EE59E9B1A0B3A848D05E33D8A071C231AA1803E45171A0C9CECEC2117
        Version: v1.4.0
    AchievementsModsEnablerLoader.dll
        Address: 0x7FFCADD90000
        SHA: DA7C8758DA9EA4709032277CCCD0D8F67BEC9381F38F29D2AF4C1AC47F10758F90567EC91EC935095FC6A2FE5FF794A9BB2D80F567089A886C78206FA5CA6D62
        Version: v1.3.0
    ADVAPI32.dll
        Address: 0x7FFCCCC80000
        SHA: 094CCDED55729BC8F1284D308FE9B7EB5F6B187E4862CDC4C6B8885C03BE9E7F11F6E2D3821D756102A96510B6B6D1D3384BB9B363B613A7D014C85209598E45
        Version: v10.0.26100.2308
    AnimationMotionRevolution.dll
        Address: 0x7FFC22530000
        SHA: 4A3A00073E3A94CA73C9F4216572DF7AE7B24ACC39112138DA70D140B404AD0069589588E7C2FF784DAACDFA1500C5DF7A0037548A6FEA3D9A8315054D71F647
    AnimationQueueFix.dll
        Address: 0x7FFC60510000
        SHA: 901F4487A29B5CAA07D98CB9AC5A611CC22A01259E0E4FFD80CDCFCA189CBD38031F6C0B51A74BE1D76C1F97FCD6A3B9F47807A38638DA0F8FC6FBDE35EFDF39
        Version: v1.0.1
    AUDIOSES.DLL
        Address: 0x7FFCB8950000
        SHA: DA2D1D49DCCCDA0560553A6428181C9224C08F3881F49303527A90CE4DFBC42D46C73248106D349BDD728B473FC7630B12925D86892B4EFF4AB2D3C6BFDA105A
        Version: v10.0.26100.2308
    avrt.dll
        Address: 0x7FFCC8D20000
        SHA: ADE6872B1BC62425EC0301755551C35083139AC56A9B8B85A8C84216FD44287A1AF65C0C1DD635CA8FF14EABADB55687D685E4976B775902DD831E445D178A2F
        Version: v10.0.26100.2308
    BackportedESLSupport.dll
        Address: 0x7FFC23860000
        SHA: 26EE6E233076212B7742AB5D7CC46370B37A94F19B5892A27FFF125F6E38DFEBC4DDD0901C71C1845686357A2DE4FAF8896B1306F6DA95ADDC97E4970B95778F
    bcrypt.dll
        Address: 0x7FFCCAAF0000
        SHA: E0D79E77027E0BDC438C500CD006C459F9164A2B2418873EF7732D3A68BD9DC5E04BFD9E0AC240CAFB03150A9E9174291CA7A5D611B38C09FB1D713380E355FD
        Version: v10.0.26100.2308
    bcryptPrimitives.dll
        Address: 0x7FFCCB470000
        SHA: 60FE720A674B364D5BAA332A9173BD05324B3C5EF2FE29F76960C733AC869667730869F1E96BA15D9150E9AF85B79E4E40C3B1C38B5363A88F4537527B6EC855
        Version: v10.0.26100.2033
    BehaviorDataInjector.dll
        Address: 0x7FFC21190000
        SHA: AFAB12C66FFA76C47EAE22B8E595EEE30A78BFA672D908834C530CD678D45605D18E36FE09ECAB2ABF8C3BE01814FF31B85EF7F823AA95A802187C209D306007
        Version: v0.1.3
    BetterJumpingSE.dll
        Address: 0x7FFC9C860000
        SHA: 28AF3364C442A0A9DC7732C4A74DC08246EA00AE7A2FB0621ED7843B48C290E804589E773C7786CBC2D3C5F8BAD800104760299D675BCB1BB7A985761FC4D3BE
    BetterThirdPersonSelection.dll
        Address: 0x7FFC20580000
        SHA: 7A3C8DCF7E51F227154E644D6E984CD648E76D0C6C4F761354CAF8216BE81F1A0DECF554647C646BE2C826D4510E8778F2A8D710574B6E85189AF1EFA0AD4099
        Version: v1.0.0
    bink2w64.dll
        Address: 0x7FFC8E850000
        SHA: 3369CC043EE6CBCA63F820E558BAC93E6B137A18C052416F18CC741BD888AF27A3AD98B83AF8BFD3C9705F7E823A9D32C17188BB4C0D797B82ACAFF123902E2C
        Version: v2.7.1.300
    BugFixesSSE.dll
        Address: 0x7FFC5D1B0000
        SHA: CA3C5D7C410D08661C6BEAD680B12628C1105F21ADE6E3583EFDE318A2EBE8BEF710B0577263BE802EFF3EA3485D7CE6E1CAAA8CE07F9D2242E1CFAD2BC20384
    CFGMGR32.dll
        Address: 0x7FFCCAEC0000
        SHA: FBE98A916A267B3C8DEFFBBA1DC4C15608EFEBBF613F00078ADA65C905EC6350904FE841F8123DD00A743662374F111DF1F75F1847184F8EDDF2158FE701D7E3
        Version: v10.0.26100.2454
    clbcatq.dll
        Address: 0x7FFCCC790000
        SHA: 1EBE6B579BB73E21ABFC7FEF215D2C55B14121D489A9D5D84288B0FB2FB7DED6D0BEAE78E248AB738395737E61DEE11976EF5AFAC506E5004E7483126FE5AD63
        Version: v2001.12.10941.16384
    combase.dll
        Address: 0x7FFCCBE10000
        SHA: AF0FD0F2B15FBD76BA1E334DCC1CFF26B45DF87B7ADCA022FC3B4D25FC11A1943749B02A7C32282F5C04C21909AA8420C3B87F0AA2913A2778D0F507D9289E7D
        Version: v10.0.26100.2308
    CombatPathingRevolution.dll
        Address: 0x7FFC1C980000
        SHA: E7F5EF9A92B789C96640CFC7B82F856E4741D4298ACF1F5C4EDEE4070EFC3F606CFE69096B9E89964230129BFBEB4F1F4F5D4B1C0B13ECB1DACBC11104059667
    ConsoleUtilSSE.dll
        Address: 0x7FFC22960000
        SHA: FF29E71FCC7061419B9B380D888D7246F682B00A6B06452E20A3ADCBEDBBF231FE3E88839CE0D765D0933178BB6A6031FE420A0D3BD33F4294A274DBFCD8BFE4
        Version: v1.4.0
    CoreMessaging.dll
        Address: 0x7FFCC6DE0000
        SHA: 22E82779D5E31ED61E49EB2D4748F6B19E6EDF0F5DE4DDE2F5855C1916E18AE66A4B31A136A10ED0B1B1C3559862A6216A24C6F1A88FFA823F34556A3C6E38DC
        Version: v10.0.26100.1882
    CoreUIComponents.dll
        Address: 0x7FFCC5580000
        SHA: F6A0E49B2DED5A911E5590BF880D778BB2B99E2A00FCE5E041B40086C15B15DF3C816FA7987E84C4F30F518FAB5231151209E4785ACC93DB9FC7ADD267FB0B81
        Version: v10.0.26100.2454
    CRYPT32.dll
        Address: 0x7FFCCBA10000
        SHA: 91FB3FA6B74CB11DDFBDA27FFFB32C010152ACFC7D5D927685987CCE34DA7C6B7CE6B1DFF14006BB95E1E4C8270490854619C7569BBAEB5CED71F2573013A1E9
        Version: v10.0.26100.2308
    CRYPTBASE.DLL
        Address: 0x7FFCCA740000
        SHA: 5C8F522617075762D11AB3A459DD58BEE0D594892168010D1DF4998B6145761F618D5B0CCCC1DF130B2D5C1E951F3B1AAE9A872FBCA1796EBDBF7FA9BF4E94B1
        Version: v10.0.26100.2894
    cryptnet.dll
        Address: 0x7FFCC4C60000
        SHA: 170B857F78D71833B66DFE8174D21FC72577B605AE8F6484DAFFC0A479774EEF135718CCCBA15FCD9CA99251D49C94C20C7C0AE46E7ECBF876C40D1DFCB9E8B2
        Version: v10.0.26100.2454
    cryptsp.dll
        Address: 0x7FFCCA850000
        SHA: D5F162272852371A795AD1EE6402F82572C3C6C048999063C97DA50DDA68CF2E2273E8C72FD63089151C09C5808974F6F830B7A0CE3834A7ACD1DAE90F9A822B
        Version: v10.0.26100.2454
    d3d11.dll
        Address: 0x000180000000
        SHA: 222DC28209A24E3BECC2F9C6785A882C430921E84EA34AC485C1EF8C1EF100C7515EFDE29B8234549EF1FAE3390A6E08FD7409DE18EB810E28D75ADCFDA10DC7
        Version: v0.5.0.3
    d3d11.dll
        Address: 0x7FFCC8990000
        SHA: CBAEEA21DB1483C79A76F6F1576F7E4DB60E7B78E2678DB6EBD1611912DDDFE7BD0CFBF15C652C6FFE39ADD356BF6716F8458D64A2A5B1725E2C92231C601FDE
        Version: v10.0.26100.2454
    D3DCOMPILER_43.dll
        Address: 0x7FFC51900000
        SHA: 1AFC63DB5D2030B76ABC19094FC9FEF28CC6250BD265294647E65DB81F13749C867722924460F7A6021C739F4057F95501F0322CDEC28A2101BF94164557A1A5
        Version: v9.29.952.3111
    d3dcompiler_46e.dll
        Address: 0x7FFC124D0000
        SHA: F1A5DCE642014B3BBDB477DA1CF4EA212F0444FEE58D3A636F0F8FC749D0B243DAD3FC980FEFF4F793B352732DB404CBA5CC5E6E7BE5E111684994189C4D533A
        Version: v9.30.9200.16384
    D3DCOMPILER_47.dll
        Address: 0x7FFCC62B0000
        SHA: 997145AAABD9F96F13581A1F1DBD3570CC549609B2AC6379CF71B68C65B351BCB1E26FF09A5B997495BA0B62413119D60BE192408F6CD3576EA014D9920BC111
        Version: v10.0.26100.2894
    d3dx11_43.dll
        Address: 0x7FFCA30C0000
        SHA: 46CBFB1E22C3F469BDC80515560448F6F83607FD6974BB68B9C7F86CA10C69878F1312B32C81C0F57B931C43BAD80BD46BDF26AB4FFB999ABB0B73DE27AD7C56
        Version: v9.29.952.3111
    d3dx9_42.dll
        Address: 0x7FFCB26E0000
        SHA: 8782AD418FEA63A2CF4DD08F87B9B2527C804C6B2AB1C4C92380A84F1BD06FF6300310163A319E0F2833F3F40A26BC5ED68763C1824071C3AAFE929A02F2E122
    dbgcore.DLL
        Address: 0x7FFCA8590000
        SHA: 389FBD7527F4A3DB3DEA4872FFC391753B4FF46220031207A43525EBEFCDB68712FE09E7FA71213CE226DCB15F54E7BC5917C9B7E28FCD6BA3A5CAA9E99A33A7
        Version: v10.0.26100.2454
    dbghelp.dll
        Address: 0x7FFCC81D0000
        SHA: C56FD83C1E7997D175CD8DADC0B6A579181299D06573E1C6644B83DDF16F8EE7A17ECC7A6DBA217E33120F86846A3DFF1C9BD021C4C122B3EE7D4F60784EC9A0
        Version: v10.0.26100.2033
    dcomp.dll
        Address: 0x7FFCC6760000
        SHA: 15A8B5A27D62BBA75137D2651ED1157CFDEF03FC99557F19A1C3DC8DFBC4EF5E061033F5AE377D4CC63F7A71FC0666652BA3A0DF61EEF287BAF180C52B4339BE
        Version: v10.0.26100.2605
    DescriptionFramework.dll
        Address: 0x7FFC20470000
        SHA: EFF1F813F7FB6225D7A41786902BC9478007118B53F81A935D107B86B961A8567CA7EBE13654C68D0469653CE6204FF0F1A2A769CAF008C6B3A2FF25490969CC
        Version: v2.1.1
    devobj.dll
        Address: 0x7FFCCAE90000
        SHA: 701FA93590C1453301873595A66E4B3BC9751F55D55220BF0E905641496977EA1ECC7654E5264B4D250646EB4B795387470F044B65C5B3123FF62BEF4A84761C
        Version: v10.0.26100.1150
    dhcpcsvc.DLL
        Address: 0x7FFCC38D0000
        SHA: DFB6F4FC0B8C866A4F083893461E9F32A5F0DCB5F4078CD3540DF354E7EBEB101E47C96B20B1D183781B5454B50905AF385E57791652F75EB80C58E85509F791
        Version: v10.0.26100.2308
    DINPUT8.dll
        Address: 0x7FFC85CE0000
        SHA: E864B7590C5D94ADBB0315E7E8E58FBFF0C5E79626015EF525299AAF5BEB0B40D5C25B2A10AC6E1FBCD32650CE40592477CC4AACE41C75FCF6FB6B063353257A
        Version: v10.0.26100.2308
    directxdatabasehelper.dll
        Address: 0x7FFCC88E0000
        SHA: 62D9652505B17C9CC526C51A858D256A0B74EF1DD806530D351646C5F9BEA0B31A95C6BDBDDAE5580D45E5B34B5AE5CA953BD4776F333C73F817E1558693D481
        Version: v10.0.26100.2454
    DNSAPI.dll
        Address: 0x7FFCC9B40000
        SHA: 293475D22010857C310CFF4B9A18F1A554ECAB28559D4FBF37CDE0988DCA8F1AAC0CBA0D945356769656189DDEF8F1D8F458933AC8E3FFE451B0ECFDB29AEE00
        Version: v10.0.26100.2308
    DodgeFramework.dll
        Address: 0x7FFC1BDD0000
        SHA: 751F029D68A1AEB631311369FEE4D825EE311738DC66946B3454C5643E9BBC097E3BB087DE21F28E12866793AE366547E15BA401972B6B0E517940D16B28F7FA
        Version: v1.0.1
    DPAPI.DLL
        Address: 0x7FFCCAF50000
        SHA: 3E832A4BC1567C41DA538CE2EF401C13F139A37056E5F49E413899E0D47590F0DA3B1674EEA2D4193183E067ABC45B7D2D5676C91471261D98391432E0D0BD99
        Version: v10.0.26100.1
    drvstore.dll
        Address: 0x7FFCC4A50000
        SHA: 541D7D418E7CEF0F6649E3F54AB336610B144FF31905C8AE1EEF709A677CCBC6232AB66C3225C2E0ACD7481480268547F6ACD9D001EC06C92F211E052BA2B586
        Version: v10.0.26100.2454
    DSOUND.DLL
        Address: 0x7FFC1EDB0000
        SHA: 551AC49BE49ACB721DC3F8BD1B038553DD4AA01A6ACAEEA85B29BE8EE59600ABB9474EBDA147B6273C9F8DC92EBAA1B641AD3C10AA678864B397D158BED85A0E
        Version: v10.0.26100.2308
    dwmapi.dll
        Address: 0x7FFCC8050000
        SHA: 666292E0F4771CDC401E89C095FD02BE0E197B8C4F5258E71F1770C2E5FB590F7017D038B5586835782D37A0B4DA05E085D1825879F04266A21E7701060C000D
        Version: v10.0.26100.2308
    dxcore.dll
        Address: 0x7FFCC8650000
        SHA: 774519BF13E700746E25685495EBF64DA1ABFCE4A907512807B7EE114AEB8ED8FB2879E7059C2832585C84EB31A3BD65144F1801EF5C0C527FA808641893DDB2
        Version: v10.0.26100.2454
    dxgi.dll
        Address: 0x7FFCC8BF0000
        SHA: EDF415D74159DF1A315BF3952B737F06279BF1C4751D62E19082904430D77AF6BAF46C9A5BF2D36243964B8E8F1E62DCC5FB5EFD909A69C9077CD53A56A060FB
        Version: v10.0.26100.2454
    ENBHelperSE.dll
        Address: 0x7FFC210F0000
        SHA: 0B5714DCDD07A8966DB93494800966DE8239073449D907A0ABC957FE1C2F70E943BD0141B043EECF721B19C7E7E3D15208254B171B36B65DB87D52F6CE8BC0B1
        Version: v2.2.0
    EngineFixes.dll
        Address: 0x7FFC24440000
        SHA: BD3077244351BFEB71F0A5B87BB192DFBEF68E3D7E3842F71B5C4683840472FDE93A740EC66ABBE0C29806CA58809E8A7C767FA3FD94E7AB40A8CE863F56E443
        Version: v6.1.1
    EquipEnchantmentFix.dll
        Address: 0x7FFC51C70000
        SHA: 2BFB1D8A802906469BFCCEC5635D3F2913A23364DD9284879ACE570D897ACA12879BE2259214104A8BF504459B7B775E2263FE4AB8327742689CCBD17091B6BB
    EVLaS.dll
        Address: 0x7FFCAD470000
        SHA: F0748EDC83749066D83872B7B5E0803726A3B00B3EA73412448172BDA815DDEA74E0EAEF7C9D378177E91E587F525AE5D3EB8F79F02C06ABD0F43F2315E755FE
        Version: v1.3.1
    Fuz Ro D'oh.dll
        Address: 0x7FFC24060000
        SHA: F88C912B09FAB4D09E84C694A55C884E9CA8B191CCA03EB089CDCC2D81948B13621BCC5AB0E0487A858F37C84BEFDCED71D7DBBF6D58932DB83149CB47CEB458
        Version: v2.5.8.123
    fwpuclnt.dll
        Address: 0x7FFCBD1C0000
        SHA: C930ED477B57D8162B569C3DB9B3E199CC31BE802D6337B506B22C651AFF438E1DE42332D5432E27CE8A271E5AA35D4B543A7D019DDBAE5549269A27BD35E446
        Version: v10.0.26100.2308
    gameoverlayrenderer64.dll
        Address: 0x7FFC12890000
        SHA: 187BE05ED1412899BF6F52EFC023FB98E72F0EE8425C69A37D08238741C16C39A805538A28B91E99C4A7F38C9F473F6149D8407980CA265906C3899FE9442954
        Version: v9.51.87.58
    GDI32.dll
        Address: 0x7FFCCCB60000
        SHA: 75F91614AD159A37FD599186FC8CCA3EE9C3EFEAC6E96C1F3309ABE7F902904F95342B4BACDC8544EEB6123250302C2BBD26334F2DAAE34182750C5B548B5514
        Version: v10.0.26100.2033
    gdi32full.dll
        Address: 0x7FFCCBB90000
        SHA: B411ADE04062AD1D1FD44325CBE8F360B396E27F0C446B474FA8EEA0A8FEDAC2BCF2820EB5BC127D2CAFCEE15D5397CD013682E138A906487F2090BB68CFCE78
        Version: v10.0.26100.2454
    HellbladeTimedBlock.dll
        Address: 0x7FFC1BCF0000
        SHA: FC94CE8CC49ACDE62DBBBE363A318622F8979F923069DA8BD5AD02F7401794CB68DCB96C92A545A7C8F7C450B863B15228D3439418F97588927E9C3532B6770F
    HID.DLL
        Address: 0x7FFCC9760000
        SHA: 544539016E5310BAD14FAEF413C0519200B7A93BCFEDD6005888D7E537047261882CC3D359F7F9FCC0500D3DDA8B89BE5F842830DE9B871544E2ABD69ACC2E25
        Version: v10.0.26100.2308
    imagehlp.dll
        Address: 0x7FFCCCDB0000
        SHA: 60306F222CD4FE32CE5BC2E5CFF52F44E547DDF67583941440AC6A7C2853626BB1728FAC813AB184AC26ADB7E16FE1EF6D52FF5F228BEE64D94248DA9E8A4ABC
        Version: v10.0.26100.1150
    IMM32.DLL
        Address: 0x7FFCCCD40000
        SHA: 746D7E040A487E468CD4A853C47BC5EBA2C46B3598FBE4A8CE851D310C2D351B8CFE8B8777400C94D1C96406C69A6377C3D2B890E6DFB2762ECEAA8196CDA480
        Version: v10.0.26100.1150
    ImmersiveEquipmentDisplays.dll
        Address: 0x7FFC14400000
        SHA: DF19303DC54AEE4DF62844CC55A81B2313ED33B9C0E9942E2F375F6647097587B26AAC1009F3326CEC49D84EF2986CC523303EBA1E1040C3A69B378A0B79C211
    inputhost.dll
        Address: 0x7FFCA8D80000
        SHA: A00349A78A0193FC5AAF7D344F290DFE1733BBE97DEAA392A03BF00327CF8D9ED869D28C8C218C1D56F10BF7FEDF76FDF89B2073467F1D9C6A1F51298B157525
        Version: v10.0.26100.2454
    IPHLPAPI.DLL
        Address: 0x7FFCC9B00000
        SHA: E630F4AFE110C32F87F42B3F342F941B7AF865EB50A6A597DD7F6ED50C029BEC3FEE4DE44488B483B9A98980A32EE697675ED811D92D1114403C191C090721EC
        Version: v10.0.26100.2308
    JContainers64.dll
        Address: 0x7FFC1BA10000
        SHA: 6A2E301A005B1680E3C0DA604300CCC2ABFA765CD744F4C5920C4347D1D2EB733FC1CD86EB7EA95B8DE5E491467DCD40B82E8F31186C8B878712DFC1C6DF41C2
        Version: v4.2.9
    kernel.appcore.dll
        Address: 0x7FFCCA030000
        SHA: B45CB1BAA443E53B0BDE895EA5E26D417B1834B0489C538CB67902E2F58F3170EB6D4037A2C0DDCCFCFBFE2BE18744FB6799D654EB3FD3B5DDD559A5F7226333
        Version: v10.0.26100.1591
    KERNEL32.DLL
        Address: 0x7FFCCC9E0000
        SHA: E5B3FCBCB2853373AA4AF8B0BB4B2E0B9A8DC7A46317712A5EB4E3BF845DE0DCB0183DEE7397B0E47FA3B17CC4FEE4714B4C9D40552CDDACCED779FB85D36AFB
        Version: v10.0.26100.2454
    KERNELBASE.dll
        Address: 0x7FFCCB650000
        SHA: 0137EDCF25EEF5C740476AE579AFE51D89ECCF7EBDF7C16440AB0D5A998986F74CBD31D647937ECC9CA227375F2A9663271A5EE7788D1BB5765ED769B1752DE3
        Version: v10.0.26100.2454
    KiENBExtender.dll
        Address: 0x7FFC188D0000
        SHA: 82255379734938A9D7DF5D4222A52153BDE6640DEE299AE0E24E890C56A75B6650858064F9213E32102313898772009D9A71D92800C9A7785B9839BB52BCF5D2
        Version: v1.2.3
    KiHalloc.dll
        Address: 0x7FFCB2730000
        SHA: D0065BE02EE36C769C0D701D692599C827518A69021C07632426193F00CB58CB44B1C74FDB56E897D86A29C324B3612D99D1C9C8008838AB7F7A4FBC87394EC0
        Version: v1.0.0
    KiLoader.dll
        Address: 0x7FFC19180000
        SHA: 97302272715629BC8A82CF8C47D1D87E61FC66A42D46E67E17986F562813F61A0EF3503BA54E9AB5EA4157E6AB313B3CC3FFFA1BA9ECDEE05B6DCCDE5E06C4C8
        Version: v1.2.0
    KiLoaderSatelliteENB.dllplugin
        Address: 0x7FFC85C90000
        SHA: 8C01C6C32D045C21D395BB58D6208B0012FEB310B0691851EB69E7EE9F15AB70FC9FFC1D8CE25DD159DA1149D8175340591586019867B6A2CD5C3C7C1668F04A
        Version: v1.2.2
    KiLoaderSatelliteSKSE.dll
        Address: 0x7FFC228F0000
        SHA: 4B1C14E556881D060E4081069CB0BBFA8877D210ED68F7CFA0E8BA9198258B68AC46D5DB1E665D8CD52C24911C98DD558AACCEDD54998FC549641068FEA60493
        Version: v1.2.1
    MaxsuIFrame.dll
        Address: 0x7FFC187D0000
        SHA: 31380298360298C47812CF8C0784E968DA4B25E9FD9A513FC527B25A9B664FA3ECA3714F25841F55B05FB6FFF6CAFFE80311CA00BD863BAB72C7B26BD8230B25
        Version: v1.0.6
    MCMHelper.dll
        Address: 0x7FFC14320000
        SHA: 64B46A09756154AE6D0D03975F59D2EEC27A9128ED07EA0E6B5D1D7ED2E29050E16D46294359F6EC130B206A8AFDACC1FAEB3CDCFBC38382ADD1283E5519F31C
        Version: v1.5.0
    MCO.dll
        Address: 0x7FFC203E0000
        SHA: 2F12C00952BC501DAF2BEC2A5BFD983B0C12687EB37785ED7828AE2A23F137280D645F25F9F3DE281BF9DB0788FA740EF681B26CD2A60EC60ADE5CC84D6E9DCB
        Version: v1.0.0
    MCOBlockRecovery.dll
        Address: 0x7FFC190F0000
        SHA: 068E9585A469E4175CB9CFFB5CEFD9CF46DDE8CD9E1DBAABB493D7ED03E64F84445B11C8F9C91A0BA9F78DCD20F4B7D04E78948F82BA75C84D7ED84CBAB2F11C
        Version: v1.0.1
    MergeMapper.dll
        Address: 0x7FFC14240000
        SHA: C70F716D00EAA9D2CE84CC19E33DAAA4D9E320400DC77E8753E755DAD21562399B8D04C5C2776A31D22723C447EFB23FF77E3B5F7C24A10205D4296A3AD01736
        Version: v1.5.0
    MessageBus.dll
        Address: 0x7FFCAE320000
        SHA: 874438CD0AB8008F8452807D9FAA9639020141579107DE6A084A5FA8AB1D8DEC5B76D09E4718C8B170E0A36AF4657E0B37F6750F6106854DAB1E97FB8BC1C084
    Microsoft.Internal.WarpPal.dll
        Address: 0x7FFCC6740000
        SHA: C7E63E3D47B78E62EF969F5DAED36EA4F6450D1A83163B1D53022EAD9DE089BC55607978DAD4606B49A3F2590AD64DEAB98E2D191096C596F4617766AF2AEE12
    MMDevApi.dll
        Address: 0x7FFCBA9C0000
        SHA: 6E490AA2EC69D61FA57209E0694DF85C29BBAA40BD0D4B2FA882322C9A0A8329F7F657E864FDB8EAB8B43D83E07BB3CC57525D16724915405863ECC77F9CE7B2
        Version: v10.0.26100.2308
    msasn1.dll
        Address: 0x7FFCCA8B0000
        SHA: D5EDC8FA56CE73E773B519792C45CD0C6F74C73C8B6714013E6EDF42DD4825E31B8275EE08360205E9FF741F08D51016CC1559C9AC92AE631C726B3FD91340BC
        Version: v10.0.26100.2894
    MSCTF.dll
        Address: 0x7FFCCDBE0000
        SHA: 746037EA459B84CB80BF6305B4423D061CEB97DE5EED5FB8419DFEBAAF36912D985907517A741FCDA0A7A2F0C803C6856951E3CE2FB9B40DC28214DA7D411375
        Version: v10.0.26100.2308
    msdmo.dll
        Address: 0x7FFC9C840000
        SHA: 3D980D5108DDEF62F8386ED36733453074DE567E7D031B77E8DD642BE0A75639DD5F2D0F05E573F927E5DD34177DF09496B500B29BFC27213207C578FCC295EE
        Version: v10.0.26100.1150
    MSVCP140.dll
        Address: 0x7FFCB3C90000
        SHA: A81FEB56AE3E4939ABB21597F4F60429B704E04E6C20FAC402A0518FE7B29606BF8824347A7570D98F3C44684C15BF6B520E350321BFC2A42EC5597989215782
        Version: v14.42.34433
    MSVCP140_ATOMIC_WAIT.dll
        Address: 0x7FFCC5CA0000
        SHA: 2D9FA95A068784A8E799362FAF97B42253DBD614DA504907ED01D1F7F3FDC56D1BB964B2009171EDA87149A595D84EC83D50DAFF30BE9BD6F7A3C76C75226C40
        Version: v14.42.34433
    msvcp_win.dll
        Address: 0x7FFCCB510000
        SHA: C42D63EDFC4FEEDD3FC4C2F330B3AD2054D9FE33128CB9D54D29A0365FC88C452F59AFA9B2822EFFEEA9D2D81CC0D4E0A0A39873B2C5480216AF68C601720034
        Version: v10.0.26100.1882
    msvcrt.dll
        Address: 0x7FFCCCAB0000
        SHA: 834CA6FFB7D2C378BFCE04B95CA667162D6933F45E8BBE41C0CC14496E8AF65AE9E3AC3BF70C21CCF0EBA1DA7A418FCB65851E614A90A05055E9D81DC72B67BC
        Version: v7.0.26100.1882
    MSWSOCK.dll
        Address: 0x7FFCCA510000
        SHA: 48031068990A509DE761F7B7833514DA44CA2A1704F7A73D5A60C90B562136D123195C2ED766907FDA0E72F59D9395FA5C774F3B6832589BBD32357991E22FFC
        Version: v10.0.26100.2308
    ncrypt.dll
        Address: 0x7FFCCAAB0000
        SHA: E5C8F393C6AAE64BF8F2863C345C145B7D178DDCA2494A7C1EE4A09B7FE08EDB01998E60C512FAC773D0FE088C25901B5E490745DE43FD18D37BFFD84D67C0C3
        Version: v10.0.26100.2308
    ncryptsslp.dll
        Address: 0x7FFCA90D0000
        SHA: 190EE5C8617722B29B8DA13CFD1E30AF3E8888A67F8FE82DF1AE8FF51C18C80BC3DD369964C5D99ADEF81A56303F0B08DBC027A4DA36E7FAA4F075A882203B8A
        Version: v10.0.26100.1882
    NSI.dll
        Address: 0x7FFCCBDA0000
        SHA: 0947FE4280A6055DEFB918B148CBCE27047FDD6E04EFEB6D84739799471753867BD32C5457F1C9A0151569917F9E5D0EE1816784081D4D3C3AE8D17CB71CA0F7
        Version: v10.0.26100.2894
    NTASN1.dll
        Address: 0x7FFCCAA60000
        SHA: A7073268A16E89DC503434DC1FE745A4F21FBF549C78ED69D7E1FCF0FB2F1333462426E570CCED18558F47A33048F2B4214D38D37F6518DC05586305C989815B
        Version: v10.0.26100.1
    ntdll.dll
        Address: 0x7FFCCDE60000
        SHA: 7F3CB87D4D41EB737793C13963D7C7A4069E9D11E8476F1309225C5250B0596E09E2EE0E95212E9BD450B54E99C4F19AC97C047D154DEF620E92751DC87BBD36
        Version: v10.0.26100.2454
    ntmarta.dll
        Address: 0x7FFCCA150000
        SHA: B46A4C36238AF06DBF3BB5BCAC75A0AFE2F7880E96CCB66016FA5FC5CCA176A0547A4717CC1459678EAA242CF64BAF90A22BB7DFCF26F82D7367E14D92E05332
        Version: v10.0.26100.2308
    nvldumdx.dll
        Address: 0x7FFCC4CB0000
        SHA: 6ABF4663503B8E86F3C54E0FF82D9C7DBC87EFDA269180EA5966B398204BC0F1B4BD41672877F8AA212456EF2AEEDDF3C92A2C69D12F0C8C00B20E83765511EC
        Version: v31.0.15.3667
    nvspcap64.dll
        Address: 0x7FFCAFC40000
        SHA: 838190308C79E116CF01D55542CD47F673C27F4158DC85C21C5AC40BD03B322C064B52BEEDE74E63533E06DADA4E35177388CCC4538C5BB7F139F688A1B0A686
        Version: v11.0.2.312
    nvwgf2umx.dll
        Address: 0x7FFCBD9F0000
        SHA: CAE99F6552B23790C2B49C910E8BC894B4CF5BF990FED92684ECC697F4D95DD4344AC673D97A12C3E883F8EFBC3087792717E97A59D1916844584D2F0BC4C0A4
        Version: v31.0.15.3667
    ole32.dll
        Address: 0x7FFCCC840000
        SHA: 29F9C897E0F33888359563B4BA2617F60C5A5E7F956E966A7A86B2776A06593E24660D21DCF952192B6DDD2CFB52188D48C21B92112E3C88FD01B55BF6111335
        Version: v10.0.26100.2308
    OLEAUT32.dll
        Address: 0x7FFCCC220000
        SHA: 7EA34468B9C72E2DCE04E346BBF1E70B0C8C5314768EBACCC43014A641538F6FD852574036E6C39236AAFEB8EB2C93760FDDFAB1BB8B29EE3951EE189E856226
        Version: v10.0.26100.1882
    OneClickPowerAttack.dll
        Address: 0x7FFC21580000
        SHA: D9566FA19D141BA13B8877C1DCB909C554D16B34C82153FA6C398F46C6A485DC96E1F1AAC970CA2C146A0C09CA12D625F87377992917DEF696E5BEE66DC0185D
        Version: v1.0.0
    OneCoreCommonProxyStub.dll
        Address: 0x7FFCACF70000
        SHA: 72A909E4568E8BC79B6F02032437918DDCE00649840666B3D10546BB4D6F34AF246C7CDA1A8C2C851094AAFA911508AC835D90963B675D4CCB713945977E7A54
        Version: v10.0.26100.2454
    OneCoreUAPCommonProxyStub.dll
        Address: 0x7FFCBBD30000
        SHA: 48BE383CF3781E115AA17E04C8F1450402768FDD9E890541BE2FAB67E8134D2973625E90E2CE637A9BDF3F046512DC0AED5B8E7984E27FD62392F1F340387F03
        Version: v10.0.26100.2454
    OpenAnimationReplacer-DetectionPlugin.dll
        Address: 0x7FFC14150000
        SHA: 299D914FD60B948F90454460A19233CB79495B772D33CB9FAD3E78FEBBD7530F96F4535DA20E20074493C8A552B007B3A17986459F0A27801E6B7368E867039B
        Version: v1.3.1
    OpenAnimationReplacer-IEDConditionExtensions.dll
        Address: 0x7FFC14030000
        SHA: 08C96C6934225CB604CDC0CCE59FE9825EDC02039A4F86D0E305B1944CEE07C99854C66EB3EA9D312422DFEB925E39F0393B110AECB569DE3463109B9823F823
        Version: v1.0.2
    OpenAnimationReplacer.dll
        Address: 0x7FFC13CD0000
        SHA: E2BB138D136EA67D73F5741E5DAEE316F40033C61E8B52C19DBAFAB888F6D4D577D1E17046A85CE69AE25AF443F5C73B57470D5D1808500FC67134EF6D815ECA
        Version: v2.3.6
    PairedAnimationImprovements.dll
        Address: 0x7FFC13C60000
        SHA: B3AF5F598B7FF1C87826505198BA50156510AEB7E580B6B5C887FC29215C8F95A14F4023CC8F32CFE39396C9C7F19445AD522CFDB4AF43A69D03956818BCF54D
        Version: v1.0.2
    PapyrusTweaks.dll
        Address: 0x7FFC13B60000
        SHA: 9292B4CC6A72A61DA67793F89BCD544ED73292C1E8564FC86A6A4017D2CBCB40BBADA206842E301CCC6F2E0A9AB4D2456C773FFB5074572EDC36D5F800E8437E
        Version: v4.1.0
    PapyrusUtil.dll
        Address: 0x7FFC139F0000
        SHA: 971B7F4C59812B0D061AFED2704A91CF2063503B990BBDD6FD4EF452294D9385DCEB4D506CA5A106FB6B5E206ED7E862D784A42BD9D18C5E0898693ECA6268BF
    PayloadInterpreter.dll
        Address: 0x01EC8FF20000
        SHA: D5DBC2A619FC1C4AFE6A7967D4225F8EAF409BCE7F3DED56AFDA3D667AA7AE716096E39D2347CB144F9FB0A2F092BB9B1698DBDA7643F850DF8B86C056711139
        Version: v1.0.0
    po3_KeywordItemDistributor.dll
        Address: 0x7FFC137E0000
        SHA: 18843674F491830E6135614D6137E9F7B718B318BDE5A1C8E27D702E0D1934EF7983E81C6A07AACAA0E3F437D4025AAEC20131136E2B76746C983F1A3637C39B
        Version: v3.4.0.1
    po3_LockVariations.dll
        Address: 0x7FFC136B0000
        SHA: FD03413F283A2701E782C66CE9C95A7766F98F9A22CB40F6A30F180BA1006B67BAD06C538A8E3EB41493530876EC4C1648256692CA6C433AAB5BB2106C1225BE
        Version: v4.0.0.1
    powrprof.dll
        Address: 0x7FFCCAA00000
        SHA: 50D68A1C3F44D0B90D13DBE74DAA19EE3045193C65772FD635A41AF84E36C2FACB8AD3AC98DC91F7FBF468E5E42878343C64DDA84BCC1297AD63D8A536E79B7B
        Version: v10.0.26100.2308
    Precision.dll
        Address: 0x7FFC134D0000
        SHA: 7238FD553247730D2D33898CA53ACCC46C1DDA6E455EF320511E3C458FA44CF8FE8A77DC513732F8CAAAF3AA052345CEAF8A68C91127A434FC703DEF05152E37
        Version: v2.0.4
    profapi.dll
        Address: 0x7FFCCB140000
        SHA: 48033FD3079CB88008A6F461DEC74EAAA17114887F50CD71D1F32C98569FF2967AB75F9B30CE52FB263B5860B53FE48C8D220A524BC97C069BB27B322855E37E
        Version: v10.0.26100.2454
    PSAPI.DLL
        Address: 0x7FFCCC300000
        SHA: 986DBB58CB62378FA9AB8A62A1362DEBF59CF674ED811F6BE727B106EB672860119EC120BF9B6361DFDB919737BA1B356BCBA5CCF7E1E4A82945B0371386F5BC
        Version: v10.0.26100.1
    QuickLootEE.dll
        Address: 0x7FFC133C0000
        SHA: F6F426AEADE9A0E7572CF639DF00A5FE5A97A61110C27A33BE23995524C58D63A05A30240EBF4AE995DCDEE3B90C117468CC4EB03E38A8AA9249401BB7793A9A
        Version: v1.2.0
    rasadhlp.dll
        Address: 0x7FFCC4120000
        SHA: 4EF633251D0F896827EDDD5091F24A7E816CFAC4670F1A5FC41D662539D6A0D5FDE788408C0E90E0F9ABAA3357C11F0C77CBEF45CEDCDA52F8A7D903D8AAB2F6
        Version: v10.0.26100.1150
    ResampleDmo.DLL
        Address: 0x7FFC1ECF0000
        SHA: 04D181AB42E9C1F1E9F6FA97713FBD6BE8A81B2BB99DAB57A18CE51EF81601ED341184C80E824342AAC7A003E29CF12D0B27EA019D9111062A1739016D7659B4
        Version: v10.0.26100.1150
    resourcepolicyclient.dll
        Address: 0x7FFCC86E0000
        SHA: EDB57D9B82245EBEB2991C34181AAF44CB94897E529BFC9CBEBCCF3E42CFFBDFC6723EA527F31F0BA89CEE55231994A13EBA4CED312B97A9DC104BAC2E1DE5BA
        Version: v10.0.26100.1150
    RPCRT4.dll
        Address: 0x7FFCCC4A0000
        SHA: A5E8CB45EBEC5B4D5F954E18BAFCEC6F8AB2827B4869178ADA622E25BBA6DA6EEA25A20DC91583C884C37414A48606015000D75A1073E113FEBBD5F6D89487EB
        Version: v10.0.26100.2308
    rsaenh.dll
        Address: 0x7FFCC9F90000
        SHA: 6DF21F86E0F1D9FCD68E044CF82ABE568BC8B695FE63F55BAFFF2A604D178CA87B5067A7FDEC1C9AB002E3773BF468533D174A578A5189E872D483E374A265C6
        Version: v10.0.26100.1
    SCAR.dll
        Address: 0x7FFC131F0000
        SHA: 240E50D33C3245F65EE4C1746906D47E86577BCF77AFD1A062A30F278E4295AF038A8A6E1A0008B93399022501475377E89F56AECE0D3EA6ED292E3D094F2F07
        Version: v1.0.6
    schannel.DLL
        Address: 0x7FFCC9E70000
        SHA: 7FD5EACD667E64E1E7ECC3C15704E4CC02D00DB1B579BFD67530310C5A8BF43A87D8B7F811409B754C101260A894F6FCB985EC415CCC4F2C5396B2B947DE4F10
        Version: v10.0.26100.2308
    ScrambledBugs.dll
        Address: 0x7FFC13150000
        SHA: 59F27D0238C4534875F3B6F815C274697358142747334D235D4614D7BF33052AF5FEFBCBDFA493739EA3B12F942167F8541DAE7323DA9A1D5C3F5B88C3828D9E
    sechost.dll
        Address: 0x7FFCCC310000
        SHA: 9E337AAA3B01E4D852F41CCA0BBFFB928197483D7CFB19BA6C1B464472D21683F38E3A1E6C9460CF0DE9923FA55F4924045C72E0FBF4D21DBC58BD4E2DA00EBB
        Version: v10.0.26100.1
    Secur32.dll
        Address: 0x7FFCC7250000
        SHA: C1128CD1C66D1ED0DEE26ADDF77F6893B1017DE8DE1AAF00CDA1C6597BA7D24E486F364621E13D1333029D69868ACDAD0689F0369ED5220FC4944BD919DF561E
        Version: v10.0.26100.1
    SETUPAPI.dll
        Address: 0x7FFCCCE70000
        SHA: BE4820AC3517C32BFA4DA71E21D5C73092D1329F488038C59C788ECD94BBF64FB5524D4831D9BDEF6EB1A492E3D8A0751DE77CCA222E36BAD48B724B7FBE7A45
        Version: v10.0.26100.2308
    SHCORE.dll
        Address: 0x7FFCCBCC0000
        SHA: 612186FBF4064008B97D7E20EBAAC2DF657A75F33E9CBA9416225875CDDBB9DA99A4E4EAAA8A833449A234430840484EE50648322D249224723B8A226F056391
        Version: v10.0.26100.2308
    SHELL32.dll
        Address: 0x7FFCCD4D0000
        SHA: CA979E10A150BECC02ABE1A3B838AB973B337405EEA4C1CF42E279DE36CB31CE7B90695DC23307335CA97D3FE839C343A203F52A223EE04DD3811B3AE629B875
        Version: v10.0.26100.2454
    SHLWAPI.dll
        Address: 0x7FFCCDDC0000
        SHA: 649279D7D0968ACB92E78B72054BB8832C38281A0CAE7CB2C90F09C02D3F2368484DA9F71490491F117B68B2AD714ACDFFAFF3517D0A75D49CFA6BE6D2AFCB9F
        Version: v10.0.26100.2308
    SimpleDualSheath.dll
        Address: 0x7FFC130C0000
        SHA: 54EAC1A3515C1DB81D6BA7C5089B32A17EE8E72FEAA2C9A8789AA5AFDE02E4B48F8D2CB334209DEAE86B4F0AA995C25F1F6320E090100C937645F0267FBA5C8D
    skse64_1_6_1170.dll
        Address: 0x7FFC24550000
        SHA: F88C10E637F67131775414DE7691884E1BD181C750DCB7B9CE69FED616285BC69BF2F5E81177EBF2CB42BF590F709A33D722BE42CAE1809B49729FFFFFB75567
        Version: v0.2.2.6
    SkyrimSE.exe
        Address: 0x7FF6D6150000
        SHA: F7A77A0646E83A078FF8A2004C39533D132B5B45B93A3C0F4B7F0FE01977E79D4028336439DA03258B1A01FE01EF23C9D30F6DF59BBF0AC0113A14EF15A4B58A
        Version: v1.6.1170
    SmoothCam.dll
        Address: 0x7FFC12F50000
        SHA: B3E41421B12842533E80874A904E08F280ED8C683F68DD1FE280B93BE036A1965E0031E4FBFF22A1197B6B5A285FADF8FEF1DAFCEDA6BED243885BD1B37A6646
    SSEDisplayTweaks.dll
        Address: 0x7FFC12EB0000
        SHA: 9D2BB0CA409F63C72E6D8D3D48347EBED959F9833236C01E8285E5BC7F06D18380CDD08FA4EFF6666A15252131E2465CE2EC87793E775E6950E4D859400C889E
    SSPICLI.DLL
        Address: 0x7FFCCA2D0000
        SHA: 7597BEA308A17408B98892CA54E8A37DF1A0EF8029E029553C63A5925BD1983BC3D4B33C648F8AD5D07F5986A5F2EC36236F6467C976CADE2D2AC704D3539675
        Version: v10.0.26100.2454
    steam_api64.dll
        Address: 0x7FFCABA30000
        SHA: C08DE8C6E331D13DFE868AB340E41552FC49123A9F782A5A63B95795D5D979E68B5A6AB171153978679C0791DC3E3809C883471A05864041CE60B240CCDD4C21
        Version: v7.40.51.27
    steamclient64.dll
        Address: 0x7FFC56090000
        SHA: BC52657F85F289D93CE9581678EBE06C1A3103C55808C5565A213D22E962790CA0C3748BFBCAD8748444C0C5D34ED3F69E6997EEF680E907AFDC39E4897373B8
        Version: v9.51.87.58
    Subtitles.dll
        Address: 0x7FFC12CD0000
        SHA: 90CA292A6B7FED8D36AB0509DE427137E22A1A752A67CABF67A2FA31ABE65AFFDA8AC9AC4010404A169182BF5311A2930271D026454CE10DB37439E777F07260
        Version: v0.6.2
    tbb.dll
        Address: 0x7FFC971F0000
        SHA: C5F706879474491A49D4A7218403559109E99FCD9456A39DBD0D4209827B56F9BEB8AE5E66054E8AA2D7F2B8C07B91E9656759964D5C81103A5F90392E878A5F
        Version: v2020.3.2020.622
    tbbmalloc.dll
        Address: 0x7FFC9C660000
        SHA: FFD14E67EBA74CA56FF301D6E72E8EB5C0127E2101EFCE1CA78F44720BD633DD54D174DB4BB0C78F1D33537D78799256DDD7D8029672AF0F2236266754ACFC0A
        Version: v2020.3.2020.622
    textinputframework.dll
        Address: 0x7FFCAEF50000
        SHA: 62C8E1590EA07DFF68BC75E6205A663EA96F7FB173CB43FCEBE19FDA475691F533E0753215E182EF127A673C43652783B4CED356FC28112DA8BC047096DF13ED
        Version: v10.0.26100.2454
    tier0_s64.dll
        Address: 0x7FFC55EF0000
        SHA: 41669EE2EC39AF67204BAD7042B001E8469D9F01C89F1B8DA2D55AF98AD95F1C71BFFD4F2868C3D537467776EF0876E64525FC7470CCACE1FC82C60B6C66A58D
        Version: v9.51.87.58
    trainwreck.dll
        Address: 0x7FFC23910000
        SHA: 261801A85D41236E35C820A78E4BC3E775EBF0C19336EF1D518A61DA20429BB30B707181606675C1BC650D678CA0A27DC585DFA35BDDD717EB830459BFF60333
        Version: v1.4.0
    TrueDirectionalMovement.dll
        Address: 0x7FFC12BD0000
        SHA: 756BC2E9EBEA978175671B7A5D8E496693E9746738448C8B75E2DCDFA86D5EA20D0EC13D12C648886767573C09BB93E26E8FB5F04DA1C9A6852EBA589F9983A7
        Version: v2.2.6
    TrueHUD.dll
        Address: 0x7FFC12B10000
        SHA: FFB0DC0E2F00AF463572A36A861498F6D213C34D35815FEA9921F014AEB15515ED736784D36562ACA44895111AADF73DD9CA2549A0A2EDE8E825404C507FD871
        Version: v1.1.9
    ucrtbase.dll
        Address: 0x7FFCCB260000
        SHA: FD2C60A4843940BED33EF87B6BC5AA646218C6D63D0EC300F11B37D3734946274D7EBCA9CA23E012AEEEB079AF6AC8AF3580C3D7EC2653A0B9CB2A1FEEEBB2C7
        Version: v10.0.26100.1882
    UMPDC.dll
        Address: 0x7FFCCA9E0000
        SHA: BE4A4B98F5402D82FFB56D4128B165412A553AE0C86DF7E3B41D63FCA1E1DC023369910253DF40D6742D01FA0D4971B19BEF26F1763AC6A96187BB512CA5AA0A
        Version: v10.0.26100.1301
    USER32.dll
        Address: 0x7FFCCD300000
        SHA: 328040695915E1B7A83C70E8A7966CF016B08715B7B152738DCCAD02E83D859D9044EFA7CFCEEBCB7478FF293DAEC165AC714E95E506D48EB507E2E661D696A5
        Version: v10.0.26100.2308
    uxtheme.dll
        Address: 0x7FFCC7670000
        SHA: C7C38B1310D0A09134240014B65294BC3D4948701AB4093DE6E88088E3C6FA86A278CA286C50AF235995AD5A33D19D9E79014512DFECAA429A34FAE6C0CEB1D6
        Version: v10.0.26100.2308
    VCRUNTIME140.dll
        Address: 0x7FFCB3D20000
        SHA: 96E9F32E89AEE6FAEA6E5A3EDC411F467F13B35EE42DD6F071723DAEBA57F611DBD4FF2735BE26BB94223B5EC4EE1DFFEDF8DC744B936C32A27D17B471E37DCF
        Version: v14.42.34433
    VCRUNTIME140_1.dll
        Address: 0x7FFCB3C80000
        SHA: 0460CC66D06DF9A2941607473F3ECCFD909F2ADAB53A3328FADCEDD1B194B388ECA738C2C6C2E193DE33606925FBED1FE39EFA160015128E93F5E3A03C62170D
        Version: v14.42.34433
    VERSION.dll
        Address: 0x7FFCC4CA0000
        SHA: D1BF36744AACEC8A95665F56F5CE4CF00685F836C4905B5A51DEE55C803FAFE6FC8069A08FE3959761B5A2E6367A2283077828958CB4888B909F7D402F6FD917
        Version: v10.0.26100.1150
    vstdlib_s64.dll
        Address: 0x7FFC5A4B0000
        SHA: 97F33F4E3CB4C23F747BEC082A0629DF82C2FBB639690416D14A7CEE4EADF13CB8E95EFF9155A6EF8FE7FE264B08DABD144D9DD3C4537828AD6A4DCC8719881F
        Version: v9.51.87.58
    WalkFixRedux.dll
        Address: 0x7FFC224D0000
        SHA: 68B1C2E84B9C7C614B4535C0EA850EEB0EFC3000F4FEFA01AE01A3F1E52334B0877C0B7FC725502D1A17DC67841AFEA9A892DB8732F710F10CFF88BC22E810DF
        Version: v1.0.0
    webio.dll
        Address: 0x7FFCBA4D0000
        SHA: 520CB385CA97A327B8836F4B57E184BFE985E851C127F27FDCA157F0A52C9A887358E1CBCB1ADA8B0C0595B396DF963CED0A7C770265ACE871891F3425309704
        Version: v10.0.26100.2308
    WidescreenScaleRemoved.dll
        Address: 0x7FFC12A30000
        SHA: 7669F1AD2C934FEF622A70153B23DBE79847620566EA491E74F26806B9D1FE4AC1E1C4621F6CEE3CE6A47E2CF88BE584CB918177676C43B8158450467AC8AF36
        Version: v1.0.2
    win32u.dll
        Address: 0x7FFCCB230000
        SHA: 9839866ADC52A6C707EE2132F8CF5300680E96302478088E824CDDDCF52B9B8488F468C52149F2EABB5DB1D41102D29D2C3949D4EE03E3A64B995EFDF53DE6DB
        Version: v10.0.26100.2605
    windows.storage.dll
        Address: 0x7FFCC8F20000
        SHA: A7D1225FF246456FF99A8FE94374E70E042EACE620300D42BD05CD269CD6A7D4BED29F022FD1212BAE407C1D3A3C571E4A268F6D0624D79C5D1B021FDAA2515B
        Version: v10.0.26100.2308
    Windows.UI.dll
        Address: 0x7FFCB70F0000
        SHA: 2900764A539180B608FCB42932EEB2D5D62F508C9772A9DA28C80BE0DCDE6855C7A989B0BD3A1680DD410437CBEDBD5E1049B20EFAA6817798F3557D69A9F8E6
        Version: v10.0.26100.1
    WindowsCodecs.dll
        Address: 0x7FFCC7430000
        SHA: 26AE76B91F2865BA3D0A62BB4EF0CBADC166252EDAF148C002C3D9670FE9C83EB50B8FB5852C4858D83F91884AA65A7EE246408A8040330C79C7400D612262A7
        Version: v10.0.26100.2454
    WINHTTP.dll
        Address: 0x7FFCC3A10000
        SHA: 98F3E97D5D2D0BA1E879BF4BB9EE0282CEDE5B61B852D4BE4E1C69DA3779796CCCD3FFB122C4E6953EC1BAFEC2624A3337294693171CE46622D40D27AD2228DB
        Version: v10.0.26100.2308
    WINMM.dll
        Address: 0x7FFCBD8F0000
        SHA: 25BD462DE912B9D0753F7DB86B96D700E7B7BF486C89B8E426D3E71F035DFA05369C22162B093169D061C15744B564BAAC4C4F7008A1B5AC09ABBB5A7D59C9EC
        Version: v10.0.26100.2308
    winmmbase.dll
        Address: 0x7FFC3EEE0000
        SHA: 209DB243E7CF01274DFC119DF06790B1D768C99AB6932B0B6BE8E0CC4689603B088D26AF463493DC42A461520C0D7ECB1D5EBE72AEBDD498205070773C8FD6DE
        Version: v10.0.26100.1
    WINNSI.DLL
        Address: 0x7FFCC5DD0000
        SHA: 377B8DF74B8BB5028E958FA9B2836AC5F590C636C55EC058C33921CB0164A5272A1AF87B597AEE526DD3209246A625EAE280F4256AD79CC9F2639581F6530880
        Version: v10.0.26100.2894
    wintrust.dll
        Address: 0x7FFCCB5C0000
        SHA: C67611A466B3B5D7EAD8EEAD62DF4AF2DAED590892EA793CF94305F13498A2A5B3B778E60E1ED76593541B96FD9B5A5641453FF78337E9DBFCBF1F9B9D79D584
        Version: v10.0.26100.2894
    wintypes.dll
        Address: 0x7FFCC5410000
        SHA: 5CCDE34EF5133E9D60BC9CA23AE162235D4C61084AE9408FA75970C0C90757C762577FFB75D188A254A291DDCD6E3F3A8468A34B3A74CE40657DF89D7E0462D1
        Version: v10.0.26100.2308
    wldp.dll
        Address: 0x7FFCCA7E0000
        SHA: 1AD26649A0A8BA729E8183C86FD4AB6F252AD0C2DFFB111D8A319F2B683F1E9F3BE8B046708AC72242538C321FD413AC487ADC9526F35FD50FC9570E9FB49629
        Version: v10.0.26100.2308
    WS2_32.dll
        Address: 0x7FFCCDD40000
        SHA: A02BD113F6DDDCF958977EA65A05C5572F209D809EACCB04D13EC204A5A587EC4B8EEFABFCB399D7C1EF92224148C265B26B64EE0966AC60C08A2BA05D8A1582
        Version: v10.0.26100.2308
    X3DAudio1_7.dll
        Address: 0x000072650000
        SHA: CEF31793E1B1714826AA95D256EBBEC457E8CF9003767DB46909BF879AF86F954F475AC84E1EE8CCCF1DCFE4A52624E3D7E8BFAFF5F567E97CAB19207DB7F913
    XAudio2_7.dll
        Address: 0x7FFC24230000
        SHA: 2CF5EA114546236F55B9CBB49643F719D892EBA8649343BC3E72FE08C998E88E26C010232CA27BCA255629AE7D0D1E068D6ED1DBD76096B1ED09362F65F5401D
    XINPUT1_3.dll
        Address: 0x000000400000
        SHA: CE2EAD2480A3942081AF4DF4BAEE32DE18862B5F0288169B9E8135CC710EB128F9A2B8A36BDA87212C53FD4317359349C94D38B5DA082638230DCB5669EFEDE9
        Version: v9.18.944
    xinput1_4.dll
        Address: 0x7FFC85D40000
        SHA: BDAAF3FB1729548773DBBFEB3F6DBA8B182EA6DBFE080016379F1F89408010027FA7869C733C973B2DC5040AF4F796EEAC515195A18794A92EB7CC2D22E6C458
        Version: v10.0.26100.2308

SCRIPT EXTENDER PLUGINS:
    AchievementsModsEnablerLoader.dll                v1.3.0
    AnimationMotionRevolution.dll                    
    AnimationQueueFix.dll                            v1.0.1
    BackportedESLSupport.dll                         
    BehaviorDataInjector.dll                         v0.1.3
    BetterJumpingSE.dll                              
    BetterThirdPersonSelection.dll                   v1.0.0
    BugFixesSSE.dll                                  
    CombatPathingRevolution.dll                      
    ConsoleUtilSSE.dll                               v1.4.0
    DescriptionFramework.dll                         v2.1.1
    DodgeFramework.dll                               v1.0.1
    ENBHelperSE.dll                                  v2.2.0
    EngineFixes.dll                                  v6.1.1
    EquipEnchantmentFix.dll                          
    EVLaS.dll                                        v1.3.1
    Fuz Ro D'oh.dll                                  v2.5.8.123
    HellbladeTimedBlock.dll                          
    ImmersiveEquipmentDisplays.dll                   
    JContainers64.dll                                v4.2.9
    KiLoaderSatelliteSKSE.dll                        v1.2.1
    MaxsuIFrame.dll                                  v1.0.6
    MCMHelper.dll                                    v1.5.0
    MCO.dll                                          v1.0.0
    MCOBlockRecovery.dll                             v1.0.1
    MergeMapper.dll                                  v1.5.0
    OneClickPowerAttack.dll                          v1.0.0
    OpenAnimationReplacer-DetectionPlugin.dll        v1.3.1
    OpenAnimationReplacer-IEDConditionExtensions.dll v1.0.2
    OpenAnimationReplacer.dll                        v2.3.6
    PairedAnimationImprovements.dll                  v1.0.2
    PapyrusTweaks.dll                                v4.1.0
    PapyrusUtil.dll                                  
    PayloadInterpreter.dll                           v1.0.0
    po3_KeywordItemDistributor.dll                   v3.4.0.1
    po3_LockVariations.dll                           v4.0.0.1
    Precision.dll                                    v2.0.4
    QuickLootEE.dll                                  v1.2.0
    SCAR.dll                                         v1.0.6
    ScrambledBugs.dll                                
    SimpleDualSheath.dll                             
    skse64_1_6_1170.dll                              v0.2.2.6
    SmoothCam.dll                                    
    SSEDisplayTweaks.dll                             
    Subtitles.dll                                    v0.6.2
    trainwreck.dll                                   v1.4.0
    TrueDirectionalMovement.dll                      v2.2.6
    TrueHUD.dll                                      v1.1.9
    WalkFixRedux.dll                                 v1.0.0
    WidescreenScaleRemoved.dll                       v1.0.2




1
