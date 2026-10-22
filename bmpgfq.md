代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2onfoxmlt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pgihijwc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xpimhswv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wwjczwmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kaseksei.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wdyolwmw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxudirnm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pavlcuxc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzwpxf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2phdunjnj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2momhnhmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bvjzounw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qkuewkfm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nvglnbai.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dtuasjco.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wsebjlym.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dtqihaqg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hemjnaou.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2quiedpna.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jyvdfdje.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykpzsnst.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibqkwmcc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2prpqgwbn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkovqtmu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vmtlivta.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvnnahqc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vhwcgadq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lbkcuzsh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2joqoqiby.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2orlsnjnr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2loldnhpu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pcobkyrx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ccwvwqgm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2nhkeewyb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2proesaht.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gyavtque.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekypafpi.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nigalukr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ppbtrxlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxbduvrh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fmuoudmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngdbsfns.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yuydqjsu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kjnnfgqz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2iebtatzk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2onfturtz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xjxrxwqy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nxhsaopv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mmbbrxih.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fvvoezir.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rrkzjsir.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ssfeoesu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wnadjhaw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2banqpkwa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mlcvbmpc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2iawhfqgk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qmphdspd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nfpngcun.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pzkklqvs.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgiqxkkb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qvneyqpl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2haxzcimv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wxrbxrwo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jmxwuutv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wutyjlls.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fkbdcrqt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2sqtsrqii.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kqsoiwxh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nlbuvfdd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2aittczsm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rebtdbjc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xxstbjok.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2khytozrp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2arebunru.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nnzpdkho.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ietztqrr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wcosaeou.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fywvbhvs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fxjeaovn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kgvmckua.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2lmlhxjbc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fnulufgc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fkicjfkr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hwmkelfo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxaulnb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fbftraep.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wgqmxmhc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qwkjlfyc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcqkhwkw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2shxjsivd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pdflxdwj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oilrpvqs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2psfakbvh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xnrzxxep.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2shdlodmp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dstemdus.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrokpmbi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mtjfvwme.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sczpsblp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dvxgbhod.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lirwiwqu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ujpxxfis.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jmpclbgu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwpcqfym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2eozzdoew.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ktvutsrv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fwnkuxfq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2omaclavh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyxmfpcd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pfawmsnf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2swtmvqqy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ztrtvkkw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wpguvocb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2pkfaoiwq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ehkwwwio.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ypufusep.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ddienmlj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eqzqotng.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vbawspcz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xjdrokyi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cfyffpmi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2onczavwx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jlsuwkkc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2swrlnlck.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lhvcrnzs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2anzlloee.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pgffmhad.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ekfsyqnw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uuwwzhlq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fdezlntf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2airtybvb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnrmvxhi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fitbwqij.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2poaalobx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vkjplpiv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2npovbixz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gzvjcevx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2anedxczd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rofuyexo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ofblwpmn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfpwqhsz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bsypkcse.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ipzvrrjh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nlpqqprp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2owrgtexn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jkbrmppq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2spvccpzr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2imlcriip.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vtciibgp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dgsnozoc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2whaubker.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ovwnsgsc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hgbwbtwm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pvwlctyn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2myfkvzap.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ldbccmho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sqcurxmh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ewyfzwso.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bisivgyp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rmacabmy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2stfzkgla.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2czmqlrzv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ootslwvd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hnqzrrwt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kuthprer.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gjydposk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vfapdvqf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wyqxudja.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rqxmfdog.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dwsfbeya.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2acidygoa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2icbzeiyo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ioswwwcn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ndvazlor.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ghzacwqp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gajcqvwy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dflhdcdy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bixgcyln.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jqaszmes.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qxozxjzr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kwfisjdq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rzhyfzxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cllgxzso.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rwfklsmg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2owmgqwty.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bojklvwn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ohmbsobx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2epkapmun.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tbrcuhmy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2begkseun.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhuwpkox.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ofljgegr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kztnhkvy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kjnqfxbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uzouktlb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxhspbmm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2aaycfywt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzaxmkqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bavnmtvg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hlbepuky.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vfhozwbs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jvmjaeic.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2euyccxog.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2karggwsg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqpibgfp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mxgfstly.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2knulijpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mohubqkx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kyxwzsta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpzkvnfj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wyuyopxi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dpvszois.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sfgngaqm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cvzldcmu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cswcusrs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qwlkycas.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2azjapyse.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2grawquau.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pbffpjmj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qyclnmpg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgvpmhc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fqyucniu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2quktodql.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ojgurtqo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sgszvirz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xwkhrsbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hdzubfuj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dvrlrvir.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dkqmbfvq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rsjjdwsc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dzjjkhyh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fexvujsh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rrinhhia.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kcfamydk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pmewwrzv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pujysxmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lnpgbosm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fniecmpb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pxwdpgsj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qqzyhxac.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2slhciyhn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vlafqcsi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2musdrzgv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2sydsmzzi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jpckrqtg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfbcjhft.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ldifkwcf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ovaagjft.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bfddziof.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rioqxqfn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ckusuvpm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qygzmjkc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2moqvagtb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zmpdmymu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jbmjrgfk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oqsqzxmx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yfvdfnbe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sirtjrpx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2meonxrcx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2diwgqktt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dtjpkcdp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fhkfdeuj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sfjrjwrz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2affdvfht.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zujvknjk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xzixwwlp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxuolhip.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2slmxejeg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hnjvjgox.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ztqqfzjd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uhtdmzfb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xglxxxnw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vlqqsetm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rngdbmmz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ylttdiif.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yrzxduck.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yxqalhyf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrboesqk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bgiwfwvc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ikfbeeam.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xjicfiee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qkcrnofa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hjaonhev.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cqbavzyb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2huwdcafa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ecgoxbem.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pmsfbgbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zeolncwa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nyqowsns.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rbawnpgd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nzbwgmld.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dfyvsfiv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jkqnftew.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2olnieiqy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2trkpmvna.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zrjsjuvt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gtebnxil.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2aoibumjf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdsqexxo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xvzdkgne.html


<!-- 参考信息 -->