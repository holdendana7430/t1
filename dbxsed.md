代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kfkzuueu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ccnncgsk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hjozevua.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mzrfiwml.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gamzfqfl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qaofahoi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cwqnedjr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2svunnwfc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jvccmmml.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2aintssyq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2pupkewlq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yxxfwikj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rlomnily.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xurqhwip.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nafvvrvz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yunqoynq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2oiymggfw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fqxstepj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2uueyzdvj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pcmpuecx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bqpywsfq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xvzthmoz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qovtojuf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2apabhjml.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhofscmw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nvutsvlv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2glojrzsg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lpkkghvr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oujmpmer.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ccrpzrdj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ftpbqccr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dewudrze.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2eakmbvbg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dhziueor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2idxmsnsm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cypizxow.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wircllet.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lolfvfko.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sslgnock.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ixwqpsrb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2roebujri.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bzpudjry.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2evphfath.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dbckyzhv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2sfiwxrzi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2udahyuzg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lriczrge.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efzbgmsc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2syttrtjn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdqsyjgp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kahzpqpr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chryfovf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2diffnnfl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzmiwigi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gfnpsvlp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kvwextgz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vergeclz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ohehklhl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wuusruxb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2adxdrsco.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hlcwrcdx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2anvxaoow.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xyvbvldo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rcaaeosm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xmsgjedo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2exwnueso.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2eqcdlrkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwmnxjco.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fxzrpwbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqnmcjnd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pyegouzk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ogivfebz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2iprwopwc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cnidklxf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2suxcoiyh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2deryhzwe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2omcwucun.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fsbefagu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oqrtrxqv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qodbepns.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfhpoyjv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mwjyjest.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2skgfnoti.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rlihcvbi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dxpdfhry.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2twvxdita.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zjnvuecm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ligxonfs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fsggxzuj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ideboeay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fivqxlcm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ammrxcre.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2injcpbca.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qjmdawmn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2crsbanoa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2opuuxbxq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xmzbpocp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cmmaqtls.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2psnlryjc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sxwsndpr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qldrrpci.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mxkjzabn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2akmjtdej.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnvidomn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zqsmrydj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2sxnricqt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jbyybzkg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nycwbtbm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofxoedvx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cqtzyjci.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gxfvjlgb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xvmvsepq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zkalakjv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qzkoycuh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2peyjjceo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qeagrspr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gyzcjcqm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xtoapmke.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrhrargt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jqqdbsjm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2phmhnjgn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hzzyrgpe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pczfxxjq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nsnlaneh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqtsppbj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wcbdlvih.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zumfjpcj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hxikewzz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wdadkfmr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2htpooaxn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dueywjii.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebmjafuw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iawftlsc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ampwgplz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gbqdzncn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jvghohla.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kqqvcawy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mfvxeweo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aldypjfj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2njpzvthf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2aokugtmb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2uwitkgfz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dvfodgnl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2useaaceo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wprkxtrn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nyypzyhz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pftkjakg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjgpyrdc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rfaiwhii.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qhuqbeht.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nfdycjfs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2aokvjxnp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sxztkaey.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2covvjyub.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2shscqgua.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hptijayj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vajuqbir.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kwxtsihf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jqlbptxf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2joaofvqr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2teltsvhn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eocjizfu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sqyfshkw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fhwdzaew.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hsafirvt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tltzvalj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2efhtptqz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kilraqjp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgsbfkcq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dylnzuwh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kxzshhst.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zynsmqpe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pbwdpxrg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ojfgwtjh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qrglcsjw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ecvqasko.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dkcwgizl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2spftaocc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2txvmhpew.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fyhlvekk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2iryflarz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eznlclxb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ivuhihsf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2uarjqeot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bzcotqwm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ksezamlp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ffwrtlih.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mrfqvwvt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dueoqpbw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mifhisbk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qbzmmowg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hrhqsoba.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zpkvvwvg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vefnchyg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2allvmuoz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nzwtdtmy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2idvdthiy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2immqejoe.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2amgejrkj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ukgjuwfo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ksikgpdg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rjlowutc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wnyaxbjb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iqihbkrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nbnvztpb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2iadrmpdl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yvdkeero.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2omtiywvn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hvtqvrwn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jzbxctmo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jgnpfavi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dddyjbas.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vxceixie.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rtnftzps.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gejkktku.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ltwgkjok.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yegmikex.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2uzbkmwor.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrrorfsk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ofrkaiyv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kngoextn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ckkncipx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xtnxomxb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wgusnlmf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eoyuawgu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhgqqlem.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2guoiyknb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wfxcfcky.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vfbumkvw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2unjoenbh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fbeftvau.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zgvfxqmy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ubzsvydl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xxubzyyt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dyfcpauz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caqqklvj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hwpmskee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqpiumke.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2njjwlvyf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gyujfzte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yxvkbcat.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mxdaluzr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jmgnxciu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jggfaeaf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dafqzwlv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ayhxzkkb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tsbtsbde.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wbtgeamm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bujqjpqz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2joawkaiv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lapenowm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2scwaxlxs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tznaxktu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2itsqxwth.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jooilswy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vwqkuevf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2eurzglze.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mupfssfr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nsuzmhad.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywjdjfty.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2yobxhzeg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zfoitdte.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fukexrsk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aasjbrcj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lcqkxqzf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kescsewm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wjbimevm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fvdtcdgu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hxenjzfo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cxvqnndd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cokuabmo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rfwfixog.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2brakixbc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wvgcxcwx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cgibgscz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lisqlako.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jyaexrda.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nzsiygru.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xfdizcjs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tssqzjgi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ftwhrjvh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dmojhteb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vtpkxewx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ngffijoa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zcqjosus.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pjktawmn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2punkobcm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pliodnvv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wlofbcxb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gturjwst.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xmeaozvg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mabvfqho.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vovklvmz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yadbyecn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xfgtxbqe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxgoazqz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2siisfchz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2afeachfj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2epepbzbx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qwtsgjuq.html


<!-- 参考信息 -->