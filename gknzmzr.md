代发 wailian999

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqiwwetq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gulvcupls.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgqprnk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gmyzagruu.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/glqarsosg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/griiuhhbd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruurclbg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gidxfplor.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/guwttzsbs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpofrvjm.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnlwcujlf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddmsbzrn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gnucrbimk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gasilkfox.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbdlqhsk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjansslnj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gatjjuxqe.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzkbxdnln.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gvitbeecv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gwnekewic.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gujjfsfcx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gncbqormg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gttzzwzsk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbwyfzma.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/grkyxjxly.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpeitzop.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbycwqevw.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grqwpofch.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gzpazrnqx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvoihdnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdwfajyb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gweinodec.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/guntmvcpe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkctgdpd.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxljhwjt.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gximizcab.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqtwdsvu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghigswsdt.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gqlmlktyu.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhanclve.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/glwxmlxtc.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxoronbxb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvvpsbi.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfxbmlus.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmioqbn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gplivpenv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqhjihng.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkxdtaqug.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvzprytx.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbwchzwtn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcomhapfc.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdiuzjzzn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfkojejvy.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gghxneerr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsswwlao.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeadeytf.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gardryzgu.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtxejnq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnruwpace.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvcizeow.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gujzotpsf.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfukxddd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsewmhfen.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxllnvdt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geiicfxph.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gsibckvtt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwkmolx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxxcopwe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehjlllx.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdytyhlmw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymtxoml.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtdzpzcf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gegvmngks.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/guaepbvby.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gumsplpis.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gaklbwtpd.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqtkclmz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtydebgqi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbbvfbkv.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/griumdrow.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjexaasqg.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcvqvkrb.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgffvxpz.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gclypwdoe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmxvnrjn.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwfzcdco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuhebgiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlrpxdgo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gudembdln.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxrruloa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbpcpye.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gfbjtjnfm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gpqwrmgha.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gmgcyqbah.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gocbwvfoa.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaurfbxj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpsdohjl.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaultphg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnuzczyy.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjywmigjq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfwqimcap.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaozfxqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfkhamihd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbwlmch.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbxdvqje.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gjzsupzly.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzzqofdhs.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gegwqvdcu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdnvzsjo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijhapxu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/giakyuyhg.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxrlbltlb.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzwhrsjp.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/ghggaqtem.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gfsoxkceu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gaijrjnzd.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gikqlilae.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyefjjukp.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gofqibckd.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrtkgxsj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgqoxlxi.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gvzjxhkxu.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcascvc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvudzwbk.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gecjacmwm.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gpdzopits.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdegwmwlw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/geymfuohb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gegzkyuly.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgtcqwac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/goukwvqws.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpakekdui.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgmzdepv.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/giqhcfjub.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzjuczon.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbdhmxtkb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnueyqxf.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkthgxtoy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbiyhqsex.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gcuhblzrd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gisecgyhx.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gmfqvxpyb.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejgrqssd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gmraixbuc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqvihekn.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/georsrijc.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldzvbjjd.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gefhicnzn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gyjxqjxgd.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwpkvlcfn.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gstvgsqdo.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gzjdxddmf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrjzfvii.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfpmsrmhr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gzfatuuuz.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gacupwmcq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gdqagrtzl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gtoddllkj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gfytpsfvd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavylbkfr.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gavkbnmpx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grdrmoqxi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gribbndfa.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnmfgmehu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmckvqip.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gctayjdgg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gjzhqacfc.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnlclxyf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaxdotgy.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkcohsngk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvzzbwbw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtycyecf.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlkpblzz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzylgxvzo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqtprlkgv.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/ggkumtbnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gououqlez.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gahumyhgm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gjjfhxwwc.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/guikwhnne.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/geubxxrjs.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gpukoybog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswizyudf.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhuvwbhz.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gugimbexc.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyfroyeb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghauwvjib.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtycfkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqdbhicb.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gipoonrve.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ghznqymvi.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gdibxgmih.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gacfdtvmk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqerrthf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqhfeqqbk.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gfomtxulg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkhtwbsan.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmnnndiu.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmezsue.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtjwgalg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gihhmcwkh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrogiiln.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gurrrnand.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbsfjlgk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnbxxtcf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/glwjkiinu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gvgatqija.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/glwjujnhh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gwtnjnuqk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgoobdro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gofrzmdyu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glauqptsj.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfkyeaga.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnncdrcwa.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gttihbauy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gflnjzpbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/ghcsiyark.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gktitwpmi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxalsgi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyxplbja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gutmrfgtk.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gyhfcaizs.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaimjeqs.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhgxsjgb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoijgorr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuklckak.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmfpwbok.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxwgshoh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzngsdb.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/grtshqyjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gnjulqptm.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gfuckrnpl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gcnqswthy.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyfdycdc.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/grznbiyde.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gggpsfrnj.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglplxiue.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/geftyyumt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gcykgnuso.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnxlqlf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjgoqhzt.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/geclquhhm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/getojyhzv.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbggatnf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzygluewo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gglnzpxvy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnhfmmqs.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gnombdrpd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gijvuqita.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gpzhtaqrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gghamklgv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywucsafx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/grhrwpqsp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gquguiafq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnpucacl.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gzciixbxc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxlupbcg.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwwyrvxkf.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwwlnckbw.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzadndar.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnxgwaql.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnvyjdtif.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtmyiosf.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnfdcquc.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gfbekljte.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/glllmuqjg.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gqqioslgz.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grvyruwte.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gdjryqthz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmeyjbqix.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtcoevga.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gcmlhumah.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/girzmilwz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gheqkecsm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlnvqzjz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmdepczig.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gnwmdbpuc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipgbfrt.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/giqpbejpe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttdgtmd.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gvulddbbg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxqwtqli.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfvketu.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnfdpumi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhmvydfy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnapmlxy.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdhdncoat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/giqcmjiqb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfgechva.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmbcvxccy.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goaenhznp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktbvdqk.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gjlmllgzx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgbzlmhs.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/geythosjx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmgiahllz.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gahnaejoi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxbqyhhn.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gqenybaiz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqnclfma.sHtML


<!-- 参考信息 -->