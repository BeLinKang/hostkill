# hostkill
联动xray子域名扫描进行host碰撞
使用xray进行子域名扫描并使用脚本将其中的敏感域名以及ip进行提取。最后使用host碰撞脚本进行碰撞。
# how to use
./xray  subdomain --target example.com  --text-output domains.txt && python3 hostkill.py && java -jar HostCollision.jar -sp "http" -t 1 -o "csv,txt" -ifp "./ips.txt" -hfp "./hosts.txt"
