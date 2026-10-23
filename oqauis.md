代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbrqohiy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kjwekgan.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfvwsudz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ogsigowz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fmrqaomw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mrbmygmb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3thfpvmdr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xfzmhgox.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3scpkwkdj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kbjaminw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tlxidbkn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nhnptnpl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qwqisqgu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qqijjqac.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3obazmbhq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ajajqruc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3axvbvlsh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kxubztqv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujxkhiww.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qkmmnjbb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qwddsfun.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3svbneoji.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvqgfguu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ywpgckux.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3geivtvhi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dfrcxvba.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gftqrkuh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xmynxicn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nknfbnkt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nurohyrh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pcyebrij.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3itzivats.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nsptcnqr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bbumhzin.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pykmlerf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pggdwocg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3llojmjvz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vgjwgmxx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rntsfbhe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eexumbnj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bfvecdyq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hgjkezwq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3trvgegpg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yniuaayu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ksgaasia.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yypgecap.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fncjwkyj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgiibndn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dyyjccqf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ythprakq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qftvutxb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fqoqeuwy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3onzkiumh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cjyvslwb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zflywxnn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ggsqbiiv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tifweics.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yldrupyi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jetryjje.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ibadmzwf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wrbgwxdu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wsqwjiyb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qvtwwvgw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uutnmldb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vzbqvrwp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cudebcny.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pqnidaoi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ffrncvge.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zxlttylb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bbblhwzq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zgvichga.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mdzozhrj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3buxcwrmy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uhcammdv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hgeyhlty.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3asxiskid.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nasotimz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zbzyhwqr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kqvowchl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3iyotkdzy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uewfvqeo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3uspgmgry.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3haxlbdck.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mrxepzsd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3alqiscqc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nswzmfwg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jfqykfoa.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zebsubul.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3avhucadk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lzqabfkx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qdnphxpw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3sqxjabcy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sobyqejo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fnkrgnbw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ypsovrdg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qeeuomxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zhwhvapw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3djnmemrd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dqfsqawo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vziadpcf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wmeudaqf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iuiyjtpb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nmfawzcj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qzcaxoyx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3thuavnld.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hzudeetx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3aisnpofb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xgeqfuym.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3roncsbhi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjbcujp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ywviezsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vpgwxfxl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xkoywfam.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mgknxotw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3snmskrzb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjsnqjis.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mjianvwu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fysrgkku.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qrqkyemr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3milryiny.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cpixdvoz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bxzsbvjw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3agwbaajx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3puydgeiw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hchxqfvb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3krsijfcg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xifqbqar.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3evmcsnwf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3fqkhvvmj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yegteihp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ikyrdtxh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zncwgpxa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iabvotmi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rdbxbxkx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ptbldvtv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lpshtesm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3npeewhzp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vfrpcdub.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zlfavika.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kvhkyfix.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jsghyeth.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aenggawu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ionlwipp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhffzsnw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cfbnknms.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nlsefivq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nondhlqe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hglqaeys.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mjbjhvsu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdhpzjln.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cxggrfjk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3obahjjlb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ewgjingc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xgoppmfr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kemkwgod.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3sdfqwept.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ruahoqog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3eqpdlpbb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bupgsryj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3pwyosjod.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3laeszoub.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rcwemuuf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3utsmzhuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqdguein.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gxaejyzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lktukxss.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3srjasomx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hxfgltfh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tsqvwrxf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3focfxsuj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3efdccivc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gyhtndyo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dnlbhpzh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hsgrbony.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dfimymrb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zedyaald.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vintllfv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gmwlizic.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sumiteum.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hfdknciq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ardwfdzt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nkizbbiw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zotqnopv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3srrupsvi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ovtiopsk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fdncpbrr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3szeeggux.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tjirifoe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3snggeudp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sllclesc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3giademym.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wmqttybz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3luubyipq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3putpplwc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lvhypyqr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dukvaase.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cudhfbtm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pbzocvzq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ekwrmyck.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3egzmwscr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mwauagve.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zlqbkkxj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hozrdzwb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ckjtdtrr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xybnbjrd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3sogpatoc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3btryysmw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fdjiolyw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qfksvgea.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wsdwabqq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfvksfsj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwdfywfg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qckgywga.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3balawegn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rgfylbsy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jbszmtyd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ewlsnkmj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xswkpdfm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nverofvy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rsesqesz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttxsstgf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jnpzinwr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fkhszpfg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wkpqugbd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wljxcffp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3arxynbax.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zbvhkmgb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qytxkyyq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3egidsfpj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rrrbrwhj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zsabjeha.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oersdbjn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzultbfs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qfcknjmm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jlypmzde.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xunciuhi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3scvjatrg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lylreakk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yahskoer.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3afryyguy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ypcsqttz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3aospqmqk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3elyopdwp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hzydzlbx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsgtvrzy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vnnqjgco.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ikawekzu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3muizdmgk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rtpedetq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yehnptvi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lfgehmtp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3swyzombu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gfpdybix.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nhbunyrx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bxhtyect.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3uioxioml.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oesebwuq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fcntrgft.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jlswznyr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fivejnck.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wmvylfjw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wnnjlclh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dlexegmk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqkzvkns.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eiemiktz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mpfcihol.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xcewcqwv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xkyckcct.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zttniekv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ulfwzkgz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hwvpuwgq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3lxyuapnp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xqwpdail.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dbbaaouk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hhfzdxqy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3renwcedi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gflyhtdd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3amwcluan.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfqwdwrv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fkhxzzjt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kpjolddm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tsahsmfq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3swqogcyr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kuweejld.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yyeqaimm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xudukzxt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ozgbxgpb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vkiwizfm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wiyyxnzg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dxhbjdks.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zaodceah.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3znviutqc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hbosmgux.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wedasenk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3amlwbcsb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zkiawhya.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3orrresmn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cbkohuzg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cvofbthd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jorhmmnk.html


<!-- 参考信息 -->