代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rtgiwwkk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kegluyuo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ocuvzfez.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2neqwmfrv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2uoykgivz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2clheuoqh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qthdhdlp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wikelyzd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yyuozpxv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ezffojdp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ehwzthjd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ffnfmzmo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2isbfpfno.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lxwczicm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2iduhzlvw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ccgpgnyk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lkndldaz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xxttxnzh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tsjduaea.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ppauawrs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xmjozbmq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pqcmzgfg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kubnjbkb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2aolhvqbr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2exskxtwr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nanmptom.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kluxscvw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2haejsqsh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iejrihsp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2batvopsx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xtiauhtu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hewupuob.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gddtqwos.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vjbxrxmz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iouvgvaw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nsdfbkei.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zxefwiwl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2sqibhenz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2iworytge.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2urlivqhp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2aufcyghi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ydsomfta.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fdbjawdn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2snnfybad.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hkqhgkjp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvqvgqfd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fzqiqoya.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwccrtgg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2linimpva.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdjrvxxu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cutjckox.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spwbdwvz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xrzljdxh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eporxlkx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gixhvbbz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fxdmmhxr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rdtejjqg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jytdomvb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dpasiyow.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2idqvaxim.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zqhvyqsl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2khgjpjal.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvfuwbuv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2avzkpmka.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bivwbnhd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nqnmskxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yiulazgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfwmkauq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yfkxkcut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofwyggix.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2byyqhupp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hlgdsybn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2deoaygkn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jqsrcopm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cekpxlmq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mxghbalj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sgtvybav.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zkrqeymi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2perdhnio.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qbuuvlzr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2liflhxfg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2umapmvri.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sbrfxjyk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzjowypt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cgxyzliv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hzknaofv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2prlftxhx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uzkqogrv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fidfczio.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xqhsdsmg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zeywwram.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pfbyshtr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vksdvefe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mwkmexmt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2issbghcw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eoytxnyd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zrpitjer.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkaxcncy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ubkeqjye.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rekqmebr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2runtidrc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tgamlatn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mamzdrms.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnbkycuw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jkpdgyvd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mlughdkd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vileyeth.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ndoliqya.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bcavjovi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kcboxcjz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wjogjngc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2czofbtlj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jsfcqhbl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ftqdycyy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cyqkqmyb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2shnrkjij.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkvmmeqg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gniiddwq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hlcrwakc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2exihhsfx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2myncnain.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vojvkqym.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mhsefpwu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ookcovkm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgysqtlv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2haoxybbh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jjpsdfhv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2btkjhiwj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tkvvnqys.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pxnihwxj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jfmszzfv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2trhexifm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2sxkxxksf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fhjlopvb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xqpiogax.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ulhkdomz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uonnknga.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vskbzhbt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqxkpjmz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fryisgtf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ajhookip.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hvzbpcyz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cxaifynf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2olkjbdmt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ocavnxsj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fkrfgqdy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mcynibvc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bzicukwl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2odemzttc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ckmqfbby.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2frdbfuus.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2recvpiyi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sauzqpjf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yuleabbz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2evflbtze.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2eseetalj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2euizncbw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vxtskpey.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kjpzfzec.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mijjiuvy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tqlncrnt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dkgdoxuh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pzsizvqm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zyuspaue.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2udhsjbrd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ywavigag.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jqzrrxuv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oyjeozct.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fxxavyqt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rvkbztfo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cdnmnxwe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kclwvalp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2etugaofy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kqbvkneq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nflgqbyb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2crsiwkei.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vklqcgxt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2egsfeonh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qwijgoik.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2orpegokc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qhumrpjt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxvgopag.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dzbaaipo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ywvibzkm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2duzsgule.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wygrwvpx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2godrkplo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2aieasvzt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bxsiaptp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ugcgicgo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kitgvvbh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2smnyhyvh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dpbcnuob.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dmujklgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2immnwvmq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hktpelik.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yxgdjonn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2woszxlel.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vauudclg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ypgkyath.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2knprxswq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2azypxmrd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uqinjfsw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bpjpjzuv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fqnjzjnl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2scrvmjrs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2taevjlsr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ymavpxjd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uwqxwhpu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2avsplkfa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcndmcyr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2stzsuzfe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nndpadqs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wgonuqwy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vtitnset.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fbqqwiwr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uwgnktkc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xdfcclsv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xhqlmydo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pmjmcsht.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jeinmihz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2lbhmsyog.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dtpchnok.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gllvtcow.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eeaagrdg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kflvcten.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2msjbkjka.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2smgzsacq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ofwragsl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xwnbdvdj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mvrlvoyc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2twfrtuyi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hbynxzfr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wmoiixpu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hfvmnphd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwbggklz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rmqunjqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlmjjksi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uviqfzlh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wagdouon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xayzkeuv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wyufnkkt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tswfcgev.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mhvszyds.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxcdazc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bguoahav.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hojzjsue.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gyoarmrc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgsyusur.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2adbvbsua.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qlzeheup.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kjpydczd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ftiyismy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tfulhejd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lbikopag.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hyrijayk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nxsdnkzi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bfxlrfbq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xzjifjwu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lfjrfgeg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2pbpnotqv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmpiwch.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qjyprswl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xlkbxkwb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uyuqjhts.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qrsokzou.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pzoxfcun.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zddttfox.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nufnhcey.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kqxtsxgb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fmiyqzlt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2iknucsrr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2irsvanci.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqzrngkp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2agoyktph.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hxdwtgmf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmiiolb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qhqqgxul.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bmleysrl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2piifohci.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ygsrqftb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ivnltnxh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2njjpqvtn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ndsdrlon.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pegqhwtw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rumuazqo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eknjdqgi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fiqggwki.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nnhixunt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jdmgbnqq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dtgewyyj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2djqizpau.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pvnvvlwe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oojpqxar.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ocrcldxn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qncebtmy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nmejfudc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlfjjxpm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jisdbihn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qmcqtrxw.html


<!-- 参考信息 -->