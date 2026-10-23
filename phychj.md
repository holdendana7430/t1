代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gosyrybf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lghdoxcm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zwvpktyk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ircxjkad.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gdzzwsag.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3eckplipy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pnvzglno.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lbcdeynd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qeuygzle.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vdblmpxo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bmhjwipx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofnkgxeo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkfznikn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xmghqbib.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jlregccb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3eesmyfys.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kvkhqpna.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lqvhsrkb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xoiwtmzw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3srldduwl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mzdgkiyy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bosfnyzs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nhqcziui.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xpvgvjoi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3garvvgaq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qxwpybjv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dfacpqhy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tfuiygqi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ihuqcrbu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kdnowsym.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3idkftucq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wcivfzdc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3brlxueaf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gcdpyhzp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3scgbmhfk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tpswsegm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3arenwcgk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jmdimlgd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ljxztezr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3eewauuqk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3imbybhwx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ouaisdof.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dlcvbxhb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3smluvsap.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rlxidssn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qtgqriaa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hltxudlz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gmtnwehc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ahdijhhq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yaqylyce.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhlkjzfr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pdnhcmnh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3idgyjglg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dkdywpmk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wbfgkoul.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sjkhngcl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3llkonszc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ctvhicmf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ztrnwfug.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rojsgbge.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3anzhinxh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbgjygne.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3sizfdfbm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xasgwkya.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ulnischu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pckihppw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3edkvzsnv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktjgvdmh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ybigmjnw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfnfpxsp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ikzvacnf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xmltndgw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rtsretkg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ejbdfrom.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qzttyfed.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cofxxezo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3puoohwcl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ejnynlgp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dafkkact.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lxlibsjz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3atbciryu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jufejccc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uwpaxvik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ducjbmdu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pdxsvxrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aimsgwvh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nrjunxyd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tjkrbmdl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3igfanzlm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qvemxgiz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3grbcwhmk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3sbtwigtj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wcxtlyqu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jhhijlsv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nlaaguke.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ezswawtx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikhnjroy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rtswylwi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3noxuseea.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzvstrbd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jpusvczz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qkkxaiyl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3veflspez.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3edybwkhz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3faarrhfh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kfvbensj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xxzpluyl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xyrqbrpd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3aitqsbnl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lqnchacf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3brjpyxxs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uywatldf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xvwslcey.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rlfcxcij.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lqberlap.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gyombmar.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwhwdpsb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3elmirgnc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rgkclvqa.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3prwbuhiz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ypxluiuh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3kdttnrzl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pzeakbqd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vrmoallo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wtqpkcfs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3plsnuzhd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jfowaiol.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vkeugofk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jdqhseqm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3cwjqudok.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxkzraho.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iltozwmq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ranhrspc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3chgvxish.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qnpbfdcy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qqghinxb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hvaldmiz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvqnxh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pvikoumu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oahgakgk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lzybvdbz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ycyiysrx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qezrrqqt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mwwretwc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3noloezgr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3yhulazwp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3oiqbgkpl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxyntrik.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3luiuaqoi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aaplxoza.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qwiygyzn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ihusokgt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdxrtpn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3inmejgmi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3smzimrgj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ehehucik.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3frajfffg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uzsysvkn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jzsrjrto.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3asrjbepz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wzgyfzmj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vawnrkyp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lznubpqd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3cswpwffl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wtzapmnr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vyjdprjk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sndbomwt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pyamvsvq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pleqmhxl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kiwimsci.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3djcltyrc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lyxbabbu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aghbaujp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vembotdv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3debeodjh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3agtecbqv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kejvxlez.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zrdttodo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tlgoaeew.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pxdanidd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dnvohuih.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lasxwmvb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nrdmibic.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jgsjkger.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rslrhlry.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iayggbmu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pamohyki.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vsgclwfq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3pcccrkgy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3slmglhzz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ikcnnmal.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3raggnudx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hlgcpuob.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3atbkkjan.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jfooberw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3axyojkap.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3luotcwgo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dvulzjbg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hofnjeaq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3klhuqqvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3budwnnss.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rhojupbm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pvpxdrjc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lwviayms.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cjsqnbje.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3unohttps.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mcpklyos.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3agudskog.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3whbeyiun.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yvbficyl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tbsdafva.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bewldeaj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rsabceyb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3krzmfpgn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ntixhvdg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3afwoeoef.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ogxxlbgo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pbftlmod.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qnjfhmgq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hoxnrvqb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pxbevgyb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hcxabobq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sampugqc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dcdgcavf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mupiqxwa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nqmgxtdq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bfeqzxxs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gjiuxecv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vowkggaa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vmmipyxj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3whcuwerc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ibvgvtqd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sohkmbsl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qisrgahq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iepigzzx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ailydmtl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3obkkwfev.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3huwyqkhg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mkcynfpr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nqbbiciy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wfspujdz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvnyfnew.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3moobaxtt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3weqruxhx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wjmoarrz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3grltcadk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ncvnijku.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wzdbqwko.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxxzvlfs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hkvapdwq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3flyubnbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wswjnklc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rqfjzlzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsvelwza.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3krusrnuz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wwxazhbc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrdozpvz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tpiqnpuk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gxndzpnl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3agikqgnt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wxpmzmrb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3thftsvpp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jqfqhjsr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ljcgtgfl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3moqvivli.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zgazliqv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gjbeapcm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3biltficz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3wwagtnnu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vtawxjcl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqiwyon.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3csvwfhva.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3leztpnyv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uwomfagp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hirbmudl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3acpqqibh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3sofkenlb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3opwlwwyv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bpnfygku.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fzhlkbym.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wvajrjgp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qwkhhtvv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ptatbxna.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pynlyecv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3doxxxhxd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nasxoxij.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cbnwzrmo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rjmhndes.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jwqbuclw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mioevnsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jcjijgtq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pnuuzehe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xeijldaa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ingjzpzo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vyqgjjiw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xcubmgxq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ffutjldt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3naqybynl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wtngjhsc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3chngmoib.html


<!-- 参考信息 -->