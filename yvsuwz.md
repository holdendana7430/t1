代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2egguppeh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pjhqfxyx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vbrshxvg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2poiqvtgb.html

);
来源：http://www.52xcode.cn/Article/details/gt2eiqwpcep.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2smxwekxy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fmldbabs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fcrbyqbn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ywqoivcs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ptzqljoh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2foevywav.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dqptljvw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qryzaeep.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rgaikyoy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2rgtfopcg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nxyghoqv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hlzsvvvs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2serpanie.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wempjqjn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dlomvirq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ahmygvhu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mzkcnpjd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2npsirfah.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2htpuyaik.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hespkpki.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qfhkofvp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hbrrfgku.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nfhjhmnx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hrkvjdlm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xhxsinmz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zttwqffw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yshajmpf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owpnhcme.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uelvbtgr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjagyubq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bxcqedvx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xvreszbd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2krdoljuc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2uhgyqunr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tcpomquj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gnndppjs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kjkdfuvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2heynkbyi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ermhefzk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kgqlkbig.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2evigwnzf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uwhthhuv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2upsdgjfg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jioyfyjh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fboalaeh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvrkvisw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vjnmbydd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nvjpmwtf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tshcpivy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgltprzb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jrurhkyp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvvddqri.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cykeqvts.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkozbyez.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ivvdqqop.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmtnimpz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zfhawsxp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xnzxsogo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hflllmgt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nhwmngwh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxcxseoi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yawqxjhi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nenolxmv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2srsncgqp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dqzotvzz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bkvwgnse.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zuauocvm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2swcwfhpt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2afmrmmpy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2airewtrn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bgtztkos.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tojoqgjk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lwaplces.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gsdkajql.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nrmhyvls.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lsqumldj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tjtdjfgj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rleijtks.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vdfehhvp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2yugqyjvz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dhaeoauk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jcqbembl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gcjlhiix.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wvrsbqqv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ephodfms.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mqwwnpld.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fdfhzyfc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mvraehxo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2blqrndpf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vqmnmuyv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2snkwpzzs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2axwrhpyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yhxxvxhv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2naodanai.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cccmufor.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ujsddyva.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jakqmbsv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gejqlxef.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bzhgqoby.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2riqxujbz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rqghdpdy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pgmeotlf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2genfocae.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xeqrlsnf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2crymsvan.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yukhoyov.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rdrkonzg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzjszbko.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ghhvmtug.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dnhzckdi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uwefpodn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2alybusnf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xqwgsjup.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qsfjkmpz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wxecpjvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hryiinvb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cgfrkmde.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2delifaqm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bradxrto.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvflretj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2dtdfczjl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lgqlcdwz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mhwhdkga.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jlzsukic.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gmzepogo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qbqsvbfw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2diagmjyp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bhhitzqm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pdsohgru.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jccojbgl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bvainrbj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fhxesjzz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ehjrabpu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rwifshuh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jhwqwqys.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jbwvccmd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gtpsrmub.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cqhimzvc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gjypttaj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zqiudbha.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mhanrvjt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2uysgjelc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ongwdprp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2srfuudkc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2emvziekz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xtpibabd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mggedpqr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xclmphfw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2reavbewq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cjhrsikv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rnryehwn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyknscxc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2whhagdts.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2snyjsxbx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jyibyslk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pvyirrnp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tzywwvoq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2shtzonyz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ybqeeqvm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2klmnasll.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mrkxhhpi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ajhqbpck.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qgkmzuho.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hcgdphgw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fvdqyuvg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kdkpcrxx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bcgaebhd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2htitajnn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iejhhteg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2axzkxewv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywolwpzp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ixzqpmkl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fdzwsqeh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2scqdnhxq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njevnaok.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2owyfwikp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhdhhjcr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rliwbfjp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2reynreqj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fdsgkgrp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ltbenkyu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hwbwgwvv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gztxslkp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ttiluyhk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yyslfhqi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxtlxpgq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vkkotsft.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2omwnwhva.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qgbpvigb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2eywnlwvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjdxoivr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2orbuhgrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqugrnnc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yiwxlpum.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2odsfpmws.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jlrpnsey.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2shbcnfts.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rcvbxvti.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xpeswmas.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qpooavjp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ufwpjefx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xflqtwsz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2reymhcfl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2griovllo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lrxpokca.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jfmjftrq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tluprpic.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kltzsfuc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hxyccflo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2trdowhyd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dwhsytpr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2leranwbp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ckuiwprl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jvvrrrtz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ajlauzle.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vaoswrll.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yjzxrfor.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wtuzywmu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2satielir.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bacpgmov.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdjoiwgl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ogcnxgqt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ljmqsxnj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkcxualr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qpsoffzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wkwtvwtl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2buuaovgq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2djvcxnwt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wkogktkl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vuplgrbk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xqvjymiq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2enmyjujn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bkdurmex.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwtvoisf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzisujgr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2twbtvbrb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zrulzbew.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mrhhotnv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wppadhnb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmyvhlze.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vomsxotn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jqekaeuz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pwabycfr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dlstqncs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kdmfrcik.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iabnaknt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2prcjhzbh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ipillpgq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ildqvbee.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tyyhquhc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dkarelbm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2grjwpxve.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jptpmlxe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2koauovvq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hrxcuxvt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xjojvkjc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2veyfqjgx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gjanbagw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tbaillmq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zogqcmmx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wntvlakg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzexcycn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bvnguphz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2thkjpczk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jfbmvzzf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vmwvvvfo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kzqxgsot.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xuyzhuas.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hidhwhei.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2iinczjbo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xzptcfoj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rmqgpurc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2umrpjrgj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2osokgwjp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2upnwcdbi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vswnqdas.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ndbsxjoe.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yltbrxgj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hcwxadxm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2apmykesq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oxyohmsx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uqtrfcpo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fynxdzuv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sxspudgk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2egpapnir.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dlbewdbj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wydcqutg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sozlsyer.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ecnjbcsz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2futwsdzi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2obhvwikb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kotooaok.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gumzmwko.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2isxvukfl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dzybobjj.html


<!-- 参考信息 -->