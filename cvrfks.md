代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xvlqjohf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3syedgxax.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mezaumsc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3virmwfdb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zmfvkfqs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uaaoauzs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tpapxitb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3omuzjigu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hcctawvh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bthxkmhq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ecvphchj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cukqyqqi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nrjdcdhy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cxupzfnw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kmhxvbuw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hwfdpdzf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vernquoz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dburmouk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vxspmjuq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vcmoyvpe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3datyunje.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3eystcnad.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dhbnsfks.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zpevobug.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ioivrdxu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zsmqqzrd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wqvdcqdx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gcfehelm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3spzqpcqt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hhxwseie.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sbmhhguo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3sctgafen.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzvcveyv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3arxfcukx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzsrowoa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dhugaajf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vdxrutbx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3joxxjbzh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ydvnxbab.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aefgqmll.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qmvaezft.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vmprwguh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3geveuhwg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hegzacus.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3sesneoxz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3scrtxgll.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3eawwaknm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vwnmkyud.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fqlaaedb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fzlhrnzw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xwdwzvyh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ixuvbaui.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qgnvdzll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kklqkdsn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3amsrtbzq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iuwtpjud.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kchfkzhu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sgvmtffl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hrmqjcrf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pzjprfnv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bqhfdcxr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ikdjjrkp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hdytwjfl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3spdyyyzi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdqwlrew.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3rrringtv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3evcfcypv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ipimznvm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3whaosels.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3acswjdrz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xfvyaain.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3uersszww.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ulxqfzac.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3okmnxjtq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dcrzncey.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zoefxxuf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nkianqiv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hkdrddxb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kmeywlia.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ktdpstxl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kjgwgrja.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3giuqizge.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lumjpmzi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojqpkjhr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mvickovt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtrdhowb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aqunpqrm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tunfrisl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ypgjhiqh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxrhrykp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3uodmjebc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ourxtico.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tedssfrg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lflpuyeb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3opsynkyx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mmijtlcr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mduyeduo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3vexzsnph.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3thdglpie.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qldfhqzt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3opyetrsh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3takcdguw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xwipvnnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leyfrdir.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kslzcwlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eugcnflh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jpsdtceq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3meguymlq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yescxsay.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3poganjvn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ivmmodab.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3oxgpuogv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ikrlqeun.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jjdjagcn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vfkktvct.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jdvpoczd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgvsyafk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ezmssghm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dtvjmkfz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjqnisbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zwxmufwc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkjxytoq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zpcowsrt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gkqxeowo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rvlzwoan.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jghwbwwe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tiarmtzu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yungrgdx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3eyvyusrz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jwmqjhks.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oduijgjm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3exwcylno.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yisawtbo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvcdezad.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wapcdqta.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gzltqfpd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhhhzpan.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lcnpjukg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ccvuvoev.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eaoqxikb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gqlczalj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3avwcremv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nsoaetxe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3diukzrlo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqijfozl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3sirwdmsx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tobhanyj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qziuxyin.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vsxzvfhs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eoffgiru.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lzgcawet.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qjkbhzfm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xmbemkak.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pfoppddt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3sesfwriz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gmpprpxp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gwileyij.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zfjodmya.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3csfcoiid.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3glrwpjdy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hkdvjpvs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rvrkisev.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mkoqqcjm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fzrplalw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yoswwopi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pgvscrbt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rsrjbfhx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3utmvfgzh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3okxtraqh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gqpijspj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wctwrtys.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nntboyuz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjdsilcl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wrahoiop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qmjhxozf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qjseveez.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xbrgffwy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3bsbrcxhk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3trjvdrah.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pyeiaktd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jlhnwove.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3iuuspkup.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tqtnpszf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qtqiysxm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ajeskkth.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xfiybufj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nxuamtuw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3woeqgtvn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3flddwpkh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qxiutmrf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xexkeylk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vzvlcikd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fpctbxsu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ncxprcqs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qedxirav.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tiknwfry.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lndoesfo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xldhopnt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zvqszfdp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hgyhrokt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ixxzhrez.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tjtsdgmh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vgqtrmev.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wdmlokun.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bcwtzxcq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nkugzlde.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kwxcpzwu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gvpeycto.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xmttborg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uiqmmrwx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajrqmdxo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ovpbdflb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dfuvhuli.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lqzxgtfa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yxayxnxz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3frblbhsz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kgotillv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gzittvag.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dirfacii.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qijocfcd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3oevgulrh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3prmmrzvo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3peaemjlx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3npppbknj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kmonvqvb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jugiqztd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qcqxtgex.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bwszvssa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hugmfjhf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3roxfbile.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3brwwherk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wgmerpht.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ypxcjgpx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cecvmrmi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yblqatnh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rwudenaz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mzscozst.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nxqkrzfd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bxddaqae.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qhfexmsu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tmhcmhbu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xlstnprl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3juxihkqe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mtedaalk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hfqlolkr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vwqdlhuc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vjixoali.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qzsmddsi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jluanspo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3odyqfbvs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kirslicm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ndhpbshk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pwzmgphu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jglnoizl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xvykldhn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gohuflqg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vkgsufmo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3msnddrvh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nnxvagqp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3emmhijad.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cgehmiyt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufkytmnt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wculfcbx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xpunxtrd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kdxhsier.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bokgmjsc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dvzlwawm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mzdefzok.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sycpqpoh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qukqpxeb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3izipxjel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfaryjpi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rmwzlgrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erqnfkvh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wzihdutm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dmvfszod.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3stxntbzx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rifiaonb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3obodulml.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gpnqimye.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kqlumwwk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bnfkhhjy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wnkasdnz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ocqlvnvl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uqdsisga.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3honxhbao.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gclifbos.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3crtxqamc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jqkqlaqo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tjyfyqqh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mvwwfjqh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3axctbmap.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jtmobcuw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ubapkamo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cqipsayy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzdebayc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zwxyhnyo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zcocfnyg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hsrggrgg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zxaxxeri.html


<!-- 参考信息 -->