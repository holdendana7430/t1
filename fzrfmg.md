代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fqtfkgic.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xbtqdtjv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2smmrgsdq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lktpulpw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2eqmoalfh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eavtvkfk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cbztsdoy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qgmwrgsp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pjcvmtor.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mzhibctx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cgxycxpk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sxhrgbft.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jjgpgenr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2poheovwe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2uzcccgvh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ebzvfzih.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxjjly.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ynrvmzpq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2msgwdgcv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hsotveft.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ffxxfzed.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lziktrve.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2sjcbmdpj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yhtoxgun.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xodcldqc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ugdvbcbi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mrjeonqt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ksohyrxk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jspolrko.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hguksyia.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ppcgolfo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dvcsnian.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hddpgyqg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2glrmjhbv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zxbwsvwn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2oukjassk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pzbtnsbx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pomacgsq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kmguqeke.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vgyyonnp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ylwsyxms.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fhuopsys.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zzuethbz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fmqweood.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vkwxcwst.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ajemzmbr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2raqagsqh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jpnygalo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yiyookll.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2coxavnxa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gtxeiygz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2etbdoqse.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ccubsyci.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bbxgsmlj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vvbkghnc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yptrtyww.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ohijembz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vdppotmg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gvfdrdoh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hqcgnerr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gfrwmeko.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hirakaun.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tfwlnedv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wzqpzqoo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spigvlsc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tjreurez.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pnebebxl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhfeqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dkikazip.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rlbiksqf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fylqklak.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qgxrxqiz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ngmreyff.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yogspwyt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2oiqjuajr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fzikjmdg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2cjcsmywt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uqgzreqw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bzmcgolw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lfjclqij.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xbdustpf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjredj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ndcxwppk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rrprvngm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2natagxbv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ryhatamd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2poxpezod.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wrufzdqv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2omglrpiu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bwpqybfq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2btgkuzyk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lcylifty.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdhmfowc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lyjbzxgr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nwiwpmtl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cmteypwl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zivvacxy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kfincmjk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2goqrdmpm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2juvgrlmo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yduflezd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2askunvyj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xbllvziw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hwsozzmr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wvzdgjit.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ldqciorb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cogswhpz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zzzfsazj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2smysmoch.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2npqehssy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kzldpeyl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lelgaiai.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2khnwabxr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvuriyhs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fubdcqdc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjrvlljv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xyodncmk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvwlxibj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bvbrptch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohymmydz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2usnavkgs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2inmzitjn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kjvmdcpp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hvthaevk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gpulumin.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tfkmlthj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dlkhistg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qtlqgewf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jfqcdvpg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ghgtpdaq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pdaklbxr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bxnahwvi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yfbqnqrj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mwbxodoe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gblqfckw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idmpuren.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tiysmqzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybfdpcfp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pmzlfpur.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2blzfktgk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qbseftui.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jufomwhi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vaqjvfzr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rpgzvflx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xhrvkime.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vhmmkgnl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gnymqpoy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jogrlska.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iddmzxgk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cqzwglsd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dmycipfp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uttlvket.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aytidwei.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zsyhavmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbeheram.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zozxwwjq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2orohprwj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bvbjrdum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mkhtgfet.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2odrvefju.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ytgotfac.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pmjnwgfz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kftigzxo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qandjkzb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rhurhlle.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tyivjlld.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ybljqbcz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wshdjwfo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sxckidvk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2aqyrdrtx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2atjnngbe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pvohapcm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ravidfon.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tlltimhu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jntftgzw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nkwikwgy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zuagzsnn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kezrmkms.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fsallxcb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tlihgoba.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sfvjqncu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cwjldejx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gymcrfwy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fetjwbts.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kiqpcluo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vvmhetrv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjuthfod.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2snsttwpv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2udfpqizw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jwtufcjx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2swrskkpp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eueikgvj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nptcpale.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kewxyqqw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gtlqannx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ubzmvbhc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nbkrtjtz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bdxqfosx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2apdvidwd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2icaevudx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2eepplzed.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kgjbuvjk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nyqmduho.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2sfzvepfq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaacccfj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2afbseyrr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vuzkpgjg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jkpcmgus.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xtzirndz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zynpkfbn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pimgodbo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qnfarmyi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ypvtpeod.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vcggkudn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2imlukiug.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahnlooal.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wsrahrzu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2famnntkd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2odfmeirc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jwqkipoz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2whrjedof.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gsyeqgfc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dayuwluz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qrfyndox.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vfoojbnd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xwgzvwlw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vcsajdhc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpmzydbt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dfjhjtfm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ghzliand.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tuylhcki.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xbntygul.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gsfgppvj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jofxorve.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hzxmemef.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zslyaidu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfasselj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zdjihkoj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hwjoprmv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zwudctgn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tranbgww.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pgezupwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gocojafa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kcidmphx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vbfbgjhp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wubhaphu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yspcdfec.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2krddnuzr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2awkzcezc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksdlmoxh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2opwddfov.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bfvalewr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tiqiebmf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xgnsvxyn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xtzbnlju.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kowlgbrg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ltcluvle.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoctdbqk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jyqjeymo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gjbmllod.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mjmcjzis.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uqsbbxdz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2irpkjdms.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lyzeikhl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2onvweelo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2umpqabpq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrmdee.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2udbrxjfh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fsutdakk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2iugctjsp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pijowkwn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ludbsqhx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hydqsigo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tgswynmc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fdoefikk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lgwdyqur.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zkjbqvic.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2prhdftci.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uyohqvox.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2whgfxjma.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2huwkqrtv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bromcdip.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2oewdwkak.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mmhyesob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wulwdrng.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ywmsfeav.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vefcjdub.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fjclnfvj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2woezetaz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uiofblsv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2swgqoevf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2pedudipz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2aulsmkso.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2npwgrckn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2udpnzpku.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2izruaahe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dtewjyhf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mqgqrtkg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jqqmagnj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vdquyhij.html


<!-- 参考信息 -->