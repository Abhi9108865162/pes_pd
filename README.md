<details>
    
<summary> WEEK-3 -> Day - 1 </summary>

# Inception of open-source EDA,Openlane and sky130 PDK

1. How to talk to computers

- ### Introduction to QFN-48 Package, chip, pads, core, die and IPs

QFN-48 Package: QFN stands for Quad Flat No-Leads, and 48 refers to the number of pins or leads in the package. It is a type of surface-mount integrated circuit (IC) package commonly used for compact and low-profile electronic devices.

Chip: The chip, also known as an integrated circuit or IC, is the electronic component housed within the QFN-48 package. It contains various electronic circuits and components that perform specific functions, such as processing data or controlling devices.

Pads: Pads are the metalized areas on the underside of the QFN-48 package. They serve as connection points for soldering the package onto a printed circuit board (PCB). Each pad corresponds to a specific pin on the chip.

Core: In the context of IC packages like QFN-48, the core typically refers to the central area of the package where the chip is located. It provides mechanical support and thermal conductivity for the chip.

Die: The die is the tiny, semiconductor wafer on which the integrated circuits are fabricated. It's the heart of the chip and contains transistors, logic gates, and other electronic components.

IPs (Intellectual Property): IPs, in the context of ICs, are pre-designed and pre-verified blocks of functionality that can be integrated into the chip's design. They are often licensed or purchased from third-party companies and help save time and resources during IC development by providing standardized functions like memory, processors, or communication interfaces.
    
![Screenshot from 2023-09-09 06-02-29](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/695b807a-7c14-477f-b8b7-a8670f9b223c)
![Screenshot from 2023-09-09 06-02-48](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/faa79ff0-b5fd-44f1-9a21-99d3f6612064)
![Screenshot from 2023-09-09 06-07-35](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/742e86b7-2dce-46b0-83eb-384c006be7c7)
- ### Introduction to RISC-V


RISC-V is an open-source instruction set architecture (ISA) designed for computer processors.

Open-Source ISA: RISC-V, pronounced "RISC Five," is an open and royalty-free ISA, meaning anyone can implement it without having to pay licensing fees. This open nature has led to its widespread adoption and popularity in both academia and industry.

RISC Architecture: RISC stands for Reduced Instruction Set Computer. RISC-V adheres to the principles of RISC, emphasizing simplicity and efficiency. It features a relatively small set of instructions, which are designed to execute quickly and efficiently.

Modular Design: RISC-V is modular in design, allowing developers to tailor the instruction set to meet specific application requirements. This flexibility is a key advantage, as it enables customization for a wide range of computing devices and applications.

Scalability: RISC-V supports various word lengths, from 16 to 128 bits, making it suitable for a broad spectrum of applications, including embedded systems, smartphones, servers, and supercomputers.

Ecosystem: RISC-V has a growing ecosystem of hardware and software tools, making it easier for developers to design and implement RISC-V-based processors and systems. This ecosystem includes compilers, simulators, development boards, and more.

Wide Industry Adoption: RISC-V has gained significant traction in various industries, including academia, research, and commercial applications. Companies and organizations are developing RISC-V-based processors and accelerators for diverse purposes.

Standardization: The RISC-V ISA is managed by the RISC-V International association, which oversees its development and ensures standardization. This helps maintain compatibility and interoperability between different implementations.



![Screenshot from 2023-09-09 06-15-32](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/142bf0d9-c983-4620-b9cd-3f8d8e0607f0)
- ### From Software Applications to Hardware
![Screenshot from 2023-09-09 06-23-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f974b6c9-427b-4f43-944e-da9699ead689)
![Screenshot from 2023-09-09 06-26-47](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d802184a-2295-4295-81a1-f79b7e9ba0e6)
![Screenshot from 2023-09-09 06-30-01](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/cdd950e9-6753-4ea1-8bcc-fee87249efb4)
![Screenshot from 2023-09-09 06-30-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8cdbb1c6-58af-496a-86e2-7e2200f86ccf)
![Screenshot from 2023-09-09 06-32-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/094a034a-0e0e-4b05-b99c-9552eb722f55)
![Screenshot from 2023-09-09 06-33-01](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ea956daf-6700-4e58-9b79-fb8ddfc07757)




      
2. SoC design and OpenLANE
   
- ### Introduction to all components of open-source digital asic design

Open-source digital ASIC (Application-Specific Integrated Circuit) design involves a range of components and tools that enable the creation of custom integrated circuits using open-source methodologies

Hardware Description Language (HDL):
        Verilog or VHDL: These are commonly used hardware description languages for specifying the behavior and structure of digital circuits. HDLs are essential for designing ASICs at the register-transfer level.

EDA Tools (Electronic Design Automation):
        Open-source EDA tools like Qflow, Magic, and Yosys are critical for designing, simulating, and verifying ASICs. They include tools for synthesis, place-and-route, and simulation.

Standard Cell Libraries:
        Open-source libraries of standard cells are collections of pre-designed logic gates, flip-flops, and other basic building blocks used in ASIC design. These libraries are essential for creating the digital logic of the ASIC.

Custom Cells:
        In addition to standard cells, custom cells may be designed for specific functions or to optimize performance in a particular ASIC projectIP (Intellectual Property):
        Open-source IP cores, or blocks of pre-designed and verified functionality, can be integrated into ASIC designs to save time and effort. These may include CPU cores, memory controllers, or other commonly used functions.

    .

Simulation and Verification Tools:
        Tools like Verilator and Icarus Verilog allow designers to simulate and verify their ASIC designs to ensure correctness and functionality.

   . Place-and-Route Tools:
        Place-and-route tools like Graywolf and Qrouter are used to physically place logic gates and routing tracks on the ASIC layout, optimizing for area, power, and timing.

Physical Design Tools:
        Tools for custom physical design, such as Magic, are essential for creating the layout of the ASIC, including metal layers, vias, and interconnections.

PDK (Process Design Kit):
        A PDK is a collection of files and data that describes the manufacturing process of the ASIC foundry. Open-source PDKs are available for certain technologies and are essential for ensuring that ASIC designs are compatible with specific fabrication processes.

Version Control System:
        Using version control systems like Git is crucial for managing the source code and design files in a collaborative open-source ASIC project.

Collaboration Platforms:
        Online collaboration platforms like GitHub and GitLab are commonly used for sharing and collaborating on open-source ASIC projects.

Documentation and Community:
        Robust documentation and a supportive community are crucial for open-source ASIC design. Online forums, wikis, and user groups provide valuable resources and assistance.

Foundry Services:
        While not strictly a component of ASIC design, access to foundry services is essential for manufacturing the final ASIC. Open-source ASIC projects often rely on shared access to foundries or services that provide affordable manufacturing options.





















![Screenshot from 2023-09-09 07-30-03](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2a1a0387-6815-4d47-9b28-f324726ba4e4)  
![Screenshot from 2023-09-09 07-30-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b2ce9eef-6a3c-4358-b504-d7b54ce921a8)
![Screenshot from 2023-09-09 06-43-40](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bb816d18-16bf-44de-a2f9-7ecbc7b24c03)
![Screenshot from 2023-09-09 06-45-28](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2d8de8b3-1cea-408b-95f0-27dbdcd5ede1)
![Screenshot from 2023-09-09 06-46-09](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6d7165ed-10e0-49d1-9c83-ae9aff5e4cdd)
![Screenshot from 2023-09-09 06-47-05](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c816f90f-96de-4738-a5bf-499f7bd9d9e8)
![Screenshot from 2023-09-09 07-34-16](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3b39394e-e429-4a70-9b45-b0f72980b228)
![Screenshot from 2023-09-09 06-49-03](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e54fcea7-42be-480a-a5d6-ffd8eec77cc7)
![Screenshot from 2023-09-09 07-34-31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e4f18abc-577b-4d5f-b0f6-0aae6aa5eccb)
![Screenshot from 2023-09-09 07-34-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/53018ea5-a708-4c76-ac49-c5bac92afaeb)
- ### Simplified RTL2GDS flow
![Screenshot from 2023-09-09 06-50-24](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ad4bef26-0f88-4170-8d06-19360aad0b7c)
![Screenshot from 2023-09-09 06-54-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/23483640-fa8e-4dc1-80b7-e65a3069d7e3)
![Screenshot from 2023-09-09 06-55-10](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/927c00cb-7b48-4565-b3b7-3282d3337a68)
![Screenshot from 2023-09-09 06-58-08](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/a19983cf-39c5-46dd-b646-62aeeeddaabb)
![Screenshot from 2023-09-09 06-57-16](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/03237927-fcc2-4cbe-ab00-9c1c2065dafe)
![Screenshot from 2023-09-09 06-58-53](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/61eb09a3-b04e-4baf-8dd1-11641bc32fa6)
![Screenshot from 2023-09-09 06-59-58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/db4f7e9b-28dd-4ac3-84e5-b24d0153f1e4)
![Screenshot from 2023-09-09 07-00-31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2f75fbe5-f039-4fb8-bcc1-d90967c24cb9)
![Screenshot from 2023-09-09 07-01-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3947b886-8f2b-4902-b27a-e03052bf1a56)
![Screenshot from 2023-09-09 07-02-13](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c23008a0-a1c0-4e67-a558-741c2283f4a9)
![Screenshot from 2023-09-09 07-03-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/af26b1b7-c8ed-4d63-b2b7-cb1d3da1ac23)
![Screenshot from 2023-09-09 07-04-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ad0a4962-74f4-4b95-a67c-b7ecb85bedc8)
- ### Introduction to OpenLANE and Strive chipsets

![Screenshot from 2023-09-09 09-56-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/74a6c5ef-984b-43cc-b52a-c81a6f822f74)
![Screenshot from 2023-09-09 09-57-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/0019dce8-b9b6-4102-b53a-e186d8041eb2)
![Screenshot from 2023-09-09 10-13-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/76bead52-2eb4-44ed-b9fe-765bf1a0147f)
![Screenshot from 2023-09-09 10-16-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7e1e519e-cf03-466c-9edd-7c34e74717be)
![Screenshot from 2023-09-09 10-19-49](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7baaa97b-3c29-4950-bbe1-622432301339)


- ### Introduction to OpenLANE detailed ASIC design flow 
![Screenshot from 2023-09-09 10-23-05](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/aac57c8c-303b-461a-bac2-9f5319aee1b6)
![Screenshot from 2023-09-09 10-23-27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ff0b2373-df5a-4580-92b7-a88c487dd07a)
![Screenshot from 2023-09-09 10-24-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/efb4bc96-c5e0-47b0-85f2-6d1b7409de76)

![Screenshot from 2023-09-09 10-25-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d7d6efb8-0152-4252-9c27-9c5d74a5f61d)
![Screenshot from 2023-09-09 10-27-43](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/53a62565-a0a0-4df6-a37c-494ee9908c4f)
![Screenshot from 2023-09-09 10-28-38](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1ea49299-82b4-4bf6-9fda-1ff3cd8f0d23)
![Screenshot from 2023-09-09 10-29-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2050278f-83ac-4e0b-826d-8a2a5eaeecaf)
![Screenshot from 2023-09-09 10-30-55](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/89db9c39-d2b6-474e-b8e4-8fa3855468f6)
![Screenshot from 2023-09-09 10-31-22](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/050c1721-ef33-440b-9be8-ae29f4d4cae6)
![Screenshot from 2023-09-09 10-33-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e5ffc34f-cf90-4454-9985-86e730600d53)
![Screenshot from 2023-09-09 10-34-00](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/267af47b-d5f1-4f84-a7ee-c15f2c54630f)
![Screenshot from 2023-09-09 10-34-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/590931b7-1c65-430e-8158-13641ce78cb8)
![Screenshot from 2023-09-09 10-35-53](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e6d17ffb-1504-402c-9cf8-ab1de64043bf)
![Screenshot from 2023-09-09 10-36-10](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/08a6587a-b2f8-4b07-9214-a61df3cf02ad)






3. Get familiar to open-source EDA tools

Open-source Electronic Design Automation (EDA) tools play a crucial role in semiconductor and digital design. 
    
Qflow: Qflow is a complete open-source digital synthesis and place-and-route toolchain that supports FPGA and ASIC design. It includes tools like Graywolf and Magic for layout.

Yosys: Yosys is a powerful open-source RTL synthesis tool. It can synthesize Verilog code into netlists and perform various optimizations, making it a key component in ASIC design.

 Magic: Magic is a layout tool used for creating custom integrated circuit layouts. It is often used in conjunction with other EDA tools for physical design.

Icarus Verilog: Icarus Verilog is an open-source Verilog simulation and synthesis tool. It allows designers to simulate and verify digital circuits written in Verilog.

 OpenROAD: OpenROAD is an open-source initiative for ASIC and FPGA design that focuses on automating the design flow, including place-and-route, optimization, and power analysis.

 Xschem: Xschem is an open-source electronic schematic capture tool, which is useful for designing the logical structure of digital circuits.

 KiCad: While primarily a PCB design tool, KiCad includes a schematic editor and is often used for digital circuit design as well.

 GHDL: GHDL is an open-source VHDL simulator that allows designers to simulate VHDL code for ASIC and FPGA designs.

Verilator: Verilator is a fast and free Verilog/SystemVerilog simulator. It is commonly used for high-level simulation of digital circuits.

FreePDK: While not a tool per se, FreePDK is an open-source Process Design Kit that defines the manufacturing process parameters for specific foundries, aiding in ASIC design compatibility.


   - OpenLANE Directory structure in detail


    ![VirtualBox_PES_physical_design_09_09_2023_12_41_45](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/0b10a680-5228-48d9-9c51-54482cfe4434)
![VirtualBox_PES_physical_design_09_09_2023_12_42_38](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/334584a0-022f-4a19-86b6-bede9905a115)
![VirtualBox_PES_physical_design_09_09_2023_12_56_32](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4efe581e-d324-415e-8f3a-cd3879239809)


   - Design Preparation Step

![VirtualBox_PES_physical_design_09_09_2023_13_13_16](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3f1994c9-cece-40fe-b0c1-1f3b18aa5a9d)

![VirtualBox_PES_physical_design_09_09_2023_13_17_33](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3addbae5-2509-4506-bd7c-3f361e7c3b15)

![VirtualBox_PES_physical_design_09_09_2023_13_09_55](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/754e2dac-b1af-48cf-a580-787128371e9e)

![VirtualBox_PES_physical_design_09_09_2023_13_22_05](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d432b3aa-0935-406c-a4d2-85ec2caaa87b)



     
   - Review files after design prep and run synthesis

![VirtualBox_PES_physical_design_09_09_2023_14_18_21](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d33d509e-261d-4c96-85a0-1049b5bb76b7)
![VirtualBox_PES_physical_design_09_09_2023_14_18_43](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/271d6aa4-e4a6-4299-af29-01e1d059b52b)
![VirtualBox_PES_physical_design_09_09_2023_14_23_49](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6aee9d70-bbd8-4a1b-be5d-892a381df571)
![VirtualBox_PES_physical_design_09_09_2023_14_24_16 (copy)](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5b26da08-c581-4992-9717-f30bd0052508)
![VirtualBox_PES_physical_design_09_09_2023_14_34_27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d8ccba8e-9346-4f0e-bc95-4404eca91147)


</details>



<details>
<summary> WEEK-3 -> Day - 2 </summary>
    
# Good floorplan vs bad floorplan and introduction to library cells 


Chip floor planning is a critical step in the design of integrated circuits (ICs) where you determine the placement of various functional blocks and components on the silicon die. Two essential considerations in chip floor planning are the utilization factor and the aspect ratio:

Utilization Factor:

The utilization factor, often denoted as UF, is a measure of how efficiently the available silicon area is being used on the chip. It is typically calculated as the ratio of the area occupied by the active components (such as logic gates, memory cells, and analog circuits) to the total available silicon area.

 A high utilization factor indicates that a significant portion of the chip area is used for active components, maximizing the functionality of the chip. Conversely, a low utilization factor may imply that there is unused or wasted space on the chi.

 Designers aim to strike a balance between maximizing utilization while ensuring that the chip's physical layout meets performance, power, and manufacturability requirements.

Aspect Ratio:

 The aspect ratio refers to the ratio of the chip's width to its height (or vice versa) in a two-dimensional layout. It is a crucial consideration because it impacts the chip's overall shape and dimensions.

The aspect ratio can have implications for the chip's manufacturability, as it affects how it fits into a wafer and how efficiently it can be manufactured in a semiconductor fabrication facility (fabs).

In some cases, an aspect ratio that is too extreme (very tall and narrow or very wide and flat) can lead to manufacturing challenges or inefficiencies. Designers aim to choose an aspect ratio that is compatible with the manufacturing process and chip size constraints.

## 1. Chip Floor planning considerations
- ### Utilization factor and aspect ratio
Chip floor planning is a critical step in the design of integrated circuits (ICs) where you determine the placement of various functional blocks and components on the silicon die. Two essential considerations in chip floor planning are the utilization factor and the aspect ratio:

Utilization Factor:

The utilization factor, often denoted as UF, is a measure of how efficiently the available silicon area is being used on the chip. It is typically calculated as the ratio of the area occupied by the active components (such as logic gates, memory cells, and analog circuits) to the total available silicon area.

 A high utilization factor indicates that a significant portion of the chip area is used for active components, maximizing the functionality of the chip. Conversely, a low utilization factor may imply that there is unused or wasted space on the chi.

 Designers aim to strike a balance between maximizing utilization while ensuring that the chip's physical layout meets performance, power, and manufacturability requirements.

Aspect Ratio:

 The aspect ratio refers to the ratio of the chip's width to its height (or vice versa) in a two-dimensional layout. It is a crucial consideration because it impacts the chip's overall shape and dimensions.

The aspect ratio can have implications for the chip's manufacturability, as it affects how it fits into a wafer and how efficiently it can be manufactured in a semiconductor fabrication facility (fabs).

In some cases, an aspect ratio that is too extreme (very tall and narrow or very wide and flat) can lead to manufacturing challenges or inefficiencies. Designers aim to choose an aspect ratio that is compatible with the manufacturing process and chip size constraints.

![Screenshot from 2023-09-09 17-05-21](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/a6b04b88-19c9-4bf4-b50c-c66b82a97f83)
![Screenshot from 2023-09-09 17-08-01](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f4b2e552-ccd6-4f1a-85f2-fff1659e7bea)
![Screenshot from 2023-09-09 17-08-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7006410d-f0fb-451c-9e88-575f2f5549c5)
![Screenshot from 2023-09-09 17-09-27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/355baa94-6ad0-4501-9c35-7406f43fc1c2)
![Screenshot from 2023-09-09 17-10-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3f8e1c2e-4089-45f8-b1b5-186b0969adfb)
![Screenshot from 2023-09-09 17-11-36](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4ccebca1-f5c7-453a-bb0d-f1f77a676b02)
![Screenshot from 2023-09-09 17-15-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f4dbf488-9808-4a73-8042-e39d7434fe19)
![Screenshot from 2023-09-09 17-16-26](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5d032cf3-79aa-4d43-bb8a-d4bf65d3b120)
![Screenshot from 2023-09-09 17-17-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8286b4c6-787d-45bf-9f4e-0c4645b41283)
![Screenshot from 2023-09-09 17-27-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/84fdc0b9-e7ff-4a33-8825-d36e936d17a0)
- ### Concept of pre-placed cells
![Screenshot from 2023-09-09 17-27-47](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7326d5c8-4fcd-4d4e-aa60-79a64b6e743a)
![Screenshot from 2023-09-09 17-30-01](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d9596c35-dbbe-4d5f-97ac-8eb9e9575863)
![Screenshot from 2023-09-09 17-31-16](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/32c864ba-de42-48e9-a35f-a18d2ab41d46)
![Screenshot from 2023-09-09 17-31-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/40f12baa-f590-4a57-af24-245145946b65)
![Screenshot from 2023-09-09 17-36-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/28b67020-01c1-4833-8414-b51dd858455c)
- ### De-coupling capacitors


Decoupling capacitors, often referred to as bypass capacitors, are essential components in electronic circuits, particularly in digital and mixed-signal designs. Their primary purpose is to stabilize and improve the performance of integrated circuits (ICs), such as microprocessors, digital signal processors, and other active components. Here's a brief overview of decoupling capacitors:

Function:

Noise Suppression: Decoupling capacitors help suppress high-frequency noise and voltage fluctuations in a power supply network. When an IC switches or draws current suddenly, it can create voltage spikes or "noise" on the power lines. Decoupling capacitors provide a local energy source to counteract these voltage fluctuations.

Voltage Regulation: They help maintain a stable and constant voltage level at the power supply pins of ICs. This is crucial for preventing malfunctions, reducing the risk of electromagnetic interference (EMI), and ensuring reliable circuit operation.



  
![Screenshot from 2023-09-09 17-49-54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/90ddb5ea-0705-495a-943a-4f18faee94f3)
![Screenshot from 2023-09-09 17-50-29](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5eda99f0-31fa-4d80-9115-0db3f2de834f)
![Screenshot from 2023-09-09 17-50-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/06ea0d8d-99df-4e5d-8193-17986d795e83)
![Screenshot from 2023-09-09 17-54-13](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b8e21e2c-c497-4d18-8a71-230a85b37d91)
![Screenshot from 2023-09-09 17-54-40](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/460807a7-f1a0-4879-b7b7-c78a5d267d60)
![Screenshot from 2023-09-09 17-56-27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f27dab67-a579-4fcb-8d84-415ecb7faac3)
![Screenshot from 2023-09-09 17-58-49](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/61a310d2-eb5a-4776-93d6-e69daad3e199) 
- ### Power planning
Power planning is the process of managing and optimizing electrical power resources to meet the demands of a facility while aiming for efficiency and sustainability. It involves analyzing power requirements, ensuring infrastructure capacity, enhancing energy efficiency, and considering future growth and environmental impact. Power planning is crucial for reliable and efficient power supply in various settings.






![Screenshot from 2023-09-09 18-01-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bde6a89f-1814-446e-8e0d-b83767c44984)
![Screenshot from 2023-09-09 18-07-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6284c266-648b-4272-8afc-436430428fc9)
![Screenshot from 2023-09-09 18-10-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/56bcf7fd-b5d7-48d2-bb63-123729a22b1a)
![Screenshot from 2023-09-09 20-47-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/66909f0f-3d0a-457d-b68a-0a9a9c447df7)
![Screenshot from 2023-09-09 20-48-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ef5d3088-e56d-461f-9ac1-5e27a1c6daf6)
![Screenshot from 2023-09-09 21-23-47](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/68aa57e7-b8ed-42ed-8b1c-fb7a2f7f6bd6)
![Screenshot from 2023-09-09 21-25-22](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/a8b71c86-3ca3-49c0-8d93-2fda9b9cce5d)
![Screenshot from 2023-09-09 21-26-49](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e987d3ec-9eed-4493-bb47-71e9ec8296ce)
![Screenshot from 2023-09-09 21-27-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/a1534d99-c024-44bb-a8e8-18657d145dff)
- ### Pin placement and logical cell placement blockage

1. Pin Placement:

    Pins are points on the IC where it interfaces with the outside world. These can include input pins (for receiving signals), output pins (for sending signals), and power/ground pins (for supplying power and ground connections).
    Pin Placement involves determining the locations and assignments of these pins on the IC's physical layout. Proper pin placement is crucial for ensuring the IC can be connected to other components on a circuit board.
    Pins need to be strategically placed to minimize wirelength (distance between pins), optimize signal integrity, and meet electrical and timing requirements.

2. Logical Cell Placement:

    In the context of digital IC design, an IC is composed of logical cells, such as gates, flip-flops, and other digital components. Logical cell placement involves determining the positions of these cells within the IC's layout.
    Proper logical cell placement is essential for achieving optimal performance, power consumption, and ease of routing during later stages of design.
    The placement process should consider factors like minimizing signal delays, reducing congestion, and meeting area constraints.


![Screenshot from 2023-09-09 21-52-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b7c1eeb7-e8f1-4c56-a616-954913a75a36)
![Screenshot from 2023-09-09 21-54-58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f058f48b-2b68-4c92-ae8d-df14e73d3ab9)
![Screenshot from 2023-09-09 21-57-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5f297541-ed9d-447a-9f63-7d4f450e2cfa)
![Screenshot from 2023-09-09 21-58-19](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7b74b091-194c-4bed-b54a-72f58ed7d8ab)
![Screenshot from 2023-09-09 21-59-04](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/033bf491-3c59-4064-ad19-f870b581956b)
![Screenshot from 2023-09-09 22-01-04](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/554ff639-61a1-428c-b87c-98b2e3b61551)
![Screenshot from 2023-09-09 22-01-13](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/07b99ebf-23c1-408b-ad4c-97d8b694e428)
![Screenshot from 2023-09-09 22-04-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4c724b84-67fb-46a7-9615-ac38955722c4)
![Screenshot from 2023-09-09 22-04-41](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/14f1fa11-c58b-49c9-bf7e-6aee538776bb)
- ### Steps to run floorplan using OpenLANE

![VirtualBox_PES_physical_design_09_09_2023_14_34_27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d341fc94-3035-4493-9df8-092253095dda)
![VirtualBox_PES_physical_design_10_09_2023_13_10_29](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c57a8377-e68a-40d3-b46f-263386ff547f)


![VirtualBox_PES_physical_design_10_09_2023_13_04_34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6a3b2c7e-e697-418b-b004-0127074357c4)

![VirtualBox_PES_physical_design_10_09_2023_13_05_12](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2c38e324-dd85-4332-b058-bf5be2e8fc0b)

![VirtualBox_PES_physical_design_10_09_2023_13_06_45](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ccb7e80a-6883-40c7-b85d-7408fa747519)

![VirtualBox_PES_physical_design_10_09_2023_13_08_50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e94998c3-9433-4eb4-b913-e8fed09c326e)
![VirtualBox_PES_physical_design_10_09_2023_13_15_11](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/98eb1e12-c61c-469e-bc79-1c591c06fd5d)


      
- ### Review floorplan files and steps to view floorplan
![VirtualBox_PES_physical_design_10_09_2023_13_23_34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bbb4cb8c-1171-4124-8d61-9c27bc37c7cb)
![VirtualBox_PES_physical_design_10_09_2023_13_29_05](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/abef7228-c8e3-4e7e-b357-2ade0d8e56c6)

![VirtualBox_PES_physical_design_10_09_2023_13_35_11](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e9c9fb49-4cc0-4243-9c90-9e34fc83cfa3)




- ### Review floorplan layout in Magic
![VirtualBox_PES_physical_design_10_09_2023_13_35_11](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/dea63558-5ff9-4ed0-85a9-99c21a3a66fb)
![VirtualBox_PES_physical_design_10_09_2023_13_36_34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/397d08d6-2710-4850-b98d-da5ccef10d60)
![VirtualBox_PES_physical_design_10_09_2023_13_43_39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/739be89f-2952-4325-94be-9bfd106c3386)
![VirtualBox_PES_physical_design_10_09_2023_13_50_58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/910e6c03-2c5d-4858-9e70-2b522c9a8352)
![VirtualBox_PES_physical_design_10_09_2023_13_52_52](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/58a7e660-6df5-45d7-88a9-63eaa4bb1fe6)


    
      
## 2. Library Binding and Placement
- ### Netlist binding and initial place design
![Screenshot from 2023-09-15 05-29-12](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/fc6cd943-ee51-42f8-bb30-f0a2f146c9af)
![Screenshot from 2023-09-15 05-30-44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c883e3a5-23b5-4b2e-962d-a2a9ef384644)
![Screenshot from 2023-09-15 05-33-11](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/88b34d62-ded2-44db-998c-da2713212bee)
![Screenshot from 2023-09-15 05-34-55](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/25ab9bba-7878-486a-91fa-721b21adfb99)
![Screenshot from 2023-09-15 05-38-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6f697327-3547-49b8-85a3-43e3d269d18d)      
- ### Optimize placement using estimated wire-length and capacitance
![Screenshot from 2023-09-15 05-43-07](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1c23eece-63d6-4ab0-a604-31878b7b02c9)
![Screenshot from 2023-09-15 05-44-24](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f86aec2b-4541-4527-9601-c05d845a6174)
![Screenshot from 2023-09-15 05-51-44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/30a4081b-fd70-4001-8c58-c7fbf7d72408)
![Screenshot from 2023-09-15 05-52-36](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f7ab42c0-60f7-484f-a5af-0002fabf5055)     
- ### Final placement optimization
![Screenshot from 2023-09-15 06-00-52](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/dfcdeb5d-8a21-4bc1-bcee-b1d875dcda8e)
![Screenshot from 2023-09-15 06-10-35](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/50806cc0-6418-4469-89f8-eaeb2f42dff3)
![Screenshot from 2023-09-15 06-13-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b7084e70-2073-4e59-a2fd-3ef8a0776fa9)      
- ### Need for libraries and characterization
![Screenshot from 2023-09-16 07-08-44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ebfba563-6498-4421-b724-b93183c27de2)
![Screenshot from 2023-09-16 07-09-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c16d9c4d-fd10-4a60-9783-f06e6fe78923)
![Screenshot from 2023-09-16 07-09-48](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/57b04d20-a130-4edc-b73d-e1ca6ca9f8f8)
![Screenshot from 2023-09-16 07-10-16](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e2f09f14-49d7-4e5d-8f37-ab4299a2e374)
![Screenshot from 2023-09-16 07-12-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/384369d2-42a3-4250-903e-ecfd69d5f7b9)
![Screenshot from 2023-09-16 07-13-31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/da6db991-9a6c-4303-ab5e-d35c529e5edb)
![Screenshot from 2023-09-16 07-15-12](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b85e6b61-4d40-4219-9d4f-adb2708e53df)
![Screenshot from 2023-09-16 07-16-56](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/443bd744-d3d1-4176-a525-c9b24864ca76)
- ### Congestion aware placement using RePlAce
![VirtualBox_PES_physical_design_16_09_2023_10_19_27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ef889f7b-4591-47fc-b88a-3ff8d9f8a3f9)
![VirtualBox_PES_physical_design_16_09_2023_10_36_26](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/712f4acd-4bcd-4287-b47b-4e7d4dc1003c)
![VirtualBox_PES_physical_design_16_09_2023_10_44_22](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c9d5e5ad-7b7f-4423-807b-91d8c33266de)
![VirtualBox_PES_physical_design_16_09_2023_10_44_38](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8b100217-ea8b-4355-a1db-e0fd8dfee340)
## 3. Cell design and characterization flows
- ### Inputs for cell design flow
![Screenshot from 2023-09-16 16-18-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ed0d99d4-0412-4e50-ae97-34e5d5513039)
![Screenshot from 2023-09-16 16-21-11](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ea6caf18-caed-42a2-8794-059480556b91)
![Screenshot from 2023-09-16 16-37-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f88a418a-eb13-4ba4-80af-6a1774b8670c)
![Screenshot from 2023-09-16 16-42-57](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/22cdf526-6a87-4001-93b7-0c961ccedc90)
![Screenshot from 2023-09-16 16-44-13](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/40bcaecf-9419-49a0-81a4-e3bba85d9936)      
- ### Circuit design step
![Screenshot from 2023-09-16 16-48-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4f1e8cb1-82f5-4401-873b-a0b60ad9ab13)
![Screenshot from 2023-09-16 16-50-07](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7a1d96ab-86a0-4c54-a247-b07c211951df)
![Screenshot from 2023-09-16 16-50-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/115028a8-d6b4-42e5-bbe2-7f3b26386193)
![Screenshot from 2023-09-16 16-51-08](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bf6f777f-1f69-4cdd-a81e-360f1da71677)
![Screenshot from 2023-09-16 16-52-02](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1c1cabcd-7e15-4bd1-a8da-5d341db01e42)
![Screenshot from 2023-09-16 16-55-31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/cc72af8e-25a1-4010-87e4-da5b3996ef56)
- ### Layout design step
![Screenshot from 2023-09-16 17-04-21](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3c7a2ffd-31bc-400e-8060-846c3e9e36f8)
![Screenshot from 2023-09-16 17-05-02](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4c216dde-065c-4334-b220-dba3ac97a28c)
![Screenshot from 2023-09-16 17-05-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/45a800fb-d061-4f44-b7f5-f9a94340f1d0)
![Screenshot from 2023-09-16 17-07-53](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/08180396-e554-4d6f-ab77-b90766064760)
![Screenshot from 2023-09-16 17-08-42](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/860f7aab-7f90-4fd6-b214-60285edc26dc)
![Screenshot from 2023-09-16 17-09-24](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/988a4747-ea42-486e-841a-fece00d6a2fe)      
![Screenshot from 2023-09-19 10-17-12](https://github.com/Abhi9108865162/pes_pd/assets/141741065/c1adf609-4a0d-47dc-b2c4-4df823b96d82)



- ### Typical characterization flow
![Screenshot from 2023-09-16![Uploading Screenshot from 2023-09-19 10-17-12.png…]()
 17-12-44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/503e8d02-899e-4b98-9ccd-ae824ecac670)
![Screenshot from 2023-09-16 17-12-57](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2eb7aed4-dd89-496c-ad0f-7ca14bdb2809)
![Screenshot from 2023-09-16 17-15-44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4599d25d-a8d4-4899-9352-aa5154cfc46f)
![Screenshot from 2023-09-16 17-16-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/adf857a4-7e8f-4be0-81f8-ac9109c9ff60)
![Screenshot from 2023-09-16 17-16-41](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/196ea324-a945-4312-8529-c65703879bd6)
![Screenshot from 2023-09-16 17-16-48](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d700337c-5670-4243-97ef-7c2c4534522f)
![Screenshot from 2023-09-16 17-17-54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/496c3864-f17a-47ca-8f62-12dc51fa89eb)
![Screenshot from 2023-09-16 17-18-04](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/557940cd-953f-452e-9c80-5506d67e6c53)
![Screenshot from 2023-09-16 17-18-57](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4b6235fe-dc57-4dcd-8455-7a63774c6e0c)


## 4. General timing characterization parameters
- ### Timing threshold definitions

  

    Clock Signals: Timing thresholds are commonly applied to clock signals and other critical paths in a digital circuit. A clock signal has a defined period (time between clock edges), and the timing threshold specifies how much deviation from this period is allowed.

    Clock Skew: Timing thresholds can also be used to account for clock skew, which is the variation in arrival times of the clock signal at different parts of the circuit. The threshold determines the acceptable amount of skew.

    Setup and Hold Times: For flip-flops and other sequential elements, timing thresholds are used to define setup and hold times. The setup time is the minimum time before the clock edge at which the input data must be stable, while the hold time is the minimum time after the clock edge during which the data must remain stable.

    Propagation Delay: Timing thresholds can specify the maximum allowable propagation delay for signals to travel from one point in the circuit to another. This helps ensure that signals arrive at their destinations within the required time window.

    Critical Paths: Critical paths in a circuit are those paths that have the tightest timing requirements. Timing thresholds are used to analyze and optimize these critical paths to meet the desired performance goals.

    Clock Frequency: Timing thresholds may be tied to the clock frequency of the circuit. For example, if a design is intended to operate at a certain clock frequency, the timing threshold may specify the maximum clock period allowed.

![Screenshot from 2023-09-16 17-22-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f141ec1c-fb44-46c2-a000-0bf4b74e237d)
![Screenshot from 2023-09-16 22-42-00](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/18c69769-1763-4a91-8c1f-9a8f6298ad28)
![Screenshot from 2023-09-16 22-42-08](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/74d90f29-5fcc-4fc4-ad6e-14c689b50f77)
![Screenshot from 2023-09-16 22-42-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bac0c216-febc-48cd-9daf-491625286e98)
![Screenshot from 2023-09-16 22-43-59](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/121df024-7e82-4a24-94f7-5aa8a308e8c7)
![Screenshot from 2023-09-16 22-44-53](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6af87c0b-fe3e-4866-a6c3-b36873fa09ec)
![Screenshot from 2023-09-16 22-45-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c2ed4515-2ff3-4d91-a830-83fc297be545)
![Screenshot from 2023-09-16 22-45-42](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/adee4b1f-8020-4d52-ad1d-68575020082b)     
- ### Propagation delay and transition time
![Screenshot from 2023-09-16 22-52-19](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/47727743-2d2a-40f5-9352-1f9eb6af3653)
![Screenshot from 2023-09-16 22-52-56](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f968eb29-95d8-46f5-83c3-5d2b31488ff8)
![Screenshot from 2023-09-16 22-55-07](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/18585568-0494-4b0a-b4fd-a62e772a76b5)
![Screenshot from 2023-09-16 22-55-21](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/33503f6a-00f7-4b20-87b4-6fccd304179a)
![Screenshot from 2023-09-16 22-57-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8001149a-7ebb-4c0a-9366-d1ad5e1b2da5)
![Screenshot from 2023-09-16 22-58-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4ee86602-fcb0-4851-9972-adff4f38f143)
![Screenshot from 2023-09-16 22-58-36](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6e860fe3-36b8-4b01-be2e-fa58459ac5a8)
![Screenshot from 2023-09-16 23-00-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/0a0a3ac5-08f4-4211-897b-120894dada9c)
</details>




<details>
<summary> WEEK-3 -> Day - 3 </summary>

# Design library cell using Magic Layout and ngspice characterization 
Designing the Library Cell with Magic Layout:

Install Magic: Make sure you have Magic Layout installed on your system.

Define the Cell: Using Magic, you'll define the layout and schematic of your library cell. This can include logic gates, flip-flops, or other custom digital or analog components.

Layout Design: Create the physical layout of the cell, specifying the positions of transistors, interconnections, and metal layers. Ensure that the layout adheres to design rules and constraints for the semiconductor technology you're using.

Schematic Capture: Create a schematic representation of the cell, specifying its electrical connections and component properties.

Extraction: Use Magic to extract parasitic capacitance, resistance, and other electrical properties from the layout. This information is crucial for accurate electrical characterization.



## 1. Labs for CMOS inverter ngspice simulations

* CMOS Inverter
* Supply voltage
Vdd vdd 0 DC 5V
* Input pulse
Vin in 0 PULSE (0 5V 0 0.1ns 0.1ns 10ns 20ns)
* CMOS transistors
Mn out in 0 0 nMOS W=1u L=180n
Mp out in vdd vdd pMOS W=1u L=180n
* Load capacitance
Cload out 0 10f
* DC Analysis
.dc VIN 0V 5V 0.1V
.control
run
plot out
.endc

- ###  IO placer revision 
![VirtualBox_PES_physical_design_17_09_2023_08_02_15](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5320d97f-5c0f-4159-ba65-a2ffe7b96892)
![VirtualBox_PES_physical_design_17_09_2023_08_18_53](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/910e6c0a-92ae-4e8b-a6ad-8114f06db3e0)
![VirtualBox_PES_physical_design_17_09_2023_08_18_24](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4bb9fd09-7e70-41da-bd7b-d01439bd5998)
![VirtualBox_PES_physical_design_17_09_2023_08_18_44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bd004446-366c-460d-8793-56ac1f4a1fbf)
![VirtualBox_PES_physical_design_17_09_2023_08_22_31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c8745a83-6a81-4435-bb78-cac12f090de7)
- ### SPICE deck creation for CMOS inverter 
![Screenshot from 2023-09-17 08-27-54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/584f6131-92bd-44ca-9de4-e33ee3a47932)
![Screenshot from 2023-09-17 09-09-33](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/15ddd21e-9062-4e84-9225-eb7d990a3c92)
![Screenshot from 2023-09-17 09-12-02](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/87640242-6b83-4b8c-b7f7-0eb4a85854d6)
![Screenshot from 2023-09-17 09-13-10](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4aabf6ca-ec5f-4d06-944c-4395ae205801)
- ### SPICE simulation lab for CMOS inverter
![Screenshot from 2023-09-17 09-25-41](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3efe7dd4-46b8-41ca-b0e2-6529994dfb57)
![Screenshot from 2023-09-17 09-26-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8a1e8e33-bb01-4ce2-a136-499dc8fbcf8b)
![Screenshot from 2023-09-17 09-27-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2fb6869b-e374-4a4c-a0ca-5bb0bce89fb5)
![Screenshot from 2023-09-17 09-27-43](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/04a7979a-1d85-4096-83ae-de9a6934c8fb)
![Screenshot from 2023-09-17 09-28-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8063f03f-6a7c-40fc-9392-2f5a9c908048)
![Screenshot from 2023-09-17 09-29-19](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7ccb2542-a80f-4e18-9610-26d36517e1f6)
![Screenshot from 2023-09-17 09-30-48](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/30c40b50-80c8-4be0-9329-ff4417a784ca)
![Screenshot from 2023-09-17 09-31-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/af9a82ae-88b8-47cc-9870-5b1cdc1502ed)
![Screenshot from 2023-09-17 09-31-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/a7fa7857-a16e-413f-af51-81ecd1b6f125)
![Screenshot from 2023-09-17 09-31-52](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ab851d1d-53ad-45fe-aaeb-109488c07005)
![Screenshot from 2023-09-17 09-32-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1b4a020d-4eff-442d-9575-fc39ba92c8c2)
![Screenshot from 2023-09-17 09-32-49](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1d3597e7-0409-4b5c-a936-d6c89c7aea65)
![Screenshot from 2023-09-17 09-33-02](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b099b3ba-9124-4961-8494-b1003257e10d)
![Screenshot from 2023-09-17 09-33-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5a4c7279-0cb3-4f12-b5c1-ec846eaf339b)
![Screenshot from 2023-09-17 09-33-59](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/41f13c9a-c6ed-4c97-8b45-6edf908a5a1b)
- ### Switching Threshold Vm 
![Screenshot from 2023-09-17 09-45-44](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/94c0bd49-4cd9-4ff7-910e-ab6ca85af0bc)
![Screenshot from 2023-09-17 09-46-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/448cf589-d97f-4a5e-8fb3-b8ad71428a32)
![Screenshot from 2023-09-17 09-47-19](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/eecf1403-7281-4173-b01f-9e0bc54840ec)
![Screenshot from 2023-09-17 09-47-58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/07fd6867-a47c-482a-95fa-73bf9c642a7c)
![Screenshot from 2023-09-17 09-49-43](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/51e18153-d0ef-4388-9fe2-545b81e49411)
![Screenshot from 2023-09-17 09-50-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/9451779a-c05c-4849-8f7e-6aaff4de6279)
![Screenshot from 2023-09-17 09-55-36](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/14574bdf-24f3-42b9-a014-7b8dd598b30f)
- ### Static and dynamic simulation of CMOS inverter


Static Simulation:

Static simulations focus on the DC behavior of the CMOS inverter, which means analyzing the circuit when the inputs and outputs have reached a steady state (i.e., no changes in voltage over time).

DC Analysis:
        DC analysis calculates the DC operating points (bias points) of the CMOS inverter, such as the output voltage (VOH), output current (IOH), input voltage (VIN), and input current (IIN) when no signal is changing.
        Perform a DC sweep analysis by varying the input voltage (VIN) from 0 to VDD to observe the transfer characteristic or voltage transfer curve of the inverter.

Transient Analysis (Optional):
        In some cases, you may want to perform a transient analysis with a step input to observe how the inverter transitions from one logic state to another.
        Set an initial condition and apply a step input to the inverter input to observe the transient response.

Results Analysis:
        Analyze the DC and transient simulation results to understand the inverter's voltage transfer characteristics, including the threshold voltage, noise margins, and the speed of logic transitions.








Dynamic Simulation:

Dynamic simulations focus on the AC behavior of the CMOS inverter, particularly its response to time-varying signals. This helps you understand the inverter's speed, frequency response, and signal propagation.

AC Analysis:
        Perform AC analysis to determine the inverter's frequency response.
        Sweep the frequency of the input signal and plot the gain (output voltage divided by input voltage) and phase response of the inverter.
        Analyze the bandwidth, gain, and phase margins to assess the inverter's performance in signal processing applications.

Transient Analysis (Pulse or Step Input):
        Apply a transient input signal, such as a pulse or step, to the inverter's input.
        Observe the inverter's response in terms of signal propagation delay, rise/fall times, and overshoot/undershoot.
        Measure the time it takes for the output to reach a certain percentage of its final value (e.g., 10% to 90%).

Power Consumption Analysis:
        Calculate and analyze the power consumption of the CMOS inverter under dynamic conditions, considering both dynamic power (due to switching) and static power (leakage).

Noise Analysis (Optional):
        Simulate noise sources and analyze the impact of noise on the inverter's dynamic behavior.

Results Analysis:
        Interpret the results to understand the inverter's dynamic behavior, including its response to different input signals, its speed, and its ability to process high-frequency signals.


![Screenshot from 2023-09-17 09-59-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3356dd2f-3591-4255-9170-9d06bb9a2f24)
![Screenshot from 2023-09-17 10-00-35](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2c5f4bbb-292e-4691-96cd-515d6a907db6)
![Screenshot from 2023-09-17 10-01-38](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/93236596-b281-4544-9b18-c82f7c79c156)
![Screenshot from 2023-09-17 10-01-40](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ee1f3362-2f91-4aa1-9965-938c35cbbb53)
![Screenshot from 2023-09-17 10-01-53](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/652e08cb-5d08-440b-b739-396e1403082a)
![Screenshot from 2023-09-17 10-02-08](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f7c17070-9045-4ca7-8006-eed5773dca67)
![Screenshot from 2023-09-17 10-02-15](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d8017a38-56dd-4426-b326-588161e2bdf5)
![Screenshot from 2023-09-17 12-47-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/21c6665d-d089-4e50-bf18-a7af527b0a79)
![Screenshot from 2023-09-17 12-48-15](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b5f7b653-3771-4588-b9ae-247dd6a2dcd8)
![Screenshot from 2023-09-17 12-48-47](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1cfb6048-873b-4ce8-b59b-ae7f7bf09214)
![Screenshot from 2023-09-17 12-50-00](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4e7120b2-1a73-4163-b22e-047c47a7ef74)
![Screenshot from 2023-09-17 12-50-04](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7362037c-e188-49f8-a90d-6aa4faa5be1f)
![Screenshot from 2023-09-17 12-50-09](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5c50c24b-40e6-4555-9154-6aabcfed95a4)
![Screenshot from 2023-09-17 12-50-32](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6846c8d5-de66-488c-97fd-433dc5097ab6)
![Screenshot from 2023-09-17 12-50-35](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b511ec53-2ba4-4229-bcc8-1eeae4e5d8a2)
![Screenshot from 2023-09-17 12-51-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/eba7801e-d02a-4c88-af20-4a3d1ad3f74f)
![Screenshot from 2023-09-17 12-51-20](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/360bf410-e0c4-4945-bca3-f323a954df5d)
![Screenshot from 2023-09-17 12-53-00](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d36e133b-5e8f-40aa-a241-7d5ea640dea1)
![Screenshot from 2023-09-17 12-54-20](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5e654017-c92c-411b-8582-927bbe84e1f0)
- ### Lab steps to git clone vsdstdcelldesign
![VirtualBox_PES_physical_design_17_09_2023_13_10_41](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5c9ba5e4-f649-4f13-8264-bf0c57c5c318)
![VirtualBox_PES_physical_design_17_09_2023_13_15_06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/15c54af6-eaf7-4c6e-8518-24fce048e895)
![VirtualBox_PES_physical_design_17_09_2023_13_17_52](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ec4521f6-5e1c-4a91-a1e0-3e28deaa32c7)
![VirtualBox_PES_physical_design_17_09_2023_13_17_45](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/43e4c943-17a8-4533-8370-5c67f6618bfb)

## 2. Inception of Layout Â CMOS fabrication process

The inception of layout in the CMOS fabrication process involves the following steps:

Specification and Design: Define the circuit's functionality and performance requirements.

Transistor Sizing: Determine transistor sizes based on speed and power considerations.

Logic Synthesis: Convert high-level logic into gate-level netlists.

Cell Library Selection: Choose standard cell libraries optimized for manufacturing.

Floorplanning: Allocate chip space for functional blocks and components.

Placement: Position individual standard cells within the allocated space.

Routing: Create physical connections between components using metal and polysilicon layers.

Design Rule Checking (DRC): Ensure layout adheres to manufacturing rules and guidelines.
   
- ### Create Active regions
   Create active regions in a CMOS integrated circuit:

    Substrate: Start with a silicon wafer.
    Oxide Growth: Grow a silicon dioxide (SiO2) insulator layer.
    Photoresist: Apply and pattern photoresist.
    Etching: Remove exposed oxide to expose silicon.
    Implantation: Introduce dopant atoms for transistors.
    Annealing: Heat treat for dopant activation.
    Gate Oxide: Grow an insulating gate oxide layer.
    Polysilicon: Deposit polysilicon for gate electrodes.
    Gate Patterning: Define gate electrode patterns.
    Optional Doping: Modify polysilicon properties if needed.

  
![Screenshot from 2023-09-17 14-02-52](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/51dc8d17-830c-4046-a3ba-ad9c33fab963)
![Screenshot from 2023-09-17 14-22-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/eac917c2-0bfb-4dc8-9bb1-26f269ee578a)
![Screenshot from 2023-09-17 14-24-48](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8b35eba8-a0a8-466c-b459-26f2c6dce6fa)
![Screenshot from 2023-09-17 14-24-54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2a92feeb-5345-497a-9f6f-b060dc9d2371)
![Screenshot from 2023-09-17 14-28-51](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/31dc95b9-0864-43ff-911e-e311ebf4a7c9)
![Screenshot from 2023-09-17 14-29-02](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/db3c0927-b86c-452f-9329-6325548190e4)
![Screenshot from 2023-09-17 14-30-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f4a9c873-7953-40a8-95fc-44f262877693)
![Screenshot from 2023-09-17 14-31-16](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b8eddfa3-3fc8-47e4-9274-0e9f15bf89a3)
![Screenshot from 2023-09-17 14-31-22](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/4c2fa1a8-ae42-43c4-989f-4c1ae38c256e)
![Screenshot from 2023-09-17 14-31-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/382c50d4-d9d1-47ef-a365-075992fce5e8)
![Screenshot from 2023-09-17 14-32-13](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/56fd2c77-b609-4141-916e-a3fc0db05065)

- ### Formation of N-well and P-well

Formation of N-well:

Substrate Selection: Start with a silicon wafer as the substrate. The silicon wafer is typically highly pure and is chosen for its semiconductor properties.

Oxide Growth: Grow a thin layer of silicon dioxide (SiO2) on the surface of the silicon wafer. This oxide layer serves as an insulator and as a protective layer.

Photoresist Application: Apply a layer of photoresist material onto the oxide layer. Photoresist is a light-sensitive material that will be used for masking purposes.

UV Lithography: Expose the photoresist layer to UV light through a photomask containing the desired N-well region patterns. This process creates a patterned photoresist layer.

Etching: Use a chemical etchant to selectively remove the exposed areas of the oxide layer, leaving windows where the N-well will be formed.

Photoresist Stripping: Remove the remaining photoresist material, leaving behind the patterned oxide layer with windows.

N-well Implantation: Introduce a dopant material (typically phosphorus or arsenic) into the exposed silicon substrate through the windows. This creates an N-type (negative) region in the silicon, forming the N-well.

Annealing: Heat treat the wafer to activate the dopant atoms and repair any damage caused during the implantation process.

Formation of P-well:

Substrate Selection: Start with the same silicon wafer used for the N-well process.

Oxide Growth: Grow a thin layer of silicon dioxide (SiO2) on the surface of the silicon wafer.

Photoresist Application: Apply a layer of photoresist material onto the oxide layer.

UV Lithography: Expose the photoresist layer to UV light through a different photomask containing the desired P-well region patterns. This creates a new patterned photoresist layer.

Etching: Use a chemical etchant to selectively remove the exposed areas of the oxide layer, leaving windows for the P-well.

Photoresist Stripping: Remove the remaining photoresist material, leaving behind the patterned oxide layer with windows.

P-well Implantation: Introduce a different dopant material (typically boron) into the exposed silicon substrate through the windows. This creates a P-type (positive) region in the silicon, forming the P-well.

Annealing: Heat treat the wafer to activate the dopant atoms and repair any damage caused during the implantation process.

![Screenshot from 2023-09-17 14-55-35](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8c37ecc3-5600-4e25-9e46-43e91f8264d9)
![Screenshot from 2023-09-17 14-56-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/154ba139-2e9b-4833-9575-7b4859ed8722)
![Screenshot from 2023-09-17 14-57-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/34cc532b-9c4f-4dce-b04e-ba45d776aa9d)
![Screenshot from 2023-09-17 14-57-57](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f9e0356e-622e-468e-80af-ba3043a68477)
![Screenshot from 2023-09-17 14-58-05](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/cf2caaef-7ea3-492d-835e-44bf6a6e17ce)
![Screenshot from 2023-09-17 14-58-20](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d1875f83-9792-462d-8839-15278d65fc15)
![Screenshot from 2023-09-17 14-59-38](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3130af16-fc66-4a1b-86ab-c1cfc45a11ee)
![Screenshot from 2023-09-17 15-00-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f2920eaa-d8cb-4693-b909-06b4cf698005)
![Screenshot from 2023-09-17 15-00-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b3625252-2a48-4b68-80e0-f210a60461b0)
![Screenshot from 2023-09-17 15-01-11](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/53e72c19-8526-440b-9550-39e7a3e29b1d)
![Screenshot from 2023-09-17 15-01-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6be644a4-2556-46fd-9c46-2133e99b59b4)



- ### Formation of gate terminal

 The formation of the gate terminal in a CMOS (Complementary Metal-Oxide-Semiconductor) integrated circuit involves the following steps:

Gate Oxide Growth: Grow a thin layer of insulating gate oxide (typically silicon dioxide, SiO2) on the silicon substrate.

Polysilicon Deposition: Deposit a layer of polysilicon (also known as poly) on top of the gate oxide. Polysilicon will be used to create the gate electrode.

Gate Patterning: Use photolithography and etching techniques to define the gate electrode pattern on the polysilicon layer.

 Doping (Optional): In some cases, the polysilicon gate electrode may be doped to adjust its electrical properties.





![Screenshot from 2023-09-17 14-36-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8da55799-f6f8-4b3b-beb7-d1591af856a6)
![Screenshot from 2023-09-17 14-38-40](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c39035af-ac8d-4549-854b-df067b70cd7b)
![Screenshot from 2023-09-17 14-40-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/65998b46-a72e-48f1-b45b-8756465c82cb)
![Screenshot from 2023-09-17 14-42-35](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7041adb4-294c-4463-a73c-a5951dc14273)
![Screenshot from 2023-09-17 14-43-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7114d3a2-bb22-45f6-b981-cd2817ad9b65)
![Screenshot from 2023-09-17 14-43-29](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/56201cff-ee63-4de8-ad3a-f1106313c6b1)
![Screenshot from 2023-09-17 14-44-07](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2b0ed540-4e7c-4cbe-971c-9f3140ba4cbb)
![Screenshot from 2023-09-17 14-44-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1b55455c-d35a-4d75-902d-3af8bafa4ee0)
![Screenshot from 2023-09-17 14-45-08](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7b492042-9050-4e6a-8835-d3a746bc274b)
![Screenshot from 2023-09-17 14-45-32](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/d90b570c-180e-4fee-8ac9-fe420f9466fb)
![Screenshot from 2023-09-17 14-45-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/69db8c43-fb23-4cd6-a03b-e311a4157d5b)
![Screenshot from 2023-09-17 14-46-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/93d07f74-e82d-4f24-9bfa-907fabdea0fa)
![Screenshot from 2023-09-17 14-47-38](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3c73351d-6f1b-4314-82ae-2dbbceea3a1e)

- ### Lightly doped drain (LDD) formation


The formation of Lightly Doped Drain (LDD) regions in a MOSFET (Metal-Oxide-Semiconductor Field-Effect Transistor) involves the following steps:

Initial Dopant Implantation: Introduce a light dose of dopant (typically a P-type or N-type impurity) into the substrate on both sides of the gate electrode. This forms lightly doped regions.

Silicon Oxide Deposition: Deposit a layer of silicon oxide (SiO2) over the entire structure.

Sidewall Spacer Formation: Use anisotropic etching to remove the SiO2 from the horizontal surfaces, leaving SiO2 on the vertical sidewalls of the gate electrode.

Heavy Dopant Implantation: Introduce a heavier dose of dopant into the exposed substrate regions adjacent to the sidewall spacers. This forms the heavily doped source and drain regions.

   ![Screenshot from 2023-09-17 17-43-21](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3463530e-7ac0-413a-815f-0985ebd70ce6)
![Screenshot from 2023-09-17 18-08-37](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c550200e-8144-4e1d-9f53-313d1f1b65b2)
![Screenshot from 2023-09-17 18-11-30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5a1d36b6-4a04-4406-8785-448fae4ba7b6)
![Screenshot from 2023-09-17 18-12-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/524e87a8-0294-4d80-a462-8d9b4f646434)
![Screenshot from 2023-09-17 18-12-32](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8924b955-bfe8-4673-9d96-07985349acd7)
![Screenshot from 2023-09-17 18-13-18](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/591d55e9-81e4-462a-8ee5-0f9d0c5f128e)
![Screenshot from 2023-09-17 18-13-54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/33e33099-3422-47fb-ba40-d9488b976396)
![Screenshot from 2023-09-17 18-14-55](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6ea258e7-cf28-4e9c-a82e-e1e06496978e)
![Screenshot from 2023-09-17 18-15-15](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/125579c8-af0b-4746-9749-d333138a3b53)
![Screenshot from 2023-09-17 18-15-52](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/909c0f82-b205-41a8-8cca-f065de33e44a)
![Screenshot from 2023-09-17 18-16-01](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7f12058d-416a-49e2-b50e-16856a5f892a)
![Screenshot from 2023-09-17 18-16-31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bcd30a3a-6d81-460f-9e4a-f7648c3079e8)
![Screenshot from 2023-09-17 18-17-08](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e1f2988e-5869-4c92-a440-b818ac69bd9b)


- ### Source Â drain formation

![Screenshot from 2023-09-17 18-20-12](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3356dabe-2447-4e84-aac4-00b7a7cc26cc)
![Screenshot from 2023-09-17 18-20-51](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7ab3f556-52e3-4427-bf4b-c17d96474c53)
![Screenshot from 2023-09-17 18-21-28](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/85efd251-613b-4c39-b05c-a714a139e05d)
![Screenshot from 2023-09-17 18-22-56](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7ec5e87b-9b2b-4fc3-b971-d132e9f1818e)
![Screenshot from 2023-09-17 18-23-50](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5d35c097-9680-49f3-be61-7a38d9969582)
![Screenshot from 2023-09-17 18-24-12](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e2215ffb-7ddc-4a9d-808f-71b69feafcc9)
![Screenshot from 2023-09-17 18-24-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/11f0429f-6c04-4949-8d37-e181d43b5f4e)
![Screenshot from 2023-09-17 18-25-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ab1de2a1-7c9b-416d-8258-cddf0a34c705)
![Screenshot from 2023-09-17 18-25-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b4ab0756-cbe7-4284-9165-26bf42a3f1ac)


- ### Local interconnect formation 
![Screenshot from 2023-09-17 18-25-25](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6149704a-4571-4493-a124-64473b0d3cbf)
![Screenshot from 2023-09-17 18-29-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2db47b99-f37c-4db6-9e4e-48b1383f07ef)
![Screenshot from 2023-09-17 18-30-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7da1638c-48fe-47ea-a950-143a08a62b4a)
![Screenshot from 2023-09-17 18-31-01](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/2a11d103-e5ce-4b8f-afdb-8e0b0d926749)
![Screenshot from 2023-09-17 18-31-42](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ce93ff75-6ee0-4da7-9b18-7d2992b66f78)
![Screenshot from 2023-09-17 18-31-58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/0702c4bc-b929-422a-9080-12d91407a944)
![Screenshot from 2023-09-17 18-32-43](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f62e40d1-313c-4dc6-b5e5-79591366bd2d)
![Screenshot from 2023-09-17 18-32-58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/0774864b-c999-4d24-9c79-f488e8d0d31b)
![Screenshot from 2023-09-17 18-34-26](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/51419184-3bbf-41e0-971b-15649a63e02b)
![Screenshot from 2023-09-17 18-35-14](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/7c757ff9-26dc-4f66-86de-0662048ae27a)
![Screenshot from 2023-09-17 18-35-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/84251179-56e0-4a30-ad2c-a27075fb53fa)
![Screenshot from 2023-09-17 18-35-33](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c78d915a-8618-4864-887e-46fbbee47a77)
![Screenshot from 2023-09-17 18-36-23](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b532f61b-6cef-4355-bbd9-a5a24f1d9c63)
![Screenshot from 2023-09-17 18-36-36](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/87dd81bd-a13e-4a64-8479-6c0b7a7bb079)


- ### Higher level metal formation
  
![Screenshot from 2023-09-17 18-36-46](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/eee39e58-d1a1-4181-b4eb-f61304f98c29)
![Screenshot from 2023-09-17 19-04-47](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6647890b-b98a-4e70-89db-5b6833d2eb2d)
![Screenshot from 2023-09-17 19-05-58](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1ce3a6e7-8b2b-4763-bc7b-e52b3c3cab6a)
![Screenshot from 2023-09-17 19-12-57](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e759f551-5f89-437d-b4e7-6022b0699013)
![Screenshot from 2023-09-17 19-14-13](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5dfa4e37-74dd-4093-85d3-7fc3f9955292)
![Screenshot from 2023-09-17 19-14-34](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/5db1f4f5-862c-4028-80d9-ba359e16ca8d)
![Screenshot from 2023-09-17 19-14-39](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/cf07dfe2-7958-44e5-b1d5-1d32139344e0)
![Screenshot from 2023-09-17 19-15-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/b6e57dbd-7c28-448a-a1f5-7242ea66a908)
![Screenshot from 2023-09-17 19-15-27](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/cb32b608-0370-47ef-beed-e45ee2ecbb2f)
![Screenshot from 2023-09-17 19-15-36](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/1c16d4b9-874b-4a68-bedc-cbbbeae2a1a5)
![Screenshot from 2023-09-17 19-16-54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e7ef238b-4fe5-45ad-bfad-a6954890086a)
![Screenshot from 2023-09-17 19-17-05](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/9bf3bd36-cda9-43cd-8683-86f7c6b2272d)
![Screenshot from 2023-09-17 19-17-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/64de6b1d-18b5-4dff-8797-d590218d90b2)
![Screenshot from 2023-09-17 19-17-20](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/f739aaad-25c1-4856-a893-6c5588c21425)
![Screenshot from 2023-09-17 19-17-28](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8988db4f-6ecd-417d-ba71-135dc4a88813)
![Screenshot from 2023-09-17 19-17-45](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/0c396d72-cbf8-44f7-84c6-e573e4921509)
![Screenshot from 2023-09-17 19-18-06](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/fadfcb56-5caa-4775-8ba3-8de8c05cdb76)
![Screenshot from 2023-09-17 19-21-07](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/c067b55f-e25e-4ebb-8e47-4be3b62e2a50)
![Screenshot from 2023-09-17 19-21-49](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/50503440-9bc8-4726-b41a-ed828d0df5a0)
![Screenshot from 2023-09-17 19-22-32](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e707e809-6e1f-4371-a6a7-fec3f5244065)
![Screenshot from 2023-09-17 19-23-17](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/3fadd29b-d8e2-48ed-8a11-a7d782a91109)
![Screenshot from 2023-09-17 19-23-40](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/e42bb111-da32-47a5-bdcd-38a848530368)
![Screenshot from 2023-09-17 19-24-09](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/ede4f858-86f2-47be-aab3-9ebfcf6c3a5c)

- ### Lab introduction to Sky130 basic layers layout and LEF using inverter 


 ![VirtualBox_PES_physical_design_17_09_2023_19_55_15](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8f7a53a1-4984-4e9c-874e-68763239881a)
![VirtualBox_PES_physical_design_17_09_2023_19_56_19](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/6b6dbbbc-5835-4042-be4c-61624a81ceec)
![VirtualBox_PES_physical_design_17_09_2023_19_57_31](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/bc10c9e5-7c17-47dc-8765-4d4871020caf)
![VirtualBox_PES_physical_design_17_09_2023_19_59_56](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/76c853ad-0e02-4b9b-a712-b1a95592f8a6)
![VirtualBox_PES_physical_design_17_09_2023_20_01_30](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/8ad814f6-326e-45fb-8102-784a5792ff54)
![VirtualBox_PES_physical_design_17_09_2023_20_01_54](https://github.com/Abhi9108865162/pes_asic_class/assets/141741065/46236685-75dd-4a76-87ba-030d2c239332)




- ### Lab steps to create std cell layout and extract spice netlist 


![Screenshot from 2023-09-17 20-08-33](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1e0171b7-0faf-4a66-8e8f-7919f4529c67)
![Screenshot from 2023-09-17 20-26-04](https://github.com/Abhi9108865162/pes_pd/assets/141741065/de0ff389-0de6-481e-822d-749cebb5ceb3)
![Screenshot from 2023-09-17 20-49-04](https://github.com/Abhi9108865162/pes_pd/assets/141741065/61d94925-cb81-4ba7-8275-eb98de7e58ba)
![Screenshot from 2023-09-17 20-50-24](https://github.com/Abhi9108865162/pes_pd/assets/141741065/b05925e9-474c-459a-8366-02a72580d369)
![Screenshot from 2023-09-17 20-50-47](https://github.com/Abhi9108865162/pes_pd/assets/141741065/c0884ec3-a442-44fb-a01b-4b78c20aafad)
![Screenshot from 2023-09-17 20-51-04](https://github.com/Abhi9108865162/pes_pd/assets/141741065/001bcdca-cca3-427e-9f99-76f26fa24346)

   
  ## Lab introduction to sky130 basic layers layout  LEF using inverter

![VirtualBox_PES_physical_design_17_09_2023_13_15_06](https://github.com/Abhi9108865162/pes_pd/assets/141741065/55c587c6-8d80-4c4b-920b-5804da632823)
![VirtualBox_PES_physical_design_17_09_2023_13_17_45](https://github.com/Abhi9108865162/pes_pd/assets/141741065/cd32fbe9-0483-48bf-a2ee-522b682a1ab2)

red - polysilicon <br>
green - n diffusion<br>
peach - p diffusion<br>
blue - metal<br>
- nmos
![VirtualBox_PES_physical_design_17_09_2023_19_56_19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/30f6fabc-aadb-4054-ba06-416e4df8de0a)
- pmos
![VirtualBox_PES_physical_design_17_09_2023_19_57_31](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6f2c2861-961a-4b9a-ae67-f08d928c85fc)

- drains connected to output Y
![VirtualBox_PES_physical_design_17_09_2023_19_59_56](https://github.com/Abhi9108865162/pes_pd/assets/141741065/46eb7ad8-6f5b-4f61-949e-57ae3ee6ad24)

- vdd connection
![VirtualBox_PES_physical_design_17_09_2023_20_01_30](https://github.com/Abhi9108865162/pes_pd/assets/141741065/fba49530-08e2-4732-8e8b-65e95b98b8ac)

- gnd connection
![VirtualBox_PES_physical_design_17_09_2023_20_01_54](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f99ddf5e-deee-49ad-87ef-931209f55ba5)

- LEF is on the right it contains the meatal connection(pr boundaries and ports)
  
![Screenshot from 2023-09-19 18-58-41](https://github.com/Abhi9108865162/pes_pd/assets/141741065/9351cf0d-dcce-40b0-96d9-3fa3f72616b3)

![VirtualBox_PES_physical_design_17_09_2023_22_42_41](https://github.com/Abhi9108865162/pes_pd/assets/141741065/da85d5a7-c3c5-4a5a-adef-1b2055dcb2a4)

![VirtualBox_PES_physical_design_17_09_2023_22_42_28](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f02e78f4-754c-4203-a3a4-0f312683e7ee)
![VirtualBox_PES_physical_design_17_09_2023_22_49_08](https://github.com/Abhi9108865162/pes_pd/assets/141741065/c5ceeb15-3ac7-41e9-a357-5eddfd67bb06)

![VirtualBox_PES_physical_design_17_09_2023_22_53_44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0d1c7553-4621-4cc8-ab15-720caea2e7e0)
![VirtualBox_PES_physical_design_17_09_2023_22_53_44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/ea1fea93-a189-4c83-a681-83183687ea0d)

![VirtualBox_PES_physical_design_17_09_2023_22_54_17](https://github.com/Abhi9108865162/pes_pd/assets/141741065/07cd6d8d-b329-40f5-8602-416282137a0b)
![VirtualBox_PES_physical_design_17_09_2023_23_41_59](https://github.com/Abhi9108865162/pes_pd/assets/141741065/ad2e0872-3f55-4dcb-933b-6eedc865f834)
![VirtualBox_PES_physical_design_17_09_2023_23_44_19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/9f39a1b4-6912-41bc-a676-7812c57fbb1b)

![VirtualBox_PES_physical_design_17_09_2023_23_42_54](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1d9339cf-5a76-444a-a2f7-b98c6f5530f0)
![VirtualBox_PES_physical_design_17_09_2023_23_59_27](https://github.com/Abhi9108865162/pes_pd/assets/141741065/45d476ea-638f-438a-bcee-a816632962b4)
![VirtualBox_PES_physical_design_17_09_2023_23_59_12](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f44465ef-ad9d-4bf8-9078-a1184bb35b1e)



To run the spice netlist, run ```ngspice sky130_inv.spice``` and ```plot y vs time a```
![Screenshot from 2023-09-19 19-49-44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/755d69b2-c15a-4bf1-895b-a00b01bade12)


![Screenshot from 2023-09-19 19-49-18](https://github.com/Abhi9108865162/pes_pd/assets/141741065/4b595dcd-5867-47bc-89db-8ca6601fb5d0)

The results obtained from the graph are :
- Rise Transition : 0.0395ns
- Fall transition : 0.0282ns
- Cell Rise delay : 0.03598ns
- Cell fall delay : 0.0483ns




</details>

<details>
<summary> WEEK-3 -> Day - 4 </summary>

# Pre-layout timing analysis and importance of good clock tree 


## 1. Timing modelling using delay tables


- ### Lab steps to convert grid info to track info

  
![VirtualBox_PES_physical_design_17_09_2023_20_01_54](https://github.com/Abhi9108865162/pes_pd/assets/141741065/5a5a8af9-e0b7-42c5-a45d-cdd154ddd0c0)
![VirtualBox_PES_physical_design_17_09_2023_22_42_41](https://github.com/Abhi9108865162/pes_pd/assets/141741065/a9d6d8f7-f90b-44ab-b794-a90d6eb9921d)
![VirtualBox_PES_physical_design_17_09_2023_22_42_28](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1106d970-ab3a-4795-9d30-32fe00f1186b)
![VirtualBox_PES_physical_design_17_09_2023_22_49_08](https://github.com/Abhi9108865162/pes_pd/assets/141741065/53d6a452-aedf-4247-9352-f856865ec676)
![VirtualBox_PES_physical_design_17_09_2023_22_53_44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/44a6a788-ef33-43f7-805f-de33f50a1482)
![VirtualBox_PES_physical_design_17_09_2023_22_54_17](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0932cecd-9506-4e47-88ba-328d9dc0d7a9)


- ### Lab steps to convert magic layout to std cell LEF

![Screenshot from 2023-09-17 23-32-03](https://github.com/Abhi9108865162/pes_pd/assets/141741065/af954ab5-00c5-41fb-bb3e-09477c7a5f3f)
![Screenshot from 2023-09-17 23-33-22](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bb3280f5-1be4-4e7e-8c99-d233cea42e3a)
![Screenshot from 2023-09-17 23-33-32](https://github.com/Abhi9108865162/pes_pd/assets/141741065/223e81d3-6c8d-4486-b03d-5d74b1a0aa0a)
![Screenshot from 2023-09-17 23-33-38](https://github.com/Abhi9108865162/pes_pd/assets/141741065/59881b06-9b32-46e1-a9dd-fd028e673d7e)
![Screenshot from 2023-09-17 23-34-11](https://github.com/Abhi9108865162/pes_pd/assets/141741065/03a9f0a9-eda2-4d76-aa78-5509c4ea59ae)
![VirtualBox_PES_physical_design_17_09_2023_23_41_59](https://github.com/Abhi9108865162/pes_pd/assets/141741065/ae1d8404-96b5-406a-a007-495739dc39b1)
![VirtualBox_PES_physical_design_17_09_2023_23_44_19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/31e4b653-8775-4a24-8551-d150f0dccf6d)
![VirtualBox_PES_physical_design_17_09_2023_23_42_54](https://github.com/Abhi9108865162/pes_pd/assets/141741065/29f5a5a2-1a23-4c64-956a-f3079d8f066b)
![VirtualBox_PES_physical_design_17_09_2023_23_45_33](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bdb24f5e-428b-461e-a436-67d7415ae0cc)






- ### Introduction to timing libs and steps to include new cell in synthesis


![VirtualBox_PES_physical_design_17_09_2023_23_52_55](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bb2f3f06-6696-49b7-ac6c-93395b4cfc4e)
![VirtualBox_PES_physical_design_17_09_2023_23_54_36](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1d5c4b53-c525-4aef-9455-97b61c9be0ae)
![VirtualBox_PES_physical_design_17_09_2023_23_54_11](https://github.com/Abhi9108865162/pes_pd/assets/141741065/15625117-2f27-4543-9ae1-f9feee5a3c8c)
![VirtualBox_PES_physical_design_17_09_2023_23_57_58](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0d1c4ecd-3cde-4537-ad5b-a6f7049be9a2)
![VirtualBox_PES_physical_design_17_09_2023_23_58_34](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8c76ed3c-7008-464d-9593-9f0893d993a8)
![VirtualBox_PES_physical_design_17_09_2023_23_59_12](https://github.com/Abhi9108865162/pes_pd/assets/141741065/7da92de7-5bae-4d49-970d-6328b18bafdb)
![VirtualBox_PES_physical_design_17_09_2023_23_59_27](https://github.com/Abhi9108865162/pes_pd/assets/141741065/73f1efa0-3368-427d-9b47-aa7aa5997643)
![VirtualBox_PES_physical_design_18_09_2023_00_02_00](https://github.com/Abhi9108865162/pes_pd/assets/141741065/28ef69d3-1cbd-46a0-925c-4426a6c94cf0)
![VirtualBox_PES_physical_design_18_09_2023_00_02_38](https://github.com/Abhi9108865162/pes_pd/assets/141741065/46b80777-37ce-432f-9488-a61088ec1609)
![VirtualBox_PES_physical_design_18_09_2023_00_03_35](https://github.com/Abhi9108865162/pes_pd/assets/141741065/63b9d96a-ce4a-47fb-97a9-a9b6f2b8a2bb)
![VirtualBox_PES_physical_design_18_09_2023_00_16_12](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3dd791bd-b3a2-41a2-806a-747911d61aa4)
![VirtualBox_PES_physical_design_18_09_2023_00_16_55](https://github.com/Abhi9108865162/pes_pd/assets/141741065/14adb1ff-d39e-4a64-9759-8a4b53b84f47)
![VirtualBox_PES_physical_design_18_09_2023_00_21_23](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8e2680a2-a4d3-4437-b537-a0fba190c3af)
![VirtualBox_PES_physical_design_18_09_2023_00_24_28](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0a8ec79f-7080-4845-96a0-a3441b34eb59)




- ### Introduction to delay tables

Delay tables, commonly used in digital circuit design, provide information about signal propagation delays through various logic elements. 
    Purpose: Delay tables capture the delay values associated with specific input patterns as signals pass through combinational logic gates or elements.
    Contents: They list input patterns (binary combinations), the corresponding output patterns, and the time delays between input and output.
    Application: Engineers use delay tables to evaluate and optimize the performance of digital circuits, ensuring signals meet timing requirements.
    Timing Analysis: They are instrumental in performing static timing analysis to assess whether a circuit meets setup and hold time constraints.


![Screenshot from 2023-09-18 00-35-08](https://github.com/Abhi9108865162/pes_pd/assets/141741065/db1430a3-5623-4aa3-815f-59f2f73f40a5)
![Screenshot from 2023-09-18 00-40-04](https://github.com/Abhi9108865162/pes_pd/assets/141741065/06d5477f-81c3-4aae-8f0a-9d53e63f6fb2)
![Screenshot from 2023-09-18 00-45-16](https://github.com/Abhi9108865162/pes_pd/assets/141741065/37334b51-77ab-40c9-b8a0-8f2cf3afb602)








- ### Delay table usage Part 1


![Screenshot from 2023-09-18 00-51-36](https://github.com/Abhi9108865162/pes_pd/assets/141741065/702ff17a-d21b-41a4-8ba0-49a70c74bb0b)
![Screenshot from 2023-09-18 00-59-08](https://github.com/Abhi9108865162/pes_pd/assets/141741065/26f2ef34-db65-4593-bbcc-4aa7f3d1dab4)




- ### Delay table usage Part 2


![Screenshot from 2023-09-18 00-57-09](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1352813d-74f1-4177-8a7f-b6500ef732ea)
![Screenshot from 2023-09-18 01-02-42](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3c0e7102-f43b-409d-9948-89a3bd72bbd7)
![Screenshot from 2023-09-18 01-15-45](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f5d5a798-623b-42ba-9c5e-b98b04ca812b)
![Screenshot from 2023-09-18 01-10-34](https://github.com/Abhi9108865162/pes_pd/assets/141741065/7358ef4c-190b-46a8-a2af-fc18de326df0)
![Screenshot from 2023-09-18 01-12-03](https://github.com/Abhi9108865162/pes_pd/assets/141741065/c819fe9c-d50c-4e28-9aad-9aac7cfda2f4)









- ### Lab steps to configure synthesis settings to fix slack and include vsdinv 


![VirtualBox_PES_physical_design_18_09_2023_10_53_09](https://github.com/Abhi9108865162/pes_pd/assets/141741065/4a99953c-cec5-471c-95b2-d9ef06f113c4)
![VirtualBox_PES_physical_design_18_09_2023_12_06_51](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bedbf225-57a2-480e-911e-4869fb424ce0)
![VirtualBox_PES_physical_design_18_09_2023_11_02_01](https://github.com/Abhi9108865162/pes_pd/assets/141741065/db103bf0-c655-451d-8d15-cac82115064f)
![VirtualBox_PES_physical_design_18_09_2023_10_57_18](https://github.com/Abhi9108865162/pes_pd/assets/141741065/027b8465-ab54-444a-a753-61eda49afa1e)
![VirtualBox_PES_physical_design_18_09_2023_11_20_34](https://github.com/Abhi9108865162/pes_pd/assets/141741065/c24b628a-0fb8-4ae7-985b-f2f96824b61d)
![VirtualBox_PES_physical_design_18_09_2023_11_21_28](https://github.com/Abhi9108865162/pes_pd/assets/141741065/50d78c0c-948d-4ecf-9363-255a9ef6fb18)
![VirtualBox_PES_physical_design_18_09_2023_11_22_19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/46807e6c-ee82-4980-86a6-f754a3037e24)
![VirtualBox_PES_physical_design_18_09_2023_11_29_14](https://github.com/Abhi9108865162/pes_pd/assets/141741065/d85b0f16-2c44-425e-9bfe-44da49be092b)
![VirtualBox_PES_physical_design_18_09_2023_11_31_15](https://github.com/Abhi9108865162/pes_pd/assets/141741065/9d827b59-c834-45c7-9cc9-22c800295bbf)
![VirtualBox_PES_physical_design_18_09_2023_11_31_42](https://github.com/Abhi9108865162/pes_pd/assets/141741065/b340ec6a-82d7-4408-aa59-49db6dc038eb)
![VirtualBox_PES_physical_design_18_09_2023_11_37_21](https://github.com/Abhi9108865162/pes_pd/assets/141741065/76c34948-20e2-44e7-be09-061a0cf49cfa)
![VirtualBox_PES_physical_design_18_09_2023_12_09_59](https://github.com/Abhi9108865162/pes_pd/assets/141741065/5dcf27d8-9492-4d5c-b0f7-72b17c96a6c5)
![Screenshot from 2023-09-18 11-53-32](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8b1c598b-cf52-4e1d-9444-63f6aee89ff1)
![Screenshot from 2023-09-18 11-53-43](https://github.com/Abhi9108865162/pes_pd/assets/141741065/572a241c-d300-4bf3-8f78-74eb379fa300)
![Screenshot from 2023-09-21 21-32-06](https://github.com/Abhi9108865162/pes_pd/assets/141741065/89cba032-20fd-4dc1-94f3-72339378d963)

![Screenshot from 2023-09-21 21-26-23](https://github.com/Abhi9108865162/pes_pd/assets/141741065/dec5d902-b923-43a4-8918-cdc19652afdd)



## 2. Timing analysis with ideal clocks using openSTA

- ### Setup timing analysis and introduction to flip-flop setup time 

![Screenshot from 2023-09-18 12-20-51](https://github.com/Abhi9108865162/pes_pd/assets/141741065/9610d2f2-5fb0-4f64-85ca-f39563fcea8b)
![Screenshot from 2023-09-18 12-30-03](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3bb22ade-1463-42b0-aa19-5464ea941982)
![Screenshot from 2023-09-18 12-33-10](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f49cebc8-665d-4b2d-8bdd-844887f83efb)
![Screenshot from 2023-09-18 12-34-47](https://github.com/Abhi9108865162/pes_pd/assets/141741065/32d32145-7590-411f-839d-2411a5ac8739)
![Screenshot from 2023-09-18 12-35-38](https://github.com/Abhi9108865162/pes_pd/assets/141741065/7a2898a4-bce3-43ff-82f0-5beeb64fd213)
![Screenshot from 2023-09-18 12-35-50](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6842645f-92f4-446e-9a68-1bd34d739255)


- ### Introduction to clock jitter and uncertainty


    Clock Jitter: Clock jitter refers to the variation in the timing of clock signal edges from their ideal positions. It can be caused by various factors, including noise and fluctuations, and can lead to signal timing errors and degraded performance.

    Uncertainty: Uncertainty in clock signals represents the range within which a clock edge can occur due to jitter. It's a measure of the uncertainty in timing and is often quantified as the standard deviation of jitter. Lower uncertainty indicates more precise clock timing.

![Screenshot from 2023-09-18 12-53-10](https://github.com/Abhi9108865162/pes_pd/assets/141741065/568ce802-7749-4fd0-a01c-7209fffd4ef6)
![Screenshot from 2023-09-18 12-53-59](https://github.com/Abhi9108865162/pes_pd/assets/141741065/ae9a9086-9bd3-4526-9212-3956aefda410)
![Screenshot from 2023-09-18 12-54-31](https://github.com/Abhi9108865162/pes_pd/assets/141741065/08838a24-cc9d-434e-9b55-a25134e6e9d6)
![Screenshot from 2023-09-18 12-54-58](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1276f920-214f-4d9e-a20a-927ec1ff59aa)
![Screenshot from 2023-09-18 12-55-44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/b9b4a519-f1f7-45fe-bdb0-e9607b6b19f4)
![Screenshot from 2023-09-18 12-56-29](https://github.com/Abhi9108865162/pes_pd/assets/141741065/4eb3d6dd-3b8e-4a3f-8085-c1c21c394a54)
![Screenshot from 2023-09-18 12-57-47](https://github.com/Abhi9108865162/pes_pd/assets/141741065/846cdcda-17d5-474b-b4aa-d0278316572a)
![Screenshot from 2023-09-18 12-58-30](https://github.com/Abhi9108865162/pes_pd/assets/141741065/56d5d21b-219c-4de3-8493-b9b00f6a2829)


- ### Lab steps to configure OpenSTA for post-synth timing analysis 

![VirtualBox_PES_physical_design_18_09_2023_16_24_40](https://github.com/Abhi9108865162/pes_pd/assets/141741065/34d9a2c7-a728-4bbb-ad76-2b1ff9449807)
![VirtualBox_PES_physical_design_18_09_2023_22_06_02](https://github.com/Abhi9108865162/pes_pd/assets/141741065/517a238f-80d0-4cb1-ad65-64d51ccd4a0f)
![VirtualBox_PES_physical_design_18_09_2023_22_05_48](https://github.com/Abhi9108865162/pes_pd/assets/141741065/4fce1c1e-240d-4df4-aa6e-455420041efb)
![VirtualBox_PES_physical_design_18_09_2023_22_03_20](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0d444a5e-7790-4e9e-9567-5e0c735bb52e)
![VirtualBox_PES_physical_design_18_09_2023_22_03_28](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bf4f95ae-2e01-4719-93be-9833bd4fe970)


3. Clock tree synthesis TritonCTS and signal integrity
- ### Clock tree routing and buffering using H-Tree algorithm

    Objective: To efficiently distribute the clock signal across a chip while minimizing skew, delay, and power consumption.

    H-Tree Structure: The clock tree is designed in the shape of an "H," with a central clock source at the base and branches extending outward like tree limbs.

    Buffering: Buffers are strategically inserted along the clock tree to ensure uniform signal strength and reduce clock skew.

    Balanced Fanout: The H-Tree algorithm maintains balanced fanout by dividing the clock signal evenly as it progresses through the branches.

    Reducing Skew: The H-Tree structure and buffering help minimize clock skew, ensuring synchronous operation of flip-flops and other clocked elements.

    Power Optimization: Careful placement and sizing of buffers help optimize power consumption.

    Common in ASIC Design: The H-Tree algorithm is commonly used in Application-Specific Integrated Circuit (ASIC) design to create a clock distribution network that meets timing and power requirements.


![Screenshot from 2023-09-18 17-10-04](https://github.com/Abhi9108865162/pes_pd/assets/141741065/2e86dde4-0b98-45cf-a4bf-192e26bdf045)
![Screenshot from 2023-09-18 17-10-34](https://github.com/Abhi9108865162/pes_pd/assets/141741065/54ef1519-c2ae-4044-9977-f8d78e76fe2d)
![Screenshot from 2023-09-18 17-14-32](https://github.com/Abhi9108865162/pes_pd/assets/141741065/d2e8a657-c7e6-4d1f-b3a6-e2dbb17d0dcd)
![Screenshot from 2023-09-18 17-14-51](https://github.com/Abhi9108865162/pes_pd/assets/141741065/ac1d451c-c47d-4c81-9d96-278e0b8b66b9)
![Screenshot from 2023-09-18 17-15-17](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bff81204-29d7-461c-bd57-f5950bacb9eb)
![Screenshot from 2023-09-18 17-16-32](https://github.com/Abhi9108865162/pes_pd/assets/141741065/5e9c4b77-d153-4cdb-ac93-a77bc107898f)
![Screenshot from 2023-09-18 17-19-30](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6c0d1e32-913c-435b-8b3d-037e1ee8f670)
![Screenshot from 2023-09-18 17-20-24](https://github.com/Abhi9108865162/pes_pd/assets/141741065/be265dec-e7d0-4eb7-9f38-297804b628cc)
![Screenshot from 2023-09-18 17-22-34](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3a2fc89f-d640-481c-b99e-cdee45885352)


- ### Crosstalk and clock net shielding

Crosstalk in digital circuits refers to unwanted interference or coupling between adjacent signal traces, which can lead to signal distortion or noise. Clock net shielding is a technique used to mitigate crosstalk effects. 

Crosstalk: Unwanted interference between signal traces due to their proximity. It can result in signal corruption, delays, or erroneous readings.

Clock Net Shielding: Involves physically isolating clock lines from other signal lines, reducing the likelihood of crosstalk. This can be achieved by placing ground or shield layers between clock and signal layers or by using specialized routing techniques.



![Screenshot from 2023-09-18 17-38-20](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3bbd0cec-f1e4-4758-903d-6e8c6197a883)
![Screenshot from 2023-09-18 17-38-36](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f67c053d-3140-4928-a964-38f14b57681b)
![Screenshot from 2023-09-18 17-41-24](https://github.com/Abhi9108865162/pes_pd/assets/141741065/c3e25a3a-2d7a-4f96-8db2-4ed44ef0ae24)
![Screenshot from 2023-09-18 17-42-45](https://github.com/Abhi9108865162/pes_pd/assets/141741065/30c848e5-e699-4105-9f49-8348f27cc45e)
![Screenshot from 2023-09-18 17-43-19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/dfec67f7-29b4-4b77-a871-8197a8528b06)
![Screenshot from 2023-09-18 17-43-19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6b78110c-acbd-4de2-98f3-a25d76a9e5fa)
![Screenshot from 2023-09-18 17-46-40](https://github.com/Abhi9108865162/pes_pd/assets/141741065/d82fd2d4-e72d-4407-91e4-42c5cb8dc0c1)



## 4. Timing analysis with real clocks using openSTA 

- ### Setup timing analysis using real clocks
    Clock Specification: Define the characteristics of the clock signals, including frequency, duty cycle, and clock sources.

    Clock Domain Identification: Identify different clock domains in the design, as each domain may have unique timing constraints.

    Clock Skew Analysis: Analyze clock skew, which is the variation in arrival times of the clock signal at different points in the circuit.

    Clock Tree Synthesis: Design and implement the clock distribution network (clock tree) to ensure clock signals reach all relevant components with minimal skew.

    Synchronous Design: Ensure that all flip-flops and sequential elements are clocked by the appropriate clock signal within their respective domains.

    Setup Time and Hold Time: Specify setup time and hold time requirements for each flip-flop to ensure proper data capture.

    Propagation Delay Analysis: Calculate the propagation delay for critical paths in the design to determine if signals meet setup and hold time requirements.

    Constraint Verification: Use timing analysis tools to verify that the design meets all specified timing constraints for real clock signals.

    Iterative Optimization: If timing violations are detected, iterate on the design to optimize critical paths or adjust clock domains and clock signals as needed.

    Final Verification: Perform a final timing analysis to confirm that all real clock signals meet the setup and hold time requirements, ensuring reliable circuit operation.

![Screenshot from 2023-09-18 17-53-16](https://github.com/Abhi9108865162/pes_pd/assets/141741065/59dc9d18-3367-4ad9-8704-6e4a7ea35d69)
![Screenshot from 2023-09-18 17-53-28](https://github.com/Abhi9108865162/pes_pd/assets/141741065/28bd3e95-9f76-476e-933c-b6cb9092e6e0)
![Screenshot from 2023-09-18 19-47-54](https://github.com/Abhi9108865162/pes_pd/assets/141741065/fc8959ff-6734-4f2b-b880-5a84a2672505)
![Screenshot from 2023-09-18 20-01-05](https://github.com/Abhi9108865162/pes_pd/assets/141741065/70cb82c0-448d-4095-9c6c-216694a65238)
![Screenshot from 2023-09-18 20-04-02](https://github.com/Abhi9108865162/pes_pd/assets/141741065/b9a15824-ce17-456b-a219-b4cda9b9b6b2)
![Screenshot from 2023-09-18 20-04-26](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8fd00394-c220-4112-8ca1-b4fe80712bc8)
![Screenshot from 2023-09-18 20-05-41](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8087a1a3-64a9-4ee6-a291-d4984fe87b1a)
![Screenshot from 2023-09-18 20-10-33](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0bd503eb-542c-4077-8b1d-b814795b2d26)
![Screenshot from 2023-09-18 20-11-06](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3869ea53-b9b9-4e47-a81e-eaf7a9eddcba)
![Screenshot from 2023-09-18 20-13-29](https://github.com/Abhi9108865162/pes_pd/assets/141741065/7340950f-1761-4434-a91b-c2becb457d6d)
![Screenshot from 2023-09-18 20-13-24](https://github.com/Abhi9108865162/pes_pd/assets/141741065/83a39c10-8b41-4249-99fb-530bf8f8e39d)


- ### Hold timing analysis using real clocks

    Clock Specification: Define clock characteristics, including frequency, duty cycle, and clock sources.

    Identify Clock Domains: Recognize different clock domains in the design, each with its own clock signal.

    Hold Time Definition: Specify the hold time requirement, denoted as Thold, which is the minimum time data must remain stable after the clock edge.

    Data Path Analysis: Analyze the data paths, especially flip-flops and sequential elements, to ensure that data signals meet the hold time requirement.

    Propagation Delay Calculation: Calculate the propagation delay for critical paths in the design to determine if data meets the Thold requirement.

    Constraint Verification: Use timing analysis tools to verify that all data signals within a clock domain satisfy the hold time requirement for real clock signals.

    Adjustments: If hold violations are detected, consider adjustments like buffer insertion, pipeline stages, or clock domain synchronization to meet the Thold requirement.

    Final Verification: Perform a final timing analysis to confirm that data signals in all clock domains satisfy the hold time constraints, ensuring stable operation and avoiding data corruption.

![Screenshot from 2023-09-18 20-13-29](https://github.com/Abhi9108865162/pes_pd/assets/141741065/736832f5-dcde-4505-b5e7-a84cea351f73)
![Screenshot from 2023-09-18 21-40-16](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1d44122a-74b5-4933-a133-34cf22ff75f8)
![Screenshot from 2023-09-18 21-44-23](https://github.com/Abhi9108865162/pes_pd/assets/141741065/023bde3b-b896-43d9-a9ce-951af443fee1)
![Screenshot from 2023-09-18 21-45-12](https://github.com/Abhi9108865162/pes_pd/assets/141741065/80bbea3b-58ca-4ebd-84f6-c524927ccaf5)
![Screenshot from 2023-09-18 21-45-50](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6663e659-f19f-4461-8994-11b448242d31)
![Screenshot from 2023-09-18 21-47-14](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0ab9b384-8848-472c-bd80-b1c58df9775f)
![Screenshot from 2023-09-18 21-48-41](https://github.com/Abhi9108865162/pes_pd/assets/141741065/130d6852-1eb4-4e05-bda9-d17fecced718)
![Screenshot from 2023-09-18 21-48-52](https://github.com/Abhi9108865162/pes_pd/assets/141741065/7805c880-16fb-452d-9266-01c80e97e058)
![Screenshot from 2023-09-18 21-49-27](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6ea8a520-82c7-47ea-8f38-2bee5b8bab22)
![Screenshot from 2023-09-18 21-49-48](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3f2ab4de-2686-45b3-a129-ca53016c0207)


## Lab 
start openlane<br>
```
docker
```
```
./flow.tcl -interactive
```
```
package require openlane 0.9
```
```
prep -design picorv32a -tag 16-09_17-39 -overwrite
```
```
set lefs [glob $::env(DESIGN_DIR)/src/*.lef]
 
add_lefs -src $lefs
```
```
run_synthesis
```
```
init_floorplan
```
```
run_placement
```
```
run_cts
```

```
openroad
```

reading the .lef file<br>
```
read_lef /openLANE_flow/designs/picorv32a/runs/16-09_17-39/tmp/merged.lef
```

reading the .def file<br>

```
read_def /openLANE_flow/designs/picorv32a/runs/16-09_17-39/results/cts/picorv32a.cts.def
```

```
write_db pico_cts.db
```
```
read_db pico_cts.db
```
```
read_verilog /openLANE_flow/designs/picorv32a/runs/16-09_17-39/results/synthesis/picorv32a.synthesis_cts.v
```


```
read_liberty -max $::env(LIB_SLOWEST)
```
```
read_liberty -max $::env(LIB_FASTEST)
```

```
read_sdc /openLANE_flow/designs/picorv32a/src/my_base.sdc
```


```
set_propagated_clock [all_clocks]
```
```
report_checks -path_delay min_max -format full_clock_expanded -digits 4
```
</details>






<details>
<summary> WEEK-3 -> Day - 5 </summary>

# Final steps for RTL2GDS using tritonRoute and openSTA 


## 1. Routing and design rule check (DRC)
- ### Introduction to Maze Routing Â LeeÂs algorithm

Lee's Algorithm Introduction:

Objective: Lee's algorithm aims to find the shortest path between a source and a destination in a maze or grid.

Grid Representation: The maze or grid is represented as a two-dimensional array, where each cell can be either open (passable) or blocked (impassable).

Queue-Based Approach: Lee's algorithm employs a queue data structure for exploration. It starts at the source point and explores neighboring cells in layers, gradually moving away from the source.

 Breadth-First Search (BFS): Lee's algorithm uses a BFS-like approach, ensuring that the shortest path is found before longer paths.

Layered Exploration: The algorithm assigns layers or distances to cells from the source. Cells closest to the source have a layer of 1, those farther away have a layer of 2, and so on.

 Propagation Rules: It expands from the source by examining adjacent cells in the grid and marking them with their corresponding layer numbers. This continues until the destination is reached.

 Backtracking: After reaching the destination, Lee's algorithm can backtrack from the destination cell following the lowest-layered adjacent cells until it returns to the source, thereby finding the shortest path.

Applications: Lee's algorithm has applications in maze solving, printed circuit board (PCB) routing, and network routing, among others.


![Screenshot from 2023-09-18 22-12-34](https://github.com/Abhi9108865162/pes_pd/assets/141741065/966c8a39-41aa-4584-9fa9-f71fb3ebb0aa)
![Screenshot from 2023-09-18 22-13-41](https://github.com/Abhi9108865162/pes_pd/assets/141741065/485414c4-e059-4a36-863a-96987ffd7555)
![Screenshot from 2023-09-18 22-15-22](https://github.com/Abhi9108865162/pes_pd/assets/141741065/82115f94-3efc-4f39-b68a-f5fba5b7e7fd)
![Screenshot from 2023-09-18 22-16-00](https://github.com/Abhi9108865162/pes_pd/assets/141741065/2c6e470f-6451-457f-9115-a31bd94ed035)
![Screenshot from 2023-09-18 22-19-57](https://github.com/Abhi9108865162/pes_pd/assets/141741065/28428227-d33d-4d1f-ac91-64915ba72389)

  
- ### LeeÂs Algorithm conclusion


In conclusion, Lee's Algorithm is a grid-based pathfinding method that uses a breadth-first search approach to find the shortest path between two points in a maze or grid. It assigns layers or distances to cells from the source and propagates through neighboring cells until the destination is reached. It is effective for maze solving and routing applications, ensuring that the shortest path is found while avoiding obstacles.


![Screenshot from 2023-09-18 22-19-57](https://github.com/Abhi9108865162/pes_pd/assets/141741065/d1a1ec2b-f60f-4287-9368-d1277399669f)
![Screenshot from 2023-09-18 22-27-14](https://github.com/Abhi9108865162/pes_pd/assets/141741065/1a1673d7-151a-4d7a-b34c-326c1b09b13e)
![Screenshot from 2023-09-18 22-27-32](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f7a330cb-3137-4156-bdb0-87e1e7d83883)
![Screenshot from 2023-09-18 22-29-44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/e02f4889-e40c-4694-afda-884ebdae97c9)
![Screenshot from 2023-09-18 22-29-52](https://github.com/Abhi9108865162/pes_pd/assets/141741065/155406f0-26a4-4f85-8e55-bc859e46699b)
![Screenshot from 2023-09-18 22-29-57](https://github.com/Abhi9108865162/pes_pd/assets/141741065/79baccd5-09b8-4e92-9793-7db69cfa1560)
![Screenshot from 2023-09-18 22-31-09](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8d24e609-d199-42fe-bcee-b1cf874e3ffa)
![Screenshot from 2023-09-18 22-32-08](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bc5849d8-878b-400e-ada5-c1b4861f8d18)



- ### Design Rule Check

A Design Rule Check (DRC) is a verification process used in semiconductor and integrated circuit manufacturing to ensure that the physical layout of a chip adheres to the foundry's design rules and manufacturing constraints.

 Purpose: DRC ensures that the layout meets manufacturing specifications and avoids potential fabrication errors.

Process: It examines the layout's geometry and compares it to a set of predefined rules, checking for violations such as minimum feature sizes, spacing requirements, and more.

Verification: DRC identifies any violations or errors in the layout and provides feedback to designers for corrections.

Critical in IC Manufacturing: DRC is a critical step in semiconductor manufacturing to guarantee that the final chip will be manufacturable and functional.





![Screenshot from 2023-09-18 22-38-06](https://github.com/Abhi9108865162/pes_pd/assets/141741065/d0faed40-a257-431c-80cc-4b6a544b165b)
![Screenshot from 2023-09-18 22-39-13](https://github.com/Abhi9108865162/pes_pd/assets/141741065/3f263508-1422-420f-a4a8-d307322609f7)
![Screenshot from 2023-09-18 22-40-58](https://github.com/Abhi9108865162/pes_pd/assets/141741065/0dce9e39-5873-4bf1-8b4d-5205a039b4e0)
![Screenshot from 2023-09-18 22-41-52](https://github.com/Abhi9108865162/pes_pd/assets/141741065/75807d11-6379-4f83-9070-efaacb207799)
![Screenshot from 2023-09-18 22-43-29](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bf5f60ea-30e7-4d92-ae9e-2fa20ce482b0)
![Screenshot from 2023-09-18 22-44-24](https://github.com/Abhi9108865162/pes_pd/assets/141741065/dcece0bd-6359-4eab-8d34-2e7bff7f6017)
![Screenshot from 2023-09-18 22-45-08](https://github.com/Abhi9108865162/pes_pd/assets/141741065/df975867-e5b2-4a59-ac58-24e19bec6065)
![Screenshot from 2023-09-18 22-46-21](https://github.com/Abhi9108865162/pes_pd/assets/141741065/66a432de-a097-4e07-84f1-736c04e90ca4)
![Screenshot from 2023-09-18 22-46-59](https://github.com/Abhi9108865162/pes_pd/assets/141741065/fd6d7671-1284-45ab-91e5-eb628bf54a7e)
![Screenshot from 2023-09-18 22-47-22](https://github.com/Abhi9108865162/pes_pd/assets/141741065/b16e767d-0889-4269-a793-c9de210398cd)













  
## 2. Power Distribution Network and routing
```
cd ~/Desktop/work/tools/openlane_working_dir/openlane
```
```
docker
```
```
./flow.tcl -interactive
```
```
package require openlane 0.9
```
```
prep -design picorv32a -tag 16-09_17-39
```
```
echo $::env(CURRENT_DEF)
```
```
gen_pdn
```
```
run_routing
```
<image10>
green color reg - picorv32<br>

red - vdd<br>
blue - gnd<br>

Global routing in chip design is the initial stage that establishes a high-level plan for connecting components on an integrated circuit. It addresses wirelength, congestion, and power considerations.

Detailed routing follows, refining connections, ensuring manufacturability, and completing the chip's interconnections. Both stages are crucial for chip functionality and performance.


## 3. TritonRoute Features

Routing Requirements forr Preprocessed Guides:
1 Should have unit width.
2 Should be on the preferred direction.

TritonRoute
1 Inputs : .lef, .def, processed route guides
2 Outputs : Detailed routing solution with optimised ire length and via count.
3 Constraints : Route guides, connectivity constraints and design rules.

4 Access Point : on-grid point on the metl layer of the route guide, and is used to connect to lower layer, upper layer segments, pins and ports.
5 Access Point Cluster : A union of all APs derived from everything.
![Screenshot from 2023-09-19 18-31-19](https://github.com/Abhi9108865162/pes_pd/assets/141741065/b2385789-8a5a-4061-95f7-c7ce843bb565)
![Screenshot from 2023-09-19 18-31-35](https://github.com/Abhi9108865162/pes_pd/assets/141741065/8c5c88f7-b840-4db2-8b5d-c703687c4e63)
![Screenshot from 2023-09-19 18-31-48](https://github.com/Abhi9108865162/pes_pd/assets/141741065/f7419ebf-59c4-4265-a2fe-28c010aaee45)
![Screenshot from 2023-09-19 18-32-03](https://github.com/Abhi9108865162/pes_pd/assets/141741065/6ef1f161-ed54-4b43-8939-5605bea96117)
![Screenshot from 2023-09-19 18-32-16](https://github.com/Abhi9108865162/pes_pd/assets/141741065/5da0bc85-bb11-4d7d-83c5-82f977dc3f15)
![Screenshot from 2023-09-19 18-32-35](https://github.com/Abhi9108865162/pes_pd/assets/141741065/bfb7b1fa-9065-43f3-a34d-1c5e7ad33220)
![Screenshot from 2023-09-19 18-32-44](https://github.com/Abhi9108865162/pes_pd/assets/141741065/97674567-29f7-47c4-8cea-4f21a78ceba3)



</details>


