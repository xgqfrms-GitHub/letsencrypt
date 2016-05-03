# https://github.com/xgqfrms-GitHub/letsencrypt

***
***
> Let's Encrypt，免费好用的 HTTPS 证书  
    很早之前我就在关注 Let's Encrypt 这个免费、自动化、开放的证书签发服务。它由 ISRG（Internet Security Research Group，互联网安全研究小组）提供服务，而 ISRG 是来自于美国加利福尼亚州的一个公益组织。Let's Encrypt 得到了 Mozilla、Cisco、Akamai、Electronic Frontier Foundation 和 Chrome 等众多公司和机构的支持，发展十分迅猛。
申请 Let's Encrypt 证书不但免费，还非常简单，虽然每次只有 90 天的有效期，但可以通过脚本定期更新，配好之后一劳永逸。经过一段时间的观望，我也正式启用 Let's Encrypt 证书了，本文记录本站申请过程和遇到的问题。
我没有使用 Let's Encrypt 官网提供的工具来申请证书，而是用了 acme-tiny 这个更为小巧的开源工具。以下内容基本按照 acme-tiny 的说明文档写的，省略了一些我不需要的步骤。
ACME 全称是 Automated Certificate Management Environment，直译过来是自动化证书管理环境的意思，Let's Encrypt 的证书签发过程使用的就是 ACME 协议。有关 ACME 协议的更多资料可以在这个仓库找到。
