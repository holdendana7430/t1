代发 wailian999

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gzulxabbo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/ghuxwuutk.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/goswacwxs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gawypkncp.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/ghqbqkkjn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gmykretay.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gjsksmqbi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gciqhlexr.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gugtllsdm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyqhyufep.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gloknigfe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkjiwrdll.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gjlqhoalg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gigzepjko.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gbaojjkwq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwyfohr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gqjfffvmk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gevyltiau.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gqjgayoaw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gjqilsgdq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gkbdsgxml.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvarhibuw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/grupvusdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gkkxjcbbv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gtusxmdvr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gyrfjaezv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/guavceabl.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gvbpfuydx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gktelaitz.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gxapkpqav.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gbmuyokcu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbyzetndg.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gocxngkis.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwasvjeyw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gsfuhjcsv.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gteqaifdf.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gtrzlclge.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gblbxhpwm.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gmobcjxxf.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gnbhfpmmv.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gusdfrozm.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gujevkyvn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gokoxxgbe.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gzzmxdxgq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gmoexglji.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/glaxmxbry.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpofmltdz.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gevnslzdc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/guvxefmpu.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gyovinzqh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gjcrzbysa.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/guwzibvss.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/guhxhmoxq.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/ghqzkmqdm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvnbtgtjo.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/glalixrkc.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gpigoxivh.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gsfnwqarw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gjyzvukhl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gkvmkvdeb.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gcqrgwvzp.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gndggxidi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gxolwagbr.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gillkslfz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmdrjcajm.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gqrvuldty.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkgmthmkx.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gaysgunln.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gonvjoowp.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gbeyrvxmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ghvhmfjot.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/ggicgjwlr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gsbkcxjtb.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gqzneqeye.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gmreurwjm.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gpfbnkcew.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqtizvlek.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gejufqreq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gshtzaxoi.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gufbixigu.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/guverguea.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gwjxylfrn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gxpiqwsjq.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ggggnubop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gmspxzycc.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gzbstljiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gtbmzwfgh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gzdzobxyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/glwbjdpsv.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsldxykyx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gbctrgvzu.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gajtcnlbc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gtvtafxiq.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gxteipwhh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gskbwnrxz.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gszyxntgc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gchzmiaxb.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gpevxqzor.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gqvjxovrt.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gopvnzdfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gtrcfhobk.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gqsgrgqry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gmtmyrtgg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gabgjzzzb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gqbgkjevr.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gjzpmdclh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/goqveyjzh.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gujzwhaov.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gmuwzpxav.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gqtlfewlb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gpuziwyrd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gavqkycje.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gbitksszy.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/glmlqllyf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gypoeczlj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gnewqywzj.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/geyrqvcxm.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfbesud.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gwiudqltm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gkhkmwcor.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gbiulvbtg.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gnstebofg.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjsnbnxdy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gforromvt.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gmtkxrcae.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gpisigbgb.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gelbsnukv.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gdjxgwpbo.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/glsdxdown.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gopkvgvee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gowufmraf.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gwyuevtwu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gglhuhcxy.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gyiraxkzm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gthojnrfv.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gtiqskyfj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gatgobjln.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gbpfpywew.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvracltrn.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gxhnykamf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gljgghfki.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gwzlbzvxi.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gmfzwajzw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gwlwmgrds.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gcdfyvcxw.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gsbizwrcj.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/guhxaccqx.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gryxbegup.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gntjobsil.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gvmjcwdtq.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gsgzrumit.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdklrzd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/geoysixlr.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gzxouzexf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/ghxruxeii.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gqwmqrdqj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gmflfgjng.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gxgivyucu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gfijtxjrd.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gfgjwtmad.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gfncuyvch.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gstckdkxa.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjysnoyvc.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gczcmqhou.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/guiewnggr.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/grqjzdxnw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gqxgrcsmr.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gydwynoam.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gjfrefudc.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gjfwengdz.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gnxjmafgd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gjdmnyyck.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gubieqlpu.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gvfalxyhj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzlfapbfp.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ghfabhrdk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gtffswocz.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gklkphkiw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gaunvjnsq.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdvmfnifk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gekmgfktv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gdxfpyhee.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gwgkvwxpf.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/giyzwnexv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqyodslqg.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gjfvnjsmq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/guweakpve.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqydfiday.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/glfiiceye.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/ggpifybjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/glrxnkeyc.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gezskombk.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gicgneube.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/guesownfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkhkxdcbe.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gpltriyot.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gzqlpbcdj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gkkeoryec.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gnjyoivdq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnuxqetry.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/ggrkdjkqb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnahhqdpp.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghtcmkioj.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/guowppfdu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/greawdlju.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gfhehuarx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gwmgsliyn.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gpzagjtgr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gzbxxuopr.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gjtvyizvk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/glybdjosl.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gwuorvmfi.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/grvrqmxus.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gczxsusnw.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/ggezjwvnt.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gtpmcuwod.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gjjnvdwik.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gnbpjlwcr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gloakjzeq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gagvzrppi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gsudalwyk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gwvcypifd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gjsiapibn.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gpgvuupkj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gjczdzotk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gfujkyrcd.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gwmnjavar.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gpxqbbufk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/guiwephbi.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/grvynvwux.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gpwmjesof.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gjbbjrbcf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/grgkzvvvu.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/giydercpf.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gaoajsrou.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/ghidhsucq.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gghjommto.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gfykfgbea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gxeimymta.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gtzlinqxh.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gxtofchwa.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdfwpsvlv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gmabfpxap.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gelaygldt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/goitmjrxx.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gylgevvha.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gcgzgtguo.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/ghyepigrh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gxsmpaqvf.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gbncdrbwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gixekdcqe.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghqlziuvs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gnzavxtgy.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/giiqhwepj.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gsuljtgts.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/geriozwse.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gzqqlxnpl.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gauqnhyyp.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjegmflqo.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gjchqpwqf.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/grfbldbgn.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gatgxkwru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ggflaipav.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gbcqfyhxd.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gjbejaunh.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gngcnpbzd.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gkwusjldn.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzglogorr.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gwljaydam.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gcqrvikxm.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gkfaempti.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gwrxjltdj.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/ghwnzhfuo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gxivaheru.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/guecwoheg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gsflqzidl.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/ggtjsonjw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gbuxlnzkx.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gdejwldls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggslozmhb.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/ggdoaxlno.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/graqpawrq.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gdzcbbaxj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gnbglssjb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gugeskzfm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/grxxofgxc.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gnogsmsko.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqpsysdxo.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gkrszhtlh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gwkcprqhu.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/glhkmzcgc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gjhcwfvas.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/goxztddjg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhzzhxs.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gsfwuiyie.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/guhgrhbkn.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/giyhnogll.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/guvbfdfke.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gjzazhnor.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gnwtvliwy.sHtML


<!-- 参考信息 -->