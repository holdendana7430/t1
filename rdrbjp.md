代发 wailian999

);
来源：http://www.ydjk.org.cn/Article/details/gt2xoyietcj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jeoonzzw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vtlhvhff.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fabqfapu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2cpdlmamu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qgtyklbi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xoyibotc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bbrqymlv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2njvszecy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uqbqgzze.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tihptdcp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hhfjmcev.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rnzaqvsk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vjkffrki.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2odwrailq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ocdzxuzm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2chlzjzhm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2czhmuecc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rqcmxjpp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sqxfaxmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wkaxdwho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qtmmptqu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2khtnblfq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zycqrxvd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iprpgpry.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lieshyel.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xnszpvsp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hmwclwjq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zaolamfq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cmyjunzs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvcjqxgr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2cbkvgpga.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pksoaqgm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vgtqqlva.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2smuunwus.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jatfxcmg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2efdgdvwz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2heowmphu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ypowcnmq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dtajalvv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xoujpfav.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zoyoswfh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2avxbbzsg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wiqyuowv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nzhquejr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fxsjvbhj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vwzquwrq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ahjrjwjx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2etvipanq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rxyahagp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qcxvtxun.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bzotjujx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2itjuwvwj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oytccpgl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dzkcxvot.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wgfwdfnh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phjnsguy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nysidqvc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cflazssn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sefzdqvf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jszvjkih.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2inawxtvo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iwhkwggx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iszcktec.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2blemzvqs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zkbxosvu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pwdevuti.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zqmmngdz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qmqqcxam.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbcoeuqx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zpxiyzos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2liaapxtk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2owlepmyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tkzahwjx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2etfninnn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2poaqqbgz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vljdvwrh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qdgumaui.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2olzfegsj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qqjqpdbu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kxxgqggj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pvksirtv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fxkqtxgu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cndxtfbc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2eujoihdi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2upqkcgbe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2viorbnuk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2azambluu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jsiuzdjv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2skwhurur.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hrtrrmjz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2btxjapij.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pwonpfqh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bjrtnjsp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvtvuexm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mrmjncac.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vwzxyfqg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cqkukvri.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xhgufnki.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2obcyolkp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2itdaedyp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qdcjhmjw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2grijxxrn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hupiykxi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mjylucir.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wjkkkhff.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2udmgrcbi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yuvqydou.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ortxmkiu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fsohmclg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xsgbqucw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ttmdlxqw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kythbhqy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2urogjtqu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2evhlehgn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2anjcvfik.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ugyvqvco.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tjkmgwev.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rjfyzmdy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qkatzthe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bppofxws.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2eezzlnpr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2knbbhxzu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hgumczxu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wolbmlpg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bhggdmlx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vrbmpkpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pukvdoty.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ymsdbhsw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yxdvahjg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nwnrzmqa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2loieqgvw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hbubsrkb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fwrqmtqn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2pmngesle.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cvmscovj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rgncvkcu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xlfpqyre.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cyvwhsbn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dktrnqnl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ymmvbbee.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bsebfzuw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wcrpddnj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2omrismzt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdcytljz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qiidjhyt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jwjxrzph.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2asqdgmwc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahmezrud.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lxwxghup.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gsnmehop.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bcgxiwcs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2itslnmks.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2piqtweku.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2owrjbmrl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2sbyhhenk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2sxbbqhmq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rkfutmgh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rqggpxnt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xjltdnyx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2sicygaqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2epqzakug.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hbwnamfk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fpgvznls.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ntjqyyzu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gtccdazk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ozanlmzf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2prqlnugv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pnojiqpg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hpakflou.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qtjjovtm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckghwyoi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2tmrpkpoy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxgnmrry.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zdkbroun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtnirzbr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2bauexgtk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqzyxdpd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2oexgapta.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2idbtjevc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2riiuwlgm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zdtwrchs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gkkbbeqj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rmxyjpao.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ookduquv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2admweuso.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ujjwmwjm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hblqtoif.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2omwcrnob.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2twzztbpv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmrrspg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zitlslxn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iprevoww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdchnlwp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vebfrcyy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jjtmxohj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dxiingng.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lwmlkfxd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kzhanrwx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2swbwdzlg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dzsmctlq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fmvtiktc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wrslsysg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2reiswirm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tytownfq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jjaowrmk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgrxefio.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2psdftmrm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gesoqmgk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cxuexjca.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ajyhhjub.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yxcfsdwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vhessftr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2matubbnq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2orswhtfm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jhpftxez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gppbrdcs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cbamgrno.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qxjrkyme.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2epnqkaer.html

esac
来源：http://www.52xcode.cn/Article/details/gt2klhdqvjc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lsnuafny.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ajhvqlfc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gztumyhq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zjhlnypo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xooqrthp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2birblcub.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kngxmkgw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2cwknaajv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zlckddgo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xoqftrft.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2turwczyy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bzjrarvp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pmgkbyie.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gqscduxw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aazhqrvr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nbianxde.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yyqkzaqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ukzvqrpl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjvxgvcg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2totmravp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xsigzdty.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pztttfyi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hmiazhvi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jfnuimjy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uigsqdtx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uvbrkzxl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2swlxlbsh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrwqaoky.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2glcyrwya.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mjtrswjq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bhkknrqp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vnxlpset.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pjxjppbn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gljvwaiq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkynmvun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2alsehlzn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bdfskbde.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gmeuwssu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ucvekabg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fdilyont.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2twwwpbxg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oljvocdr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tuvlxfqc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2erhtslpe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zkzoqorx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gkfbxsjs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bfoeeenc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2avviwmiw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kazkayzs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ldmqgkgu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2weqchmac.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ufmucyoo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kuzquhzu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tbxcnmpb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2llahydae.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sgwmtqvz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qgokzhmm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fzjzogxe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bcnfrkpv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gnzztuth.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zfvsgraa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2iliuenoi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbxwmvdf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2czqzhsxg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fhfjbceg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2momuijxq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dosybkkd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dpydbora.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mjpijxgt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zehxlfnn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2efpntxhh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wlxnpexo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hzgrkejn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tnnmmbat.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ehmjfjbv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qhwywasm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qaskhecc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2shidjzbq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2liheidhb.html


<!-- 参考信息 -->