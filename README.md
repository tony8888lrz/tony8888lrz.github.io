## Runze Liao  

This is [Tony's](https://github.com/tony8888lrz) webpage.
![46D54DA61313AAE2C1DAF6E141FD313E](https://user-images.githubusercontent.com/72693579/166874266-e1df8f0e-d73f-42e9-b0d9-5d50bc3e9046.png){:width = "200px" height="200px"}
  
He wishes u enjoy the music.  
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=120 src="//music.163.com/outchain/player?type=2&id=4237923&auto=1&height=66"></iframe>
### Education background
2008-2014 [ZongBei Primary School](https://baike.baidu.com/item/%E6%A3%95%E5%8C%97%E5%B0%8F%E5%AD%A6/5468346?fr=aladdin)  
2014-2020 [Chengdu Experimental Foreign Language School (Western Campus)](http://www.cdswxq.com/)  
2020-2024 [Southwest University](http://www.swu.edu.cn/) & [University of Auckland](http://www.uoa.edu.au/) Joint training BSc programs  
2024-? [?](https://www.cuhk.edu.hk/)  

### About  
Runze Liao is currently a Bachelor of College of Computer and Information Science, Southwest University, China and a Bachelor of the University of Auckland. He will receive B.S. from Southwest University and University of Auckland, C.N. & N.Z., His research interests include computer vision, computational photography，  graphics, and deep learning. 
[CV](https://github.com/tony8888lrz/tony8888lrz.github.io/blob/main/CV_Runze_mitcas.pdf)

### Projecet
Modeling Deep Learning Based Privacy Attacks on Physical Mail's Extension of Text [Text-Neural-STE(code)](https://github.com/tony8888lrz/Neural-STE_Text/)   

Swu-book-management-system [Data-Structure Curriculum Final Project(code)](https://github.com/tony8888lrz/swu-book-management-system)   

### News  
He won a National Encouragement Scholarship 2022(top 2%)  



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

For more information about this boy, you can find him in [scholar](http://scholar.com).

### Workspace

- He has done some work in his Undergraduate career :  [data structure](https://github.com/tony8888lrz/data-structure) & [c++](https://github.com/tony8888lrz/SWU-c-plus-plus) & [swu book management system](https://github.com/tony8888lrz/swu-book-management-system)   
- He is the initiator of this project :  [swu-cst-cracker](https://github.com/tony8888lrz/swu-cst-cracker) star[6]

### Preference
His favorite director is Stanley Kubrick.  
His favorite band is Radiohead & Pink Floyd.  

### Contact

[ins](https://www.instagram.com/ttoooonnny/)   
[linkedin](https://www.linkedin.cn/incareer/in/ACoAADsXTKgBP0cHKc9Dhx7yOvdeLLMCxyaK9Os)  
qq:2043491428  
wechat:liaorunze1314  
phone:19934325211 
