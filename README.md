# chinoukin.github.io  
change 2025-01  

首次在gitbash存储github密码  
1.  
git config --global user.name chinoukin  
git config --global user.email chinoukin@qq.com  

2.  
git config --global https.proxy http://127.0.0.1:1080  
git config --global http.proxy http://127.0.0.1:1080  
git config --global credential.helper store  

3.   
git clone https://github.com/chinoukin/chinoukin.github.io.git  
cd chinoukin.github.io  
git push  
为了避免非github项目也走代理，取消全局代理，在本项目中配置代理  
git config --global --unset https.proxy  
git config --global --unset http.proxy  
git config  https.proxy http://127.0.0.1:1080  
git config http.proxy http://127.0.0.1:1080  


4.不建议用密码登陆github,用token登陆  
git credential-manager github login  
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  
  
5.退出重新登陆  
git credential-manager github logout chinoukin  
rm -f ~/.git-credentials  


