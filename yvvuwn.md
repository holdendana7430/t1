代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lxrutpfr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fpazjkdc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uvksqxqs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nzynurbt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zeycuqeo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iuveegkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jfaelcem.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3llwjjjbg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jsxifytp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nywoqxsg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nkngrnnw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yaujkvdw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rwwomozn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qcvvpzut.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mvappqia.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zzxgyiqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nnzrmqia.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qsmyfjzy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yezhthsu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gwzfrprh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vapejtsg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hutsnpdv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zucrfyec.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pozdpkpt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uvpbepip.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hfdcrsjs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ukenxqkh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ovckenbb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xcbdhvey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bygvntoi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jvfsiqif.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvbhzori.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hgjvcwwj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qiebjhfx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hlgbhtmn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etpebznh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3izujgrsr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ryhiarxg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fqdahjat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ibstwaps.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cnmjqqtb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3waupkwkp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vdqrhcsx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ihauxmix.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3aakjvylt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sqwmfgms.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skuyzcmj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gbvjxmeu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zubgxsbf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vvwmuwae.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3iodcihmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjtymtyf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3seukwwhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nosykzio.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qkohrlpx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jrcfmynm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zabgtzor.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ecnapoml.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fskcsqty.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sxzcigxq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3umchxufi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ilmcfgqb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gblbrpuz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ijwlowib.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xysdsmoj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3imughnog.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3otvpwodd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssqyrlzi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rncrrlks.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ztvjmvjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iymcsfak.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kqtvphvc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mqwavinu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xxkzhmqw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3srawvaqh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nuomaohl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wzrdaqbn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3urshdgvq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3judlfoos.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3onbdthst.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hgcneqew.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xiwhfzzw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bzjdbekt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dveloxpp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ppvdqdcu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dkjenccx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mrpbfjyo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkgtsxrc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pxtfsiht.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hobhssap.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wwwfpjfo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xthapjab.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bpxaxyrm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qyrqsord.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kosydtxk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vmtwkdcd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tspmrlzh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rijxjxic.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bsngdhdj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yhlrjkek.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mgpftwju.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rdpwuzip.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aoyypvgl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gytmwzuq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hysufwib.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uogncnai.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eevhvoya.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zhhtcfot.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3todvimkv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbqzmywg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tgrtvnax.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kucqewmj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uryhfpuu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wiwkbkab.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bkjxcbou.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uhrtlhtz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3visxtpfe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hrshvgkx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qgaxelpb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3phuahlky.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibrymdsy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3jwipqisx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hnoscola.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rjcrhnec.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pdlgwwgf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mdhadjdb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uqqemric.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3anbylndt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vkqbyeen.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ctqpgcou.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qwmrzirf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ouyxtonl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3owrobtia.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3creuhdaj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ntgpsgwz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3oorbvprd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fllolrjp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lwmzfvwa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3smfbwuet.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pmjqhnjp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lgpauube.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3djahojzj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3asycxmes.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpfziixs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rveiwkgy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ufsvosua.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jplrchvl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kbnfkgck.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zlkwyiii.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rxvzuuld.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yqexrxvd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lvhniqfd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3smwybeaq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fileitub.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ibiyikwg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yaninkfv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mqqxizlb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jbfjrntw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xnniogbg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ytxdkbws.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3aiebaliv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zyuggebd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ntsgallx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zlareexg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qhebnofj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rbqzzhat.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xfrldpvz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3eahjrwgt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yhvnqxgq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3sukqujdj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dnlqogif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3oaytbnem.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xrrpylgo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wqeiewan.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ensjqpgc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lzmkdmnr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vknregvm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mtrfrhgk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zlqxqwyn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kpcmcxzn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vlkdtxeg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3deiiwvlc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3niounbnc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qveyvkvy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uatjcbwa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zasdgxcl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmyxhex.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3imvpvxjl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jufdkxhy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3byuphros.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tlnamakh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dfjcjbyl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3sjdfaqnn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nviasxxt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gpcipthb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hyqqkchb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gdccbnqm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bwcozlem.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ywvzonei.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3glfpwuut.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ccwvaaqj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uhjaaagd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnhpfpxr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hmvrasgt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3msjjujlk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sgoayqbt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dnansynq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rbcuxhdu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3scgdvnqg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tvmowteu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pgevszid.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qpkbhrio.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dnybbefj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bqbowsds.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dlssjdvl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3avymaigc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uatedwyc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pdfniqre.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hoxyyzxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjzognbr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3smtixfvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoxobubd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3myonvwpl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kgvdqmgn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hpsjgfjz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zdnmogfi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uhofhhsf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3btldomrd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3camztpra.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iemrebgb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nxlrlqbq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3utoptydh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nlxxxtew.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rhodhdwc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yuzynaai.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3elxejbwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yxfugqan.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vntlcocr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qqpbteqf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3touzpmhr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3alrwznej.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3opzikygv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pgohfvdw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yychnkcw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vnxraqvd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jswxuhvu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bagrzqie.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xprnnimf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uvwlxddk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zlfrgrrq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eaofwlyr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wqrcucfr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vjbsjspw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3kduxwcaf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rfugjigc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xdkonugi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jmtavfaf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lzntvrqz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kgvqquaw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jrvovbaf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cyuqgacy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zrmcnwtv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3scuvrxim.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3isftqoru.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yzyseivz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3brrfbaec.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gjcyvmhv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iquyeuhz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dbqfevow.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pckkirxl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tikiktvi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3skcsgcgd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ybwpnrub.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3edmyrypd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kmmwyoxb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vkqscdek.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xsyzxiah.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ktbtjftc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sbfqpmrd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3epgzyjxb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3scrnnzfc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3shfxkvjh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jtuvccfo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ikbojffd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3poayuoup.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oazwiinr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vzrzqcdr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itdwlphk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3clcncuog.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oiafjexw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vpepvnst.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3riqvzzio.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qaxditqx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fhxdwubg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vjhdaday.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3csiwtord.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3natjrpqn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqlxkck.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3leukglll.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sxucemoh.html


<!-- 参考信息 -->