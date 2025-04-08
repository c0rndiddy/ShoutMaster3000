# ShoutMaster3000


This is the design tree:
ShoutMaster3000
├── README.md
├── project.xpr                            // Project File
├── project.hw
├── project.sim
├── project.ip_user_files                  // Generated RTL for IP blocks
│   └── bd
│       └── design_1
│           ├── ip                         // Xilinx IP and packaged custom IP
│           │   ├── design_1_ShoutMaster3000_0_0
│           │   ├── design_1_microblaze_0_0
│           │   └── design_1_clk_wiz_1_0
│           └── ipshared
│               └── b368                  // Custom IP core: ShoutMaster3000
│                   ├── hdl
│                   │   └── ShoutMaster3000_v1_0.v
│                   └── src
│                       ├── TRex_top.v
│                       ├── DinoFSM.v
│                       ├── ClockDivider.v
│                       ├── VGA.v
│                       ├── vgaClk.v
│                       ├── AudioDemo.v            // Audio process custom IP
│                       ├── BackGroundDelegate.v
│                       ├── drawBackGround.v
│                       ├── drawDino.v
│                       ├── drawNumber.v
│                       ├── drawObstacle.v
│                       ├── gameFSM.v              // Game control FSM
│                       └── JumpDetector.v         // Audio score converter custom IP
├── project.srcs
│   ├── constrs_1/new
│   │   └── ShoutMaster3000.xdc           // Constraints File
│   └── sources_1/bd/design_1
│       └── design_1.bd                   // Main Block Diagram
├── project.sdk
│   ├── design_1_wrapper_hw_platform_1    // MicroBlaze Hardware Files
│   │   ├── design_1_wrapper.bit
│   │   └── system.hdf
│   ├── drivers
│   ├── ShoutMaster3000                   // MicroBlaze Software Project
│   │   └── src
│   │       ├── helloworld.c
│   │       ├── platform.c
│   │       └── platform_config.h
│   └── ShoutMaster3000_bsp               // MicroBlaze BSP Files
