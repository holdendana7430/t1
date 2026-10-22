代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2phikhztc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wryzpofy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vxbwxinj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2kptcehml.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohfqrbtl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2skufmwxr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lavhfvbu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2bbnvsdaj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2myjanaln.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zdefybsw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bpvfouwo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cvwarmom.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dvzebbom.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2daupertr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2holmbnbf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vrtqqteg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yykmxqsn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tlmzzydw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zntptgvv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kqyearfo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tkfwyljn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wmujzhgr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ogczoeud.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mdbqrjtd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2brdsbhsr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wkrrhfyo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xquoukln.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ktpvlkhy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kcbetqcx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tbktwzgu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zcnhjbex.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2byburhqj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2asocrjqf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kupyeqno.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qwbtuhgd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wdnykywz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gfiyxttr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2byjsyrpc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kqpefdtu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2irmfhykh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rodolbus.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uyfxrkfg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yceqvpys.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xxddifue.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxqvwjhn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ynsvxndg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2aavyeohw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wgkvdxau.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypupfekl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jyseogiz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pgjsxysm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oyexnnpp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2szgcqojo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uredqmzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ofmsquom.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2nrlpffcb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bxvzdkse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tbemilwb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ikpmttmb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hvlsnzgv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ntugsrhf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2glcrunvm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yrcshqmb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vuxpmhfl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2okaqngbd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipxfggml.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cdxzzwub.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnekdlin.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hsqjwdvv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lzcowqum.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bjkbpplr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lsemzijb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bzpipxfc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxmvvgoy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2exlsewak.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ojixnzaf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2thduwfos.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2uzckfstn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wtlhlluq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xxikosct.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dzzclvar.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fjaatzrh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phkzyted.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fojuself.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2iszbpbdr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wvqslrop.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fjaemvrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydimkyyl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ieoxntwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehwbadzo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2eroqepns.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qftmyxxr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vwxchjpr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nxwjpfkv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lenrsbxt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbzdciiy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2twzcxpoa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2drhdptbf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dumtblvf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ptrqhckg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hqvheqsu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hhbfhaud.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iasiccuj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ohfwfamj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pmlpgukm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hxgaknvo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sosweuuz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eidieyta.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2emnafifu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kpdpvxbp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kokuakhx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nqjwzker.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jlurywqn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yekoujwk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2snnedzac.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hkcfztbs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2aiwupyvb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2davwjuca.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ekweojyn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eauwmiuc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mbfuqjjm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2heparnjh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wbfzlggx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcbcjkjc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yumedjgn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2asawdopy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mcgasysq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2prdvsygu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2silmenhs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lhahwwwt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fuiigzad.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mijnuthw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdskwzma.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2adqfrrtb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wwncosdv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oakmxpdb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pvjtvkjr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qdwdrptv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqdymqaw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wcuesxby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2whyfotqo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xjtcypgx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bytvblsv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gwxtdhpd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fiqaktqi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jdmbqrnm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sncgtuzs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ksmlgcon.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hhcepwsb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mtygvazu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xehkhdum.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2njfwgqff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jkszwhah.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yjokjyjc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mgjjldoe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtywwsck.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2luhzzirh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tqupxflw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2psxvrwsg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sdqxjzpb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lupfdqmc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vqclcliy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hjqliulk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pczjrjip.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qakbdtey.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rbpcmpdl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2avtpovxb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvwceytn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2txcfjxdc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2iaekwzsb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2aceevpcl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yzqekycs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2alsvvbgx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mhyjyeje.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2psfenfse.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2japxddkb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iybwugks.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rfyezcqd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tolaeacn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lysaqfjr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ngzmwxsx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lmqwvvwo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bhszntqd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kbdlurct.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aojoppjt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hllzrehs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2abzdtaqo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dqdgnfok.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nifgknkl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yaqhfowq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bmcaiyzl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kpeimarw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kqakjygq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tdonrixh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fanqrywt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ffhemgbn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2foglputt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kilnxvor.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkswhsfr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2molqayfh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ppwzipxh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvwrxpzx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2eybogvur.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2iufzfbzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wfszksxh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zmjmzams.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cnqbmjhv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nlfedpix.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2yvfobzhf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkqkcxqy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fkfyxadi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bnujvxvj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lrleupav.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hczvgmyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2blfjxjkx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2czvctjdd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cpmeuoio.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqwjhjjd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lohahxig.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ckewkozr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2eorqjoyd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oxztipyn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ltxghdbe.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lblckakq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dcwpuzuh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rijlmnfs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fsdcxuwr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmppus.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ejnpdwle.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fgjnwrcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cwjedpdg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2harsobit.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fossdbik.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tqqvxumg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cewspszm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jbtcptrk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gmwjlfpa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2opnyscub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2obgilgob.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zgfwsmwl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vhqhwvyz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hmwnpscg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xfwzhxsx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xcmphrwg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hjiiywqe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qbpdarvc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2aztiqlmv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mvvdirpl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ehlebthx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bparblwu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2adoqecqz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vlacnrqq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2srakeuvu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vcuipuji.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ddotnvgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxdyujxr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ftjjgkzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzymqoyx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ljkttktd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2anbwtctz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2urhxsyyw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2opsretac.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ihanublz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rktgyynf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2aaaipiyb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bxmiywvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pcgetbsn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vnmmjhyg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zoehtjot.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oprayspt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2voydujwa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mtgvbqtz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2soxymxsg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ursgqwuy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2peutmgof.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zizplpyv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2anltezjc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fqnejhux.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jryjdvdn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hrljptft.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bssslvrs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2faffrovo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2stalorbl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzsbzjch.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2djksopmv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2fcufjrel.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2levnwuny.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uxglxzxy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2snopkmxn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gnvqqygj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uvtvcsxi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pkxgrzcp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vnvbojam.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oystyytr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2oxooxylg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bnwgiatg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sowvswbb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2beytfbln.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rfwvnljy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zqggbjyx.html


<!-- 参考信息 -->