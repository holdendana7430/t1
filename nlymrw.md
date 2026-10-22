代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2eirfvwad.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ggtvhuby.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2repsncck.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2etyaivpg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdhyuzgv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2umoakwmm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tzvfkvfx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xabfghkt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oawjlbze.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cgdzagkj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aptrcmla.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zuvwaefv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jnflezgq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sukgikpe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dlwcmgzb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ujdkcbxp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wbppclvr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tnnbvgip.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uhvjkkkt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bnxrzwdc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fpwicnev.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwnnagyq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vbambckg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wcwzsrox.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dhtwefdz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxgtnkvv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tsrjvllp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oltiljii.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cgbvhmyd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hjpyakee.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vdvrucyq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2onhqhwwv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xynlamga.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2tqizpink.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hwiuigag.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sntzhnxz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ggazpjxa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qxphopzj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2akbthrof.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rfmsncrs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dzwxhrww.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hycvrrqy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qukkkjmf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jvywsoif.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2junbmmdp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2doefrvdy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cafsausp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ckjdhbgx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ubelmhas.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2anfuxtrq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lxdbhvoz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zhoivfdy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ttujscma.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2riponypn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ecnoqwfi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2toaylyoy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fpmfuiiq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2pnijdqkp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qgrephqo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xbkoauqw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ojkimmtc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rmmhrpfw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aztnaeud.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pqznedsa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2buluuqkr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bgcyabki.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ejbmkbya.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mzifsfbz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2khifvfjl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rddvpqfp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2krobiwbx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yffrhirc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzdkjoov.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2uimzjhfx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dqkehgrp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ocmltmuw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2agecustx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gpjghwug.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qolcqzda.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2guhoiakn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dliatzmk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2papfcqwg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kvpvoqhf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2udotoztl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lfhgattz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kxkilvnf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hysiuwae.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xabsxvxu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xveqminu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wblbprgi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqalrkgd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uzescigv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xclidfka.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nsghkozn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xrshexii.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2prtwjzlh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mbmymzhz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2setstlzt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nwcakvhf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hsltnkjh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2quhvfimh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kjlbvyzs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sujtpele.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2aozdvxxn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfgwbrra.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fmcezibm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pzdrhowk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ixdcntgk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2siudgusi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dlacsbac.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cvxkvvpt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2totcwmtz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xozpbfbt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2axwxsjuy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ioyiptxo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ogjuemwc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hipyvnkm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dpsjobvf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hnbtiqwp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hbtxzdkn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jylbdxcr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trzubaev.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kvhbxrfw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmwydvog.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qxuurlai.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2alkpqepx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pmazlthr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zopipbdh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nkweafvg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xodayhyd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2eiiksbro.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lrignlwp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2goyeeqvi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2slbammqm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2amiukqfd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fjsjxrkm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2regqshyq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2goioztih.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdcqtmig.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2opoabini.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pzzsfazu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2znomtypp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2elzowglk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycnnlaib.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jwrzfnvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsqhbomx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lkutxaqn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kabcurwv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2prabbqkn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2geufghox.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2avpzgfnt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nhrmfhjx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ilkudsnl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nirpwgdy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qrfgcsas.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uidilfkb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2bawciakt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zxuweirk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbxzcclp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kslmjgoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cilbwcos.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lbnziypl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rrggvhfa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bleirkjf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kstncwed.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2srzlrfql.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2igifvogr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xurmixnh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pbsghsig.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2meqtajnu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xovylaox.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rspjqbrw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uuncyunh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lvbyfthn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dygduoaz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kotdwsfa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zofjqdci.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2byaudjps.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2acwqvekg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cvqbznol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ohfstqnm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mphcypdl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2anxcntpe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hbjecvbx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2aehkcigq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gyzxsgte.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ecgnjmhd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oopjnghs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2omyhjdis.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kbsonxxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zequyypu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2esthatra.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cxlxdivb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uussiwpe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2amexecvd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvsnfmuy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fblycsnr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ogbskany.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2desbnciu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vzleerfp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eodzdvqs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hxedeiof.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ptlwgipw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nrsqsinw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ultqzkwu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gmjcipbp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kbxlvyvx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2geljgknf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jigrsjum.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kootqywu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2epxgvaiq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2njecagye.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dufawsnu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pfipykce.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xvlswlsk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vhxjcrei.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jwzvgxxo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ujbmsjec.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kxzpnwuo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hrdnpihc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2udoiylzs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jjlrojdl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qhasnhxx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2twycypjt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgkebctc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vrmzjgwx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2svxnevje.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2boigrwhw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kcjvqawe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iovnmrpz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ollaxxlx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zavolowp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uppbbaww.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ievciuhy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bqaacshr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xamzobiy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2exfjxvri.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gqoonxud.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2klsikput.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2aadtrsmg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2loiprmoe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hdfllojg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hwrsnfpc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xzzngqgm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gisfeimd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2slrtdkng.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hymjiasm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2icrlgegw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xingtazx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2itowququ.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfxzegim.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gslbchxc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2smzrpgnc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2krchbcpc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2upwofbro.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xqkjspvo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zkytbdfn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlshashm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hwabcrza.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ogilimgk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ijewdihd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aqktcwni.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hpimwkyl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mqgzxjcp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yvgbtcjg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tkmmwgeb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cqbrrryt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zgeazpwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zzanmcrh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iugoadng.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dtdsuvtj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2esvhjqfi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hrllihde.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fgsiyaqa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sgydwznj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dokatqng.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2twlwjndv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xpezugqs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwchxcg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nkflwhds.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2idpasuhk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qgusocjh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fhaiovna.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dbfcbkzw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lkchmhjt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ilkvvwwr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntjwbqjl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zkzvjqkt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2joyueyfn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vvqieese.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tuaxkzyf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ycyuridg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2minlrloa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2iwcvxwca.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sooindew.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kyxsytji.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vcgfhvpu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2byrcvsga.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ddsyutbw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2snbombhz.html


<!-- 参考信息 -->