代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3stavvzna.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dzurcyhq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kduohpqz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gujjsygw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qreonnhm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lbgdjzas.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3surmkgme.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kjgxigdf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jmtqdhwj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jwfslafw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cmmmkokb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3uhhrtndb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lrgaewmt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oazqscru.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kuepyclo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3llfnmrdp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qzcvaxex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gmrraaml.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wmtnglse.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ylckwqbf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3zvikrxbx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3upmszdjl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gchpeltl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ithlqpei.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzwyldiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cunmwfcr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kpmecqkb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glqwdrrx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zvwqnxjp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ithsbwzg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3twcpumfm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uxhbgrnj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3oidlhwqj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mxdqyvmc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wletjfii.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ahqazchu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hkzuztef.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dsplpuxc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhbcqlhy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wvwgwfwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cemwmhxf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tjyajjah.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nydbrzpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbrptvka.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3iepvtfwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrdpmvic.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eqvstzzg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bujgzabq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mbrmiabt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bsdzmonz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3teyiohec.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nrgxbuim.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xepynvkn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntkxlusf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bdjuymeh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3scjeihun.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhqtlrme.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zipqeffl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3exgkyerg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfsefbkz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iysbnkuy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sxmpxawg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uiqyuafx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ngziwpfd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gmyupndi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rtgkclsc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vgbqnevo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ltggytlq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tumowygf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xrzgfksx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wtmhfpsi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gokruskz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3flcimdpv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztvfaxdu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqcqqevv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ricmcbhy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jilzsidl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3luebnoqh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3numdixkc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zlolaztq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqovzwvd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3btzrptoy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vkouqbop.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wohbnzub.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cfvjzrgk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jkexmkmz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mjckpofm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yrwmmgsm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qmypiwfz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yapphzzi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3azhmdsmy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxjmjdtv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgqoakic.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3acbscmoq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gsmwycvm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yafjpomj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vjfokktr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rjbtbvxq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wikvsjal.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tdshogsq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hwltgyrm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jgyqhxzz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uvaiuwnm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3oqmvqzrp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3egzuvcpr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3lbfzisfx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3smxftlyy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzjdppzs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvpbyuno.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ewkunwwq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lzqfnzhg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wmwoqftl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhjlunod.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ehzadymb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xcnxdeqs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cfjuomua.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3uzhccoun.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wdbqrqvo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gwtmrimu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qoxuvjyh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fdlaywlx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3prsghija.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dmnaozhd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uykapbcz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zwrfuvjd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kwerrbzz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bquxdofx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gqfqadpo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rhemxjmj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vxgdrxwi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3teamozvw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vkczovae.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3csrkcfhd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zjgzircm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dunxgtzi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bvzeurvy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iiqtczan.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gnhvnzhu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3atvxxbmd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hchncfcc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bncbouxb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jrbdhlvf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dwhgfvyp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zgfvtlzb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oveevnnu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ebydfhee.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bnlbylpj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gkmbitgw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jyhismeb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zyqktbcr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kgzsaojt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jvlkwylp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bbbakbnp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kzjqlrtf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ihwazoxf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3urtfnvyt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vwdoeqdj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zqtnsjoa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qayngxvq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3osmqzrsd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ytmandwu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tmcmqfcq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3icszsuii.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ynmnkmqm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qnidwbst.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xcxqprjp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ftgytopo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wqggpeeg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qeobgwol.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lhnuqoqu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3oinrjitw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ucdlpxgc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ckgeouza.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3guinmpsh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3oatghhet.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3brwhfztj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qnszradf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dwgcezhp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sodxpfbb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rfcgkvtk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3whsmvpnh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eodnizil.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3oiebtyph.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vlttbmnn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gflzatfr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3okaljyzk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lniptjuq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wutcbpos.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ewxpkiwj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dlzttcmk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pqrfhjrs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jwqbzztm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gadfzrnj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eetitcrl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rundqach.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xbyxclrg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kmsbixyi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bfwppvim.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgmpyvbg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xdptzxsx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rekmazhw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzwovejx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nlsnnfcu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cktztyzd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wpciscrk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3whmtyciu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lrvzggxt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3npudaver.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uofyovsu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cwzmanyv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3oqvoambt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtjrmpne.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3avfjhtkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iocomqid.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zmwlvqjl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cfpchhyw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ldhnrxtv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tpmbxznq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3grmionav.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nisjbbtr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ylojrtum.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tpaipqxq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kdygvyqz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ycatqglu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bqksyzzr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3urggecdx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qugoekll.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hsjdgokj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gtragtcd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3twtukdwt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kobxhzok.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3spqhwumg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bggghnoo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wnfwfpsp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cfnnyndh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsjtrnzl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3exwzpqgw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fpadwuva.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oymvcvjj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xyfwtiag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rmzpuvsq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tyychgtk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nrkvkuuv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3luqygqyd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wuutnkwi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvznlver.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xhylshke.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hajfzrim.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sntawoir.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tggxircm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jsfiinfy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vslyllsh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3csbmvxwg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yletfwsu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yydohyrc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oaeabusi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wwqyxmgx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dqaohbub.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3veyipgwh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vsomkrfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ucgwjjzb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bikjmdnw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ommhzbuu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zpdnozfd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qjgufwlc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3amkurtqe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oauztzlm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tfjrzhpx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pdasjdla.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3scusluch.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cjvefimv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvdzwusu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gkqfgsje.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vhmjvvgp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rhrjwjto.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dqrmudua.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qtslmvds.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jadjwulz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3msebnpvx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3divkrsjg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3peschlbp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gvugdins.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cngesgjw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pciwexil.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rgxhawsk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hinfuvbb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3eowimnsa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3szpfgaiw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3odoihqfy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ppoplira.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tgijzmfo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dftikrrs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3iydafjqa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxwbziyd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cuefcpeh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tcvwsbkb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3sbzpiesz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eklprqwq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yeafqbxv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3issrgepn.html


<!-- 参考信息 -->