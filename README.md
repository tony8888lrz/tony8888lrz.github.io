## Runze Liao  

![46D54DA61313AAE2C1DAF6E141FD313E](Photo.jpg){:width = "200px" height="200px"}
  
### Education
2014-2020 [Chengdu Experimental Foreign Language School (West Campus)](http://www.cdswxq.com/)  
2020-2024 [Southwest University](http://www.swu.edu.cn/) & [University of Auckland](http://www.uoa.edu.au/) Joint Bachlor programs  
2024- He is now applying to his graduate degree.

### About  
This is Runze Liao, he is currently a forth-year bachelor’s student at Southwest University Joint Bachlor program (with University of Auckland), majoring in Computer Science.

Runze Liao is currently a Bachelor of College of Computer and Information Science, Southwest University, China and a Bachelor of the University of Auckland. He will receive B.S. from Southwest University and University of Auckland, C.N. & N.Z., His research interests include computer vision, graphics, and visual privacy attack.
[CV](https://github.com/tony8888lrz/tony8888lrz.github.io/blob/main/CV_Runze_mitcas.pdf)  

He serves as undergraduate research assistant since May 2022, working on the area of Visual Privacy Attack, supervised by [Bingyao Huang](bingyaohuang.github.io)  

### Projects
Modeling Deep Learning Based Privacy Attacks on Physical Mail's Extension of Text [Text-Neural-STE (Coming soon)](https://github.com/tony8888lrz/Neural-STE_Text/)   

Swu-book-management-system [Data-Structure Curriculum Final Project (code)](https://github.com/tony8888lrz/swu-book-management-system)   

### News  

He awarded National Encouragement Scholarship in 2023.  
He awarded National Encouragement Scholarship in 2022.



```py
fn research_no_failure()->Result < Paper, Error > {
    let output = if cfg!(target_os = "linux") {
        Command::new("qemu-x86_64-system")
        .args(["-smp 6",
             "-numa node,cpus=0-2,memdev=mem0,nodeid=0",
             "-object memory-backend-ram,id=mem0,size=8G",
             "-numa node,cpus=3-5,memdev=mem1,nodeid=1",
             "-object memory-backend-ram,id=mem1,size=8G",
             "-m 16G,slots=4,maxmem=32G",
             "-machine q35,cxl=on",
             "-M cxl-fmw.0.targets.0=cxl.1,cxl-fmw.0.size=4G",
             "-device pxb-cxl,bus_nr=12,bus=pcie.0,id=cxl.1",
             "-device cxl-rp,port=0,bus=cxl.1,id=root_port13,chassis=0,slot=2",
             "-object memory-backend-file,id=cxl-mem1,share=on,mem-path=/tmp/cxltest.raw,size=256M",
             "-object memory-backend-file,id=cxl-lsa1,share=on,mem-path=/tmp/lsa.raw,size=256M",
             "-device cxl-type3,bus=root_port13,memdev=cxl-mem1,lsa=cxl-lsa1,id=cxl-mem0",
             "-device virtio-crypto-cxl,id=crypto0,cryptodev=cryptodev0",
             "-object cryptodev-backend-builtin,id=cryptodev0",
             "-object secret,id=sec0,file=./Drywall/passwd.txt"])
            .output()
            .expect("failed to execute process")
    }
    let paper = Paper::new(output);
    loop{
        asm!("clflush" :: "r" (&paper.iter()) : "rax", "rbx", "rcx", "rdx": "volatile" );
        __atomic_thread_fence(__ATOMIC_SEQ_CST);
        if (paper.is_valid()){
            break;
        }
    }
    Ok(paper)
}
```

### Workspace

- He has done some work in his Undergraduate career :  [Data Structure](https://github.com/tony8888lrz/data-structure), [C++](https://github.com/tony8888lrz/SWU-c-plus-plus) and [Southwest University Book Management System](https://github.com/tony8888lrz/swu-book-management-system)   
- He is the initiator of swu-cst-cracker :  [swu-cst-cracker](https://github.com/tony8888lrz/swu-cst-cracker) 

### Contact  

[Linkedin](https://www.linkedin.cn/incareer/in/ACoAADsXTKgBP0cHKc9Dhx7yOvdeLLMCxyaK9Os)  
Wechat: runze324  
