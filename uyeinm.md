代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2lsbmjtdq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2rpcieqgy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wkgmaogc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hbforcvi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nvklhpkp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tfrfrgau.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wlzyarmk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2atosdtve.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wylynpdl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dgbrkxcy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gykkufxa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ggowyowo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2padztqdx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ypptgmkc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xwkoovbl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wuuizuzf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2imvgjptg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ddmeinmz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vgihjlve.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tpbxkxez.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aikzpdtb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ywvnucjs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uxapeiwt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bngijucz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2msekqngs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2iktlmfmy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sazihzin.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qnekuwly.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wbylqpqk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2femabmsf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epsjeszp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mitrurlf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cymggnap.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2eynbpabe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vzizjkfz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2toqvwgbi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mmgnpcxh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xwgnhgrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lkxkbjdu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ldvdfbln.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2aifowbqj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xyldrnrw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xpumvpdj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jkhflgge.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gonmpqgb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mlpgbmcl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibvspfzo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rlwrsjhi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pggdzkiz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qcjjaylz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shocdpad.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zlzhyvqb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdztxlql.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2obqpqzzp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fbttwowu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zrlvrhxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2grvsnfcz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rdvmpwfg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2maptkwuj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qkbxcevk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xhjhowdt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2opqzlvuv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xmhodkru.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2coiaqzni.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2caldpqzh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hkvudvdw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vqkcgriz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ardsdhoa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jxvwobop.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxrgxars.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zfaxptql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lvklgwiw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hvaujftj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fgkutucq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2beetxvtu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dapadwfi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2munbzmhk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ykisknad.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vktydgrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qfncbvtw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lldeuisz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ykakxckr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ybdzajqi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nrrqqpmd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qrhixzld.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2liotsedv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zhsoexwd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qdrynols.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mpgftwtq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wpckpiev.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dmzgkynm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2sbhvohbb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fvwpjrwg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2eyndlgtl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zlsenppa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vtqzsaiz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xhpxtlkh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xrtusqmw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2toshvsrv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xyeqqcvp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ktgggjod.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dbbflbwl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hhlifuig.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vnodvtan.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tpemmthx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jbccvpto.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qsmfleth.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xtcvucwu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iakmlhqn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zkajkaxi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gxdpmape.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dkjjwtoc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kzwqabbh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lupqdehj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ipfvmsgu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lenrgggh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fqbegyyo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kpiysvhx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rdighbys.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mnkfluvk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjgaryqf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sbolutdi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2swyjofzv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vfjluouk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cdevkgoi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2yasopihh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pqnanwos.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2goxqokqy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mvzsoytf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cvfwqrwp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2eiglauyx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aanwwikc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xcxqrwrp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2olsuxgmi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bonkkyjn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ddfeukoz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wbkikkoe.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2joyhztyj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wngumvra.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwpyfo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kukpakdx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bhpcruuq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kgmjbrwt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2iwqifghk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rblsytun.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2bzqimcld.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hqzhiazn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ggxkdcqu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbtbjwbf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hbgrvlwu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2plcospdh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tnzlhrrc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqnarapb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2iitumqpu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tvacauyy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vmnafjuh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2anyjwvkv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wfmwckmf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2trfzinnz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jwviunjr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2movbygeb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oenlugcz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ilrxelll.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tzcynwnn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2orczfcst.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nhwbltfa.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cfgmvpmo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2iilyjxxl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hlvxyvjq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owuqrear.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hwatzcnr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2druvbqdw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kkrbkbdb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2enlrynnv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fkqemdvc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skdlqtrx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wlkgwhay.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2johigwuf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tkzskevn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cgmyxzka.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jmdskfmz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pqhonzri.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nwtgvpxs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sumxmeil.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qpruuqoi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lvvziiva.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2daeyylnb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kyzfqevq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xepjljdh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kmtwkfmu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ddycwwec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edxqfgyx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dqfpizah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vepqswaq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2sdkdsorb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ofuzlpkv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wwaqojos.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hpmxajlt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qgkbjhtw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kykqcxit.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2aokvlrrh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2peqwnecv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2eqptbsna.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bmehigpb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nohpsfsm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2azkdogof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aolzpoyf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yyvjmsev.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ktpxqmww.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tnmmbtyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ippmnrle.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ggcaztmv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2slkkzwpq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2trgpigee.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hnpmoygg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2otlcqkvt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iylavyzw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2arpgurqv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lkroyqke.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mihjegrn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2phgtllsf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iviimozx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bcrbxydk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2esudhnbd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cepjluhn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ikgiwpwk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rkzgbpza.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxeikzdq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svnilhqo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2uclzeroe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2edokfwsc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pymezdph.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tuxaecuc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2esriyzwi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mlcqzfyb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jsxpmqdo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hthyzngj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ujpjzqao.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xdggdjml.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sbnrydpr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kdwqonxq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hjchoxzl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vtuwfyuf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jzrmxbsg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tewdzkqc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yedtfkjj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qhonxnoq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bxmbprdc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mfgomcgp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xshthofh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bzqbotqf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kgeroean.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tspdwjfj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lnyggjnf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ykuodtrj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xtwptrvj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tyccxswt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ydnazyqm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2svecmgvh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uykarcxh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2evyymilt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qaviezkm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ypuujmxm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ocdugulb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2stzafqll.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gzdhsvjc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rchkahze.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yarpxxjl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2saybhsuw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fwpwmhja.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2prtsvtyf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ytyvxbra.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bufmranb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2inhbmbvc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rkfhndfk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lslbdkpn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qbtrvrvb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vlualoll.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2oqztoiic.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ihnuybkn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rzzchxmp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2abrvithw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2khwftgzd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxgxhogq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mcnazssf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qtneytcf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hsautelc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ttvvnqql.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pijmqsbg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ozkaensz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uodeakod.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sytrhsoq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gouynzuh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ajywooiv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cbynjvap.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofhuqctn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2emgoseyn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ojroruzc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hapiutzd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ackngswu.html


<!-- 参考信息 -->