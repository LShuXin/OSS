Region表示OSS的数据中心所在的地域，Endpoint表示OSS对外服务的访问域名。本文主要介绍Region与Endpoint的对应关系。

公共云下OSS Region和Endpoint对照表
公共云下OSS各地域Endpoint如下：

Region	Region ID	外网Endpoint	内网Endpoint①
华东1（杭州）	oss-cn-hangzhou	oss-cn-hangzhou.aliyuncs.com	oss-cn-hangzhou-internal.aliyuncs.com
华东2（上海）	oss-cn-shanghai	oss-cn-shanghai.aliyuncs.com	oss-cn-shanghai-internal.aliyuncs.com
华北1（青岛）	oss-cn-qingdao	oss-cn-qingdao.aliyuncs.com	oss-cn-qingdao-internal.aliyuncs.com
华北2（北京）	oss-cn-beijing	oss-cn-beijing.aliyuncs.com	oss-cn-beijing-internal.aliyuncs.com
华北 3（张家口）	oss-cn-zhangjiakou	oss-cn-zhangjiakou.aliyuncs.com	oss-cn-zhangjiakou-internal.aliyuncs.com
华北5（呼和浩特）	oss-cn-huhehaote	oss-cn-huhehaote.aliyuncs.com	oss-cn-huhehaote-internal.aliyuncs.com
华北6（乌兰察布）	oss-cn-wulanchabu	oss-cn-wulanchabu.aliyuncs.com	oss-cn-wulanchabu-internal.aliyuncs.com
华南1（深圳）	oss-cn-shenzhen	oss-cn-shenzhen.aliyuncs.com	oss-cn-shenzhen-internal.aliyuncs.com
华南2（河源）	oss-cn-heyuan	oss-cn-heyuan.aliyuncs.com	oss-cn-heyuan-internal.aliyuncs.com
华南3（广州）	oss-cn-guangzhou	oss-cn-guangzhou.aliyuncs.com	oss-cn-guangzhou-internal.aliyuncs.com
西南1（成都）	oss-cn-chengdu	oss-cn-chengdu.aliyuncs.com	oss-cn-chengdu-internal.aliyuncs.com
中国（香港）	oss-cn-hongkong	oss-cn-hongkong.aliyuncs.com	oss-cn-hongkong-internal.aliyuncs.com
美国（硅谷）*	oss-us-west-1	oss-us-west-1.aliyuncs.com	oss-us-west-1-internal.aliyuncs.com
美国（弗吉尼亚）*	oss-us-east-1	oss-us-east-1.aliyuncs.com	oss-us-east-1-internal.aliyuncs.com
日本（东京）*	oss-ap-northeast-1	oss-ap-northeast-1.aliyuncs.com	oss-ap-northeast-1-internal.aliyuncs.com
韩国（首尔）	oss-ap-northeast-2	oss-ap-northeast-2.aliyuncs.com	oss-ap-northeast-2-internal.aliyuncs.com
新加坡*	oss-ap-southeast-1	oss-ap-southeast-1.aliyuncs.com	oss-ap-southeast-1-internal.aliyuncs.com
澳大利亚（悉尼）*	oss-ap-southeast-2	oss-ap-southeast-2.aliyuncs.com	oss-ap-southeast-2-internal.aliyuncs.com
马来西亚（吉隆坡）*	oss-ap-southeast-3	oss-ap-southeast-3.aliyuncs.com	oss-ap-southeast-3-internal.aliyuncs.com
印度尼西亚（雅加达）*	oss-ap-southeast-5	oss-ap-southeast-5.aliyuncs.com	oss-ap-southeast-5-internal.aliyuncs.com
菲律宾（马尼拉）	oss-ap-southeast-6	oss-ap-southeast-6.aliyuncs.com	oss-ap-southeast-6-internal.aliyuncs.com
泰国（曼谷）	oss-ap-southeast-7	oss-ap-southeast-7.aliyuncs.com	oss-ap-southeast-7-internal.aliyuncs.com
印度（孟买）*	oss-ap-south-1	oss-ap-south-1.aliyuncs.com	oss-ap-south-1-internal.aliyuncs.com
德国（法兰克福）*	oss-eu-central-1	oss-eu-central-1.aliyuncs.com	oss-eu-central-1-internal.aliyuncs.com
英国（伦敦）	oss-eu-west-1	oss-eu-west-1.aliyuncs.com	oss-eu-west-1-internal.aliyuncs.com
阿联酋（迪拜）*	oss-me-east-1	oss-me-east-1.aliyuncs.com	oss-me-east-1-internal.aliyuncs.com
说明
关于OSS域名的构成规则及使用方式，请参见OSS访问域名使用规则。
oss.aliyuncs.com默认指向华东1（杭州）地域外网地址；oss-internal.aliyuncs.com默认指向华东1（杭州）地域内网地址。
①与OSS同地域的阿里云产品可以通过内网Endpoint访问OSS。如果您是ECS用户，建议使用内网地址访问同地域的OSS。访问方式，请参见ECS实例通过OSS内网地址访问OSS资源。
*标注的海外地域与OSS产品定价页或资源包购买页面中的部分海外地域在表述上略有差异，但代表的都是同一个地域。例如，美国（硅谷）地域也称为美西1或者美西。更多信息，请参见OSS产品定价或购买资源包。
IPv6、IPv4客户端均可以使用OSS提供的统一双栈域名访问OSS。更多信息，请参见通过IPv6地址访问OSS。
传输加速Endpoint
Bucket开启传输加速功能后，会增加如下传输加速Endpoint：

全球加速Endpoint：地址为oss-accelerate.aliyuncs.com。传输加速接入点分布在全球各地，全球各地的Bucket均可以使用该域名进行传输加速。
非中国内地加速Endpoint：地址为oss-accelerate-overseas.aliyuncs.com。传输加速接入点分布在除中国内地以外的各地域，仅在中国香港及海外各地域Bucket绑定未备案的域名做CNAME指向时使用。
更多信息，请参见传输加速。

金融云下Region和Endpoint对照表
金融云下OSS各地域的Endpoint如下：

Region	Region ID	外网Endpoint	内网Endpoint
华东1金融云	oss-cn-hzjbp	无	
oss-cn-hzjbp-a-internal.aliyuncs.com
oss-cn-hzjbp-b-internal.aliyuncs.com
华东2金融云	oss-cn-shanghai-finance-1	无	oss-cn-shanghai-finance-1-internal.aliyuncs.com
华南1金融云	oss-cn-shenzhen-finance-1	无	oss-cn-shenzhen-finance-1-internal.aliyuncs.com
杭州金融云公网	oss-cn-hzfinance	oss-cn-hzfinance.aliyuncs.com	oss-cn-hzfinance-internal.aliyuncs.com
上海金融云公网	oss-cn-shanghai-finance-1-pub	oss-cn-shanghai-finance-1-pub.aliyuncs.com	oss-cn-shanghai-finance-1-pub-internal.aliyuncs.com
深圳金融云公网	oss-cn-szfinance	oss-cn-szfinance.aliyuncs.com	oss-cn-szfinance-internal.aliyuncs.com
北京金融云公网	cn-beijing-finance-1	oss-cn-beijing-finance-1.aliyuncs.com	oss-cn-beijing-finance-1-internal.aliyuncs.com