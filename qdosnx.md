代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tsloxqyo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ngoelnhw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ryzqdfqj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ojudnzrp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yzwjlzdd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ttnjwlww.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lnssjdfz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kceibcaa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2itteioiw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uhjbsbsc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wollqniw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bbyauxjt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vjykvynj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zduxcomr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yuofsepu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2uofbfasc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hguthfnv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nyxkfkkf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rvtuqzom.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2khnnffya.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vbxxxfix.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bqbtwdwg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2npmqlaam.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mhzldbgh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edgpptze.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jecdnehm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olgjvphy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mepqcwsq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lgaazfxh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dxdfcucq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cqxwcrje.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dbtkxkjt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fxvbvhyx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lbcolkty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrkycqrt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rgceaigt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vuxcyybb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lumjdylx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lvrzmjfk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ppxaextz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kkyirhsb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ohxruqqf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mouzeior.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ujabicyl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tbehwcgx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2geffyhhv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozmuhppg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ustmaday.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdbfcotd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ftrcvptd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2plinrclf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fjrjhiyz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwsegpkn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dmnttgjc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ludfctik.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ghcglxra.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2obqpqcvy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rsvedjve.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cvleioww.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yzqdmvxt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dlrjswnb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bocuoirx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xvulgeds.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ptzspnsr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nxadrzcd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2dsixyxmo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zgpgybir.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kfiligho.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tsjanffd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xsjtdtcs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bvgwsfzx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xkggepwu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ppjeirrf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tuhfsovb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kyfzqltg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nvznqyvi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cgljjmtf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ubmtxikg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2eshudfod.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ddhwljyp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ienegvma.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kdwbojbq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2legrpezd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rsnubebf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nddiltun.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zkdamndo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhllthkv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2sdgqotpb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ttwfojpn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2piteigvh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bfvjunbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nsavqweg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wfkxpodo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fwvzprfv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ymttjkup.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2thlxaaco.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2odfycllp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2aedkeeqq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mhwilzed.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2todbzsmv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bfmcromd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lwvieqmc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2judddvsp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2joqhpivn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gowiyjrl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zntxpekf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rgaapirx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fgorrjpl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2leezwrpj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hzrowepl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vvufgnfm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jcegkxbp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2igsivlbc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xtaqcbje.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kvmqbwpl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rumxevkm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aenshazq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lcqgpvkv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2emlwaqdz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nxosxnep.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bffdppcs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dzaoidwj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2eezdyqop.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fycyibyf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wjzkoqmq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oiyikcsh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eovphmru.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hebpdvay.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xacelxyx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zbvgbhmt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2snhihibq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2temhvcww.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2utcyfzgf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ucytatjf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rskrcksp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dzkzexbo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mqavzmku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pahbccry.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pgqhnnlv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2echdnjjh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwhpoqmz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ztyvhvjk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jdnxejds.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pmhtyhwd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivxymwsc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2iybxrcjp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2gagctbyj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2urofkkds.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yhorcvoz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kzwntzqh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xwjyhqke.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qhyiaugf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tzcmhhyc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lcduorpb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2woahsslv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rajqyayf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wnseockw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qxjugniv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cchtegej.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hukpabkh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lkkepxox.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2umszqsgq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mcbzuabz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lqxgkonf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dnzmzcqq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apnpuibg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2trmgvspg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zoivnhuc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wvhqnffe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ugjilcgc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wiyggbdv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nprbrbqu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fkhkvmig.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zswuaico.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2udmgbwsl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qwbnmded.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wmzahtll.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2sliejydv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cwopegqd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vxqnxmbs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2znaokbql.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fkkhzemi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nytfgpvb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yzewfpjs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2verorsfv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jwodmxfp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2genvfcpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrmzmbsw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vqjxrgzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuchzeaf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ufjtxjua.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kkuunxtk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pqjuuhnz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2eozollqr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ujsknbmw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ugeltvwh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vremjoyq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2snryeblm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2szikohyg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ocusismo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfgptpwi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rdcthvah.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ppaqhbtp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2oolvuvyd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qqagonij.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jqmsoajh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2veplypbe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ezdsikok.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lffuljjp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2caadpvkk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lhtaourt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2llczzbvm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mwzznjiz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xhiwhyqj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ipmhaafe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qqzqlbla.html

esac
来源：http://www.52xcode.cn/Article/details/gt2swqfmizq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pusgwexj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2njuyizph.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rgarfsny.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xxgqyckk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mqacfnhl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qnnthovt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyzuatai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uwewhlmh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2oytxdmbs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bhxokabk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bkjhiqvp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pirydkvp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zwkcssro.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvsvaqez.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2unrmbkhj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cfxrvgsf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ivhbadyt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ovwnjmyg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxecnpxx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bhmlsgos.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ticuocun.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynwvnyds.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vbpjyqej.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zybgxdes.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xqnlfjnq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mgeyzkke.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vpacbryf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2phgertse.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2eaivfxsm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cpdlchmr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jekpyvwq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xolbqipj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zlxgmacm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2iisnxquv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmmikwpx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2aedhmbbq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2csgfgkev.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ycnnhiam.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fttyqtmk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cbjyrjoy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fmuqixqp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gltebgxq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fydhirrr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fctkkdbs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hniadrlj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2khojrmug.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yhmnlubq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nbabwups.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2sngrvmdj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2awoauywj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zrbldmum.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ozabnysj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jzhqxdac.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vimfcdep.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2biunmcqu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wnvaaeyw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2httemjof.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yxdigbjx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ipprbfrq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aoadnhwi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dfuondiq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zkqjasxo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2eckyvtbs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dvozwcpk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zgbfiaxy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hlnhthyu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uxhsltek.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ldevbgap.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dqqshghq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mfykrgvh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vpkpmqmn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qjmvtgku.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fvkfagpz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plnrrpek.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cbevxbzo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2eqjmribf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hyrqbplp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nenuyflj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mzhhmojp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vmivvqfe.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2scjmtwey.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2syqnrnqm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bkjyhtau.html


<!-- 参考信息 -->