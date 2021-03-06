# 京东票据

银行承兑汇票由于期限短，便利性高，流动性强，已成为很多中小微企业普遍使用的低风险金融工具；企业通过票据贴现，可将手中的“票据”变成“现钱”，加速企业资金周转，提升资金使用效率。 但中小微企业和金融机构长时间的信息不对称，导致票据融资变现一直是中小微企业的心头之痛。银行授信及贴现手续繁杂，中介市场融资风险高且中介无法提供合规贴现凭证。针对以上问题本系统为解决中小微企业“小、微、短、急”的需求，打通资产与资金的对接瓶颈，搭建企业与金融机构间的“桥梁”，**为中小微企业提供合规、高效和便捷的服务。** 

## 秒贴业务流程

该业务主要通过撮合银行与企业，平台通过对接多家银行提供其最新的贴现率等信息，为企业票据贴现提供一个合规、高效和便捷的平台。其详细操作流程如下图：

<div align="center"><img src="../document-illustration/tiexian.webp" width="70%"/></div>

 

## 我的工作

- 使用[文本图像识别技术（OCR）](https://piaoju.jd.com/fast-discount)为用户提供了更好的票据信息输入功能。

  <div align="center"><img src="../document-illustration/ocr.png" width="60%"/></div>

- 使用分布式缓存**Redis**，**RPC**和**云文件服务器**为银行用户提供白名单管理功能。

  <div align="center"><img src="../document-illustration/maintain-whitelist.png" width="60%"/></div>

- 为银行用户提供动态报价列表功能，并实现根据订单信息匹配报价功能。

- 使用H-ui框架为该系统实现了多个管理后台页面，供运维人员监测系统运行状态。