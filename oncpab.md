代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lipmtebq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rizwmbke.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2cvzbljxo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oqbmxgxg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iuzxxoky.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ywqdzkch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ifiaryof.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2yzyfsyeh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czwnchuq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zxwxekom.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eauvzvqb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2euluynmd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cpaqrkpe.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2prsddhbz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xqfnvhby.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dmdqzdvi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qhwmdgky.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2udroyirj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2cempcnrf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fwshqisr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dslewccz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2dqjhmynf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tmgprqpg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fqrnpfko.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ebqkzqpd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gxnzpnwp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ryeavdzl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2huqvqixx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cvtxdnkj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cccpzkfa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2axhfoqtc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2losmccet.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iistzwql.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mapssjji.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rfbivgdv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bbnhubjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qcokuflo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vleemjuw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cuswulby.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wzqpdpuz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nbzmbjqh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2euxgplhu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pjcyrmfa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lpvbxjtc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmieyxje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pvmfduik.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yevtlwco.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fzegfvlo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2scgjqvwo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xhzqezii.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2airgdvyq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwsjkmjg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpvoldtj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ghunwvyt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jefofrxu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2idnfnojo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zfuvymkq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kijxbccq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jodzrpwe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hoijouiu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qpqmeepq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ufsusiwe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zmipcrrt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mtstiiqx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qmharaxe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2epukaeyw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uejkcngj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2osjvkuqb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2aocqnnno.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nfcllqht.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hdgdwbpd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2flzzoadq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mzodyrcm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hwtywuvs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vjbfymih.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gupaadoa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dgyoqhxl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sbryjtsn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zqrkuicg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2curzyblm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wqiohtum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhnnxai.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xwubmpif.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fqegeyal.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ldttcxpt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2igyytsvx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tvkyffzc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2whcwajru.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tfjggcxo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gkgslfwh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tqkdhxjr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hqavdfkb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gcowdyev.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wllhrgsg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fkghcrvx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxzfao.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gkufakxu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2olszcdwh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rdlsvwjb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sdrgkwei.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clavbqwi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lxjznpfp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2phhrftyn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sazdkgef.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwlbltlv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lebnwlts.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bjlgmatt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rsiqdgqn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aulauvwq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wmkbdcmw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2viopyiyt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bskcevov.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ecgttpie.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rwdtaewn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vbtuxuvk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lqdaetdl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ljodllxn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lmjyddqh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tsplsgtm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nwcdtndw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ghzrvcnx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nrgduqvp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vrvlfwzi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jtyphfaj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ckjedfuw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pwochvke.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wvxfcxsc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ewhefgac.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dhnbsjkn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hdhiwdcc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jvpgvznu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zxolvhvo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oesakbqy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2knvmqonw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jxmlzplz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oizildnp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ncrkxmai.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bceecyvd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gqlqdbyb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pfbsupwg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rkvvnruk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wwmfmods.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2lwrvpjlp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2seebqyll.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yflvfvwq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nmtltiuy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bnohyvkr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2facbtsgf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ehiuqwyj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdghnapj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vbfnvmtc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ayhdmdoq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2auoiotid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vzwftgxd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sdtrhewi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjynrppc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mmdllbpw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwbdxmre.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qrxjyokk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jzdofblc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2aebifraa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2amqrpwbz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cxsdxkxu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kzoksgev.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zcgxsqkt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2umitncfb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njldggmy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ulpfatxi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wdnxzqxx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lrsryohx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2toazrkmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzpfkopa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zbqbdyel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgupwmmm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zjmxfizy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pfsekptn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jcmeltpc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vtnnttyg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hyuiiwoc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbauvfqt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2svwahirn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sisbpwmb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2utjttfkb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wsoqspzw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lyqcywan.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ygvllego.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nhtjgpmq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnhhjaim.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vbxjvjrh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zssiphdv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2asbcqwdv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhzuvsfh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2slqhatfz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kipuyapv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ddmucdww.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ajjzptbp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jiuufssw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qugxilta.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2izncdpka.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xcrxkjwo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ovnwnius.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfwjzgic.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlyzbeyx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckztespi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fbcdujly.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lxbgxqal.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eguouriz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbihefop.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hopukwbn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mmzmuakz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2usdjwglt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dekmpogk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2falznzrl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zgulipbd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yhrztvfw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ybdqltgb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qyrwmyff.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jmjhbujz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mynxdkfw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kcoryakp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xoazoike.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rritdpum.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xkucujmu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mocbrfez.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bookjxto.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pihkgjma.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fguygoxk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nmzntoff.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxvfdunu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jiiergnn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ympbfsgp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pwraxifi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2htlnjcpc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vvrwpyvn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2eguoutvq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvxfezhf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2yqxiorcz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2egmygnow.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jjxsthbt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ucgrjkcr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2anxjukqt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cdfoydem.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmaybkzb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zxmfxwau.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kzhhldgs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fppwuplx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lfwuurus.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wxluhrfj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tytsnlvp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2nwbofhhn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qolfobvv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2birktkmq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hpquohiv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hjlhqgyl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vnsbengm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lryuokvy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tctvcixj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lulrxkhi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ejtpujqh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dznayfzc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kuvadeqj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pzrtwnap.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2alageuwy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tkwmiqfc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2epslmwkm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gxzbkcnk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2unresjgi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tekwkvgu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hxxnmyok.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zvvnvhzh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2szfzdvhz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2einmkhwh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgvqyirv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2srcovrpe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2evvtvajl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xtgafgrb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2snyktylw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2sewnrwhb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mpglnxog.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2emnjebrx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2uwnlupgh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ieicjldb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2daqrspyh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rrskuxib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2krdjdfrk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cedebcxv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xvvfdvic.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mpakmdzi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jzbusteh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2blfitpxi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ievxsofy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2osfzfdhs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fydivdgt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zuknclav.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mtvufsth.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ucqawzog.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jaolhljb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xahraywq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qfqjqvqv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tfksfofu.html


<!-- 参考信息 -->