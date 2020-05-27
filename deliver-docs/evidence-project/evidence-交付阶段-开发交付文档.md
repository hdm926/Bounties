#当前开发阶段：项目交付

#预计开发时间：2020-04至2020-05

#实际开发时间：2020-04至2020-05

#开发内容简要说明：借助区块链实现了电子证据的存储和固定。经系统存储的电子证据能提高可信度，降低司法诉讼中关于验证电子证据真实性的成本，提高诉讼效率，降低当事人维权的成本。

##面向的用户：1.固定电子证据用以再诉讼中维权的用户；  2.用以对艺术作品生命原创的用户；  3.查证的司法部门；

##存证需求：1.对于用户1，他们存储的电子证据往往需要用来证明案件真相，需要返回证据原文件；  2.对于用户2，他们需要借助区块链的时间戳标识作品完结的时间，借助哈希验证标识作品的内容，所以仅需要返回哈希验证的结果；

##验证需求：对于第一类用户，输入标识码，返回原文件；  对于第二类用户，输入标识码和原文件，返回哈希比较的结果；





#项目开发代码库：

<https://github.com/hdm926/aelf-boilerplate>



#项目需求说明：描述项目的开发背景、用户、需求、功能等；

##开发背景：随着信息技术的发展，电子证据在诉讼过程出现的频率高、范围广、种类多，由于易篡改，如何认定电子证据的真实性成了案件的首要难题；

           此外，电子证据也易消亡，通常需要多次备份存证且可信度的高低也依赖于原始存储媒介；

           再者，传统存证方式耗时久、效率低、成本高，也不适合电子证据的存证。

           在电子证据的生成、收集、传输、存储的全生命周期中，区块链可以对电子数据进行安全防护、防止篡改、并进行数据操作的审计留痕，从而为相关机构审查提供有效手段。

           本项目借助区块链实现了对电子证据的存证和验证操作。

##面向用户：需要将各类电子证据等作为诉讼证据的用户；

           需要将自己的艺术创作进行原创声明以备日后被抄袭之后用于维权的用户；

           需要在诉讼阶段查看当事人提交的电子证据的司法机关；

##需求：1）对用户提供的电子证据进行哈希计算之后存储并固定；

       2）根据文件标识码查看存储在链上的原文件信息。

##功能：提供两种存证方案，方案一：存储文件哈希、文件二进制数组、文件名、文件大小等信息；

       方案二：存储文件哈希、文件名、文件大小等信息，不存储文件内容；存证完成后将文件标识码返回给用户；

       提供相对应的两种验证方案，验证方案一：用户输入存证时返回的文件标识码，系统根据该标识码返回存储在链上的文件二进制数组，并将数组转成图片之后正在前端界面显示；

       验证方案二：用户输入标识码，同时上传原文件，系统对原文件进行相同的哈希计算，并和链上存储的文件哈希进行比较，返回一个布尔值，表示文件是否被篡改过。



#项目设计说明：

##描述项目的框架设计：

###系统流程图：![系统流程图](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E7%B3%BB%E7%BB%9F%E6%B5%81%E7%A8%8B%E5%9B%BE.png)   

###存证流程图：![存证流程图](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E5%AD%98%E8%AF%81%E6%B5%81%E7%A8%8B%E5%9B%BE.png)     

###验证流程图：![验证流程图](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E7%B3%BB%E7%BB%9F%E6%B5%81%E7%A8%8B%E5%9B%BE.png)   



##数据库设计：

###State:![state](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E6%95%B0%E6%8D%AE%E5%BA%93.png)   

###proto中的一些message：

![ptroto1](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/proto%E8%AE%BE%E8%AE%A11.png)   

![proto2](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/proto%E8%AE%BE%E8%AE%A12.png)   



#测试报告：

##项目的开发完成情况：功能开发完成，已完成各项测试.

##环境：（1）合约使用C#语言，编码IDE为JetBrains Rider；（2）前端界面使用JavaScript语言，react框架，ant-design组件库，编码IDE为WebStorm；（3）系统环境：Windows10家庭版。



#使用说明：

##存证：上传的文件来自用户本地存储。两个按钮：“存图”表示系统将存储图片的全部信息，对应存证方案1；“存哈希”表示系统将存储文件哈希，不会存储全部文件内容，对应存证方案2。界面中央的哈希码为存证完成时返回的文件标识码。界面最下方的图片是用户选择上传的图片的预览。

![存证](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E5%AD%98%E8%AF%81%E6%88%AA%E5%9B%BE.png)   

##验证：  

(1)验证方案一对应存证时的“存图”，只需要输入存证时返回的文件标识码，点击“验哈希”，系统会将原文件显示在界面上。

![验证1](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E9%AA%8C%E8%AF%81%E6%88%AA%E5%9B%BE1.png)     

(2)验证方案二对应存证时的“存哈希”，输入文件标识码，同时上传原文件，点击“验图与哈希”，系统返回比对结果：“哈希一致”表示图片未经篡改，“哈希不一致”表示此时上传的文件和存证时的文件不符，“标识码错误”表示链上没有存储该标识码对应的文件信息，可能是输入错误。

![验证2](https://github.com/hdm926/aelf-boilerplate/raw/dev/chain/contract/AElf.Contracts.EvidenceContract/%E9%AA%8C%E8%AF%81%E6%88%AA%E5%9B%BE2.png)



上述操作使用的图片如下：![PIC10](https://github.com/hdm926/aelf-boilerplate/raw/dev/chain/contract/AElf.Contracts.EvidenceContract/PIC10.jpg)  

针对该图片的测试用例如下：![测试用例](https://github.com/hdm926/aelf-boilerplate/blob/dev/chain/contract/AElf.Contracts.EvidenceContract/%E6%B5%8B%E8%AF%95%E7%94%A8%E4%BE%8B.png)   
