代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyixglcd.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdubqxkkn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gleimydjx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gksbcavel.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ghgsvfcvv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjmsfji.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/giyrxxggk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gijnhhbyw.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gtfoxwyeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlgceluf.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbnarvap.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gvzeleuqk.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gogzmweob.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbsjopwry.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyduymwui.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gekmgwsqw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuhzqzrr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeyzrxcx.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnvjofrws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqljxbsu.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gvvuppdsm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqlacgrr.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gqulemzzn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gbwfjtdqd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjzqkhvp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gktelhyci.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gokgaseaf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwsoyeo.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjcyyjel.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/grydnsges.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjmfbhk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqxzymlg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/geaizdlmr.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gjjkeltbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxfxnsjt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glpdxnyvg.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gnngrtjax.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grvirnifj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/giarbjkld.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjwuyvzm.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gjmhtzuoo.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcvsktg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvpnckgb.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpoaecik.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimaphapi.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctsvekhe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzvcgici.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghmjnygeg.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhztmyf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnqgsctl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwwpkoc.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkjhjwj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqbnqwtd.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gggwwpkum.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gteazvjjk.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gviwhxnqi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbziidim.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gfpupbkij.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gmsgitqdj.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscywieo.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gmqhieoqc.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdnzgar.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbryccyh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecldrvqv.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbetcyqf.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gclmklrhb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbsqqdmnq.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzaomgog.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupbtxlto.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ggchsuuww.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjhsteifh.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcdvpnwbh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggtiwyoi.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpermkmqk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/givxsyfia.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuodaqdx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggdngfseb.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gqdgxgitf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiznoyum.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvdwejwob.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfxkzecx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsddvpez.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggeqrmzqj.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glpomamqx.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/guurdqtln.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjztwpdjs.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhsjoctk.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbeyahnqh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxjlhsfds.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gacwhmyyf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gorggjbiz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaigcyus.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvbfplyyl.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjpmwwao.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gadrxifby.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyfspjta.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjlfsbd.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/glxegknus.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gagzdqflg.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvtclvum.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gesgmqwwa.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdbdmimik.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gklniihzo.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gknegxbzy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwxbkkrdh.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdimkwloh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqwrrboe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxchmmes.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gcwlzjlur.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gputzutub.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbderbz.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gculxzmux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbghzlwi.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gwlrtpdto.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdprrjqt.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpasnzwns.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrtbazri.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/guodiguuj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdoonyr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/glapoommw.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gpzqistpv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxankwwds.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmamdrrmu.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gavhknotp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gptezywxq.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gjkpootdz.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmnotmaa.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gativxoei.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifvdecag.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gubgeqfix.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzgffhezf.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhqeunaw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gddsbzipz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqbgdqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gntrjphzl.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldjkvjct.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqdltlvjr.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgzcmkuj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwpagadpd.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpeypccj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwqftvlc.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqeqemces.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueedpfgn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/geothclkf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlngcwli.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gberigaws.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gognqnxls.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzjreovx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gevprliml.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxllybigq.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkpjqlbek.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gerqvukbr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gagzymmjc.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gfimjxehm.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpvjcas.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtzvdlzw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhbmfazi.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwunpwggp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gsgbqzdjj.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxmyhcir.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkaowmor.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/geadcadxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/goxwnblbs.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gnownowph.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqtdkne.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjlnsnnly.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gzsaknjnk.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grwcsieqn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gylxpwngg.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gevyrdzlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhokkzdc.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/galfhfogs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkvxaphw.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gycsxzhqe.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gaydvniin.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbylsmhok.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfsvjqil.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gdwtkkmfm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjiksazzw.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfodkqvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxygyit.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvnxkumf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppqgnyrz.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gtwunyoju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gfrepnmpq.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gkinfrdzr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzcyuvkhc.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjpyhvlb.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/grrbyawjr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspscaaef.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtoralpwq.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfdhnua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gxpwtwbcg.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghurjanbi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyzzmphb.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/geneosgbt.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgbbfulv.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gzswypgtz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gshaemgxm.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpzhwzxt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpbwzxp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/grhdbxivs.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gvvfyzvzv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvixwlifz.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/guwsxhlbw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbwvnqqp.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthxucegy.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gddlbjvbk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gapihuxuc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gryruwqdb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnythlepr.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiihhyfb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphwwuuzt.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gsyudngrj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxhkobby.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgubldkb.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gltcmvszv.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdatinzop.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gbtoreugq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbouqnvt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gzkcrxjky.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gugmsafsm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemxueiub.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gjaqeovna.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbjpkpmw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gojcthunv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdisvfizx.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gksaagtct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwiuugqc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkufvfvch.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbstafuor.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsbcwqqu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghisxakgr.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrxtqpat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gwdpilhbu.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqvchojy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmzwnvtv.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqyfxxia.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdadmemn.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgxpvgqn.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gittunuyu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gngcemftd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/givwrjvja.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guuelnwdk.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcgylfod.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkxohflk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdpoynnf.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqrwmahhh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gvfnbitvs.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyjudndy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghytomthi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/geztkbjmd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gecakcnch.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjclarils.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gnhrvfwbx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvujzucfx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gydapriww.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/grzgtoalf.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhpvvied.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gvpxqiddh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gtnsvslbl.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gokwjpcvq.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/geowfvjup.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpjszimuo.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjznqkrj.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkxcjtdl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gsnyfobxm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhpbvcwo.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmnhmqyo.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gncehqceu.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gtosgnxca.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvuggolfe.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdoaatz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgddgqi.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/geslnqacm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goosglkwf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbuadans.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gywpmddei.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtedpyiy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geljfsvaa.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/guyvcdgdd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpvmjjfe.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfivbhad.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsguagrlz.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/goypajwrx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grnxcqdef.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmjvrrvbk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfkdgeusw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcdmsgbhi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflpoqoij.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnwatxov.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gefxrnqce.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuuyofro.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojblmaqw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbthswpjp.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gikpxuhtl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocfswdnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gasidgpnw.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgndeiwe.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrgvkfe.sHtML


<!-- 参考信息 -->