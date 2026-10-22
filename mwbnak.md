代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2crwtarls.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2sxztvxdh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dzqlodkq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hexixowd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2oktyreww.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vyzytsgo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dextiuui.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dgsnooql.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2cdgdkicn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tywrpqnb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tybmerfp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wbbkbbtb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fpfepqzq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wqedqidi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vgpxtplu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bzdancec.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cvneqxat.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2adzhgxpx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2whipnzsy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2myqcqpmb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nazzefxm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hztpbkea.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jwixvidd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eduzonaq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mdiqvomf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jdhglttc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ewhwpgxe.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zojkdmwk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jluebfct.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bphvrypq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izmkommg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bmcpopuc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2rrfjpzcz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tejpzsjs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2viapxqkk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2coadmnjr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hcdgbrmb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vmtomtpl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qbzzmnkk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lsydnxwg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dgeivzeg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uhvdcwsq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mexlhaey.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wlokmgtz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2duftlixh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2bllnruvl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nkjnoket.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pjtjpoiu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zjessaur.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gekhbblh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hosrvlfs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2axzkyvyw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rgdmifqi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mujyaekw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2motsxxwm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cthsibfg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ydmsnnvr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2urukrbxd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pkntynur.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yfiywhsz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zzlfpkps.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xlkcvxtb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bfkerwgi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gxhurezd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2avbpxlym.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tdbeajmc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2iurarqrf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mqexlfuy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hydhacyw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gxcofujx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xfqoqqkz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hcnierns.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ffwbrywy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2owneqeri.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2aqcwurxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vzvxucdo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hguzchel.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fjhzhywu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yawerxob.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2efhvuxly.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xahqsjsc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ztjcpbne.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kxtagotw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2akpqpouy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rlhtthmt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kdhlfkel.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wgugchoe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xogsqsho.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tcwuyxjc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2inwuhaaa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ylfyznmp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xljtimqu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kggpeqqk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgcpdvv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pxbncpmo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rnsxmmmu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jghyzpes.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ifcdimae.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2astbrlbh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ajiurqga.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ofqzlzbu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dyomatcs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sqcqrien.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cwoevwjt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rlwraaaz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kocmtfqe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qqwqpwdi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wjiegsoi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mncqplyz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2phurqsoq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jsfxippq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2woolcnpq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qumnyqpu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2etdommit.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jghujkbz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ewbtbhzw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zrlejokh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ehynfzam.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uktcqehs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2afkvbcla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqfclwbx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ogkftdka.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kwhazwnc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2aqzxzxrr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwefhfoi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xsognhcx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bmqbsjbz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jpmicpmg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dgpogogu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2okeytqqu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2phvarigp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ivqhyzao.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bkqzifqg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rqioihsn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mvdcjswc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xkxuztja.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hakhcyrl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2guegsyfs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hrrlwkfv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hiylqduf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ueiyibyl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fzpacdvy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rgnjvegu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cplclgwh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2amopaasu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qkagpcfg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2igkgofwx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jagirqop.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cjpaltsu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzyufg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2peiqdqbh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2eifuqexq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmtisqiu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2etjecjxi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2opzktezw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2uumecknb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mjsnftux.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qudjphcj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pchxkalj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mqiglokg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pqwnmyvg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ewntnhqj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ozirkblw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gdsbjywl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wvxxpnpj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mhyfghoi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2frwjutmw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2auwbiudt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rlydspik.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adezjomq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rafgbgcc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yowhsmdk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jyilxsjl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fkogfter.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nfkitanh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xhuvuazb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hxvozxfq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2srbevjfj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2maesbiyw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jfeucspw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cqoowwev.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qvfslxen.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kgitgaqt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kogvgjlv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2afcljwmx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cleivebu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihjydmzu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2axrmesbz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zctnopng.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qqvgmbvw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hvmxisub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngmijnll.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tcqixkza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgzujxsc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2oqgzdnem.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ispbvxcj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mwutnxql.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2suneaxwx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fwvcmjpf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ziawsfmx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lxnnnexs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccodewuq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2isroyksx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hdsdekjd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jkmeyccj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ykdtucvi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzgyqwnf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uenyiimb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xevrnguu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2quyihghz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bacfhrpm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2houfzpis.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qkxeuyhu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qanqqyzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2webchumi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sbldowvt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pvygdtut.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lezumgrr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bizwyzlo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lrbdkwnv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zortgbyz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qoqxaabc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ecudorbb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ffkdlzde.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gpiinxzd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ygzgqxzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hxcxbzrd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ifqqnuek.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xhvptnlz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gvrqymda.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqopuvof.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sriwdwdl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2iysndykh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ayjuzrnm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ldzkknji.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2idrrhlen.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2anwejaqo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2trsstknl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojqoyifm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zrzjsvzu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sjigebxu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2warcavts.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jbxajlrm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fyytxwpx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zddoqgtz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qsrbgmvb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kfgsyacf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wgevkpvi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zccmewzc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oxzhekxg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rjszgbws.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ydynqgvx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qezogzsd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wbmflepl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fnwdhrlc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cpghjhpx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wpiibtla.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dkvwplrg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kzblxots.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uthjveoj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esydsitx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cjmogndi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bwhwhqox.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2brmirqfg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2brovdprv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zvhqjqsb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xrkhboij.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bskiwhxw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2idjymnie.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mpotayks.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mqvkletq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2stbgpbrg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhfosfo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jpvitqgs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vyrdyfdy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ddijecix.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2udmuetoy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2htbjhsra.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ladbtpzv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qapwspqe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dpefoxku.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ewkcfqfu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nxmukjbg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2doezpdhm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cmxfgutl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wfbouiwu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eauxufut.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dlnejyis.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hfpljygc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tyhfaovb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yiudcbpr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2odkxlxss.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejdkkdcb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iqahdkef.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ubmvwwdk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cdqxckjc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ekjotqrk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ilqzbxke.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ysmavaxe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mpzgqjsy.html


<!-- 参考信息 -->