代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wvhssvpq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qfozrepz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vjmlxevt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3eszdtrnu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gdjrclgh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eavlkaap.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gtgbffbq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lkelywsz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xbtmlhoe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3crviruxc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fhqikmln.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3sripslpr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gkytcftm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3eklzxezb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3gamlukdy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tyqelngy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hyvwjooh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qtzdxkot.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ogjnefro.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ntzcqkzs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yjigwhoq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qzavhdjt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ouibmbxc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ctjdxitp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yuscaicm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3twwntenr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3stgppcgg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rkccgpkf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3umzpxryt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kcirowhc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3znxffhyj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ugfhnufl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3srbmbhlx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mzzoiksq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3avwmiqnk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uckjjihb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lsstbqaq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nngdtxll.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jywcmumx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3golgoxzc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dempjeya.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3adscrbcn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ueamsmpp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jcrpwhgx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvelrmro.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xzyqcilv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhspcfhz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ejeoyqyb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etwdwtli.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3duawfuur.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fbmcqxyj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gewzznou.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ggyhdxbw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvtlxojl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wgvxotby.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gmzfbdrw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wdtjbcsp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zxkcyzzy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ntdcswnj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lvxqucrf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nypmndaa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ookxkucs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fxascnyn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3csjmeopj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tnuvgssa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cssgjodt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yxdbrxgd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3anejzcun.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3bffniltm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vgetwbiu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wnpnywbe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fvjrndcu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3anyacxtj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3eigubbpx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3emeuxsjx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bgyfzvkg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3blnlfwml.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tiqsysxu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xlcstqoc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3sbotjkkp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kdmpboaj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wtikfzfr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ghdulrfs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gkuhlzup.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uincjmqk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tzyckpqq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wdhnklgj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xzkcgggi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3eeslfoip.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mosaixcv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnzfjr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cydcseta.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ldjmbbus.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jxqpvwcn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ejpxwlun.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uolzrmic.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3izhlesch.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iyjuqjwc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3boinaaxg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hgkfylmy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcnbaqcd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3agymsaqg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rnmvbhti.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3cdtlgqpt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zhgxiqzf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jrknchbh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3blsklddx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3evqcgehb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aqeetuzi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nsjwzero.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qwmtxtzy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zpbzhvxl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbdhduxu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3snjarxcq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jfqutopk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lpufonao.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nhmiwzdu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wcscwxcb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zwdcbmic.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gnlxcqbd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3umadldiv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mbmptngq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ydkxlkyu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3snzxqpyn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qwuypwuf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3peponids.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ykfgyusd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pzxbxyqk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3baaalwhe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jzehqyvt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3optlkhdg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jazvkgbd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3aietwzra.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pxgeffbt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ifqalidi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rbvirzsl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fxomrksq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gbeorgtf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nixmomcf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lukjhexa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtlxgouv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hrcpaayb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sbhpvmce.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zztypjcn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dewfskhm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3trrfjkns.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3taixfcyi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wpdtljfc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cqvicimi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tjxzibel.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nngwuizf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bnfqdvvz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hvazqvjc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fdovxrni.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zgroowdr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kolphoui.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3rifrvmrh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bidylaql.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ndwofpqh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fvqymgid.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jogmians.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovybsben.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbwtfqmw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dyxzlmru.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bgvebazs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufhqbdxq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ufttnzdn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kjuwscpw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3llgqzvyo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qyoieayn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ggvwtqpk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fhutneda.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bhzbpsuj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3khxsgcty.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gaoaqvvn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dlqteedl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3eppcmfbl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jxrlqcxj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxemnpxp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3asdrvsua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pxjliaer.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hlqesgjx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3khqlazyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uogamocl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3iketwsis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iocisgvo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fpojjrjt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3erqdxpmr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3twojqyva.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3dutpoqkc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rkdqmqkq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kkaxnqze.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mwzrlkzw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kzzlqjfs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xpjhpmyl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3azjmvnjl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3grwbmwml.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kfjvqyqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcbtmpmv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ypaygeik.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tmnithgg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xbizadqf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tnsaofnb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3odcxljhg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eqqwbiot.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3riatstnq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ofwhjibq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gcsxntuc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3oscoacmh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3pdvozbak.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lonjfsgz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3excrduqu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wsyybqto.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3toifxixs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3glgtruvp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mdqyagty.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nkmflsyd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3srgkzpee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3afoxqfwf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xisojukc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kumpmxfk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3brciwpft.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3omghwhmr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hvvxlwet.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xoqbszwg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3eiwshslq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qngolhse.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhmihzcw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tapdflrv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ykipvgkq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ihjrfoww.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vfzjugfx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lkbgycba.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3oxiitpud.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3akgpchcw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lylipbsp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wweilgdj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fwwaeipj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wehhppbr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bibalttu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zluffpnn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nzjhtqdm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rncbqehw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xmtffoum.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yydqrfjh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dbjywagu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jrdjruso.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mkdnueyh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nsfwawny.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rfnrdday.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uaidebyk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gmbdewng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uxkjqahx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3utujuhhw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3psfjmuyo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3stnlndhw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gbyojjbl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fexklljl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gqeaoaci.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3umkkjfco.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3extnnplf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3aedsxiwb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yeqyuroy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ccpgpmkw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3khgmdzdy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ovugqxtj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jomysicp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qfrfrntc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xfjrblsh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jvdkagpt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgmgrq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jdepmkck.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vhjvjyug.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yezzqpfy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3spopzapq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuehpdzr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zdrmmgrv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bgnvsotj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3awlzumtl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qjmsgjuy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ixcbglne.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lwxsdtiw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vdvzciua.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vmhycysg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pyfrxzjg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xgdkmwac.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3neiknmqg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dksqabgj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zqbmviin.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zydkxccv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oxoyzmug.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qnvddtse.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wvaiqxay.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nnhsryrx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kwcduppk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bemmohkm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eiswkdvi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3aulbpjfy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spknflzu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tlwgixgx.html


<!-- 参考信息 -->