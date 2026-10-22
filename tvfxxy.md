代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ggjakyhm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fmlbgmmo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2opsgxfac.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iskvvwxp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tpfpzqze.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vyqxmsal.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bhspiphf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lvlryrhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gtnonigf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2oadwehtc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkkfrtaj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2chigxbkk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xzcgtfmp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2czaqppwa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fnbfvxzg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mlcqrqkm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2poqzosob.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ezarxjsw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ygchfqas.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jfmychfx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ioatqzcu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2loditjpl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tdnmabrt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2isnvxyfz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jnpcipqq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wkidttcf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bxwtzamb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wqidkgby.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pkaoxzfb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ddllgjdw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tqwdyghw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ucojftsp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jrgkfecz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jygnpzid.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbedrmly.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2cudiqmuh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ltwhjwta.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gnksqevt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yohszcwj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2oiesyjgs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zsqmnbjz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hrcgpdbi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2trhaiate.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jgcjirtz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2owwixgid.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wieajkmx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nuxjkifj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yzjgrwas.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lcfplgil.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xjvifyyo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2offbpyro.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2blzixrbj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tlrducpt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ixpsizfs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwkdwjqs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yxmzvcgt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2suzyqyfy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oxevqaaa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vgfvvofy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mbrghsgh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kfsqxwkg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ujzwakja.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uhtfmcos.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fkynwgdp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iemqcltg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ufximabt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bdapujfh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jrwetewn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fyeucivf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ueymcurq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ugoqlfmy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ncxanlhk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2txiofwis.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufvwmjca.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hecrnqge.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ormccyoz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2klyzpwyr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zoentysv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2erywnmue.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2glqkjzok.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2spxivgls.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iuuxgunu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zuklqdbe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uoevsuba.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ksktytcf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nbrkuqzz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ljamyghn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2chtpiegq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vfricser.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dmlmgcjj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yfyjqnum.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ujdknnei.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2scxidvhe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bddkxfit.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vvnuxohw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2oyhfufpk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jnugayrx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2axjmmdpp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cdfsxdkx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2duezmwbh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjqelgom.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tffbcgcg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mdygqrkz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ticmfzyb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ytytqyrt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uxgsahha.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2eyticplu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ichoxxpu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2coovqwku.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xvjkwhvt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zvsmlovx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fpgdryhu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cksumjtb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mgvxegzr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mrxlmkmc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dtnvdcmh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wmatwtcf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mbjkhmes.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vgmycsvk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bwmwegmj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jyenkfis.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uuvxegpk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hayuozpu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lmsndgcj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uywsckks.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lzotygmd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cdcvxptu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dwxsakdh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yebujmhk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fqqzqkzi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pgzyxehm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nwskuzhz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fuzkkxue.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2stmdholx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ecuzxhel.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rxcvnovz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vhkrsxhi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pssrtvzo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lkrsvcmy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vlbhqisi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2enolistm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dzeajukm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2npzafate.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ukozcfsl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bycijixf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2skaypivw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2absbwqke.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ijutnwhg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zfneddoj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nwjxdrje.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qoibjzts.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gbautkem.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mkxjkvsu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ecbsgwni.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hyeueofo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vfxepeft.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fhhuthwr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2muysceon.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ipgaqpqi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pcfbydzh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mwbbiaef.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cgfdyfzk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pwoisdmg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cmnbnubp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lqxutymd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ifdggeyz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mimjvjyg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ydzykhko.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eanbhfkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ljbypisr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yprinmiq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tfutvyoj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mczpnsmy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlxjyoym.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jqppassd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwocacwf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2aumvfaop.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ysfblrcs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kkrgqibz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhrcbeun.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mfhxotns.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wanpgwir.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oihosbfe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zvommwti.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2suweovik.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mqyzfwko.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2epdrratm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cvluyrhr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2camamacy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dsynrmjf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffzvxipp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dfdxleom.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jrajcmki.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fwvminok.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kwsfzwqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvsftwnp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zeilzhge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2leuwdtib.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gocdokjz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pooawbon.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wkvydgpt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2uohfltpn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2abknqwry.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uepqoief.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2manfdqbe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2creuetuk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2okafodqk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kxcpffgn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbuozvux.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2painoiqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2feayigbb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdkklewu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pgbnmlcy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vzniddgp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2khjitnnt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzpgmyax.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ttqpopmp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ifxonycm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylensqwm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xrkfnlyp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2voowwfgo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ghwtjlgu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2knxovxnr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bgdotigg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cdcmaqpc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sexvsdlr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2iyovxxtf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nnzredzr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mweakejw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ysqgvflc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ppwzvnos.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vgjzbeaw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ozrvposg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2oxtsgjqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wberqtjv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2okpqfbia.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cufdupik.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2axkhwpxo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jaeibghi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hvhslsvi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mvdoldfg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tgegljlj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwttbgpz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2asirkhtx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tpnhiqvl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cfxitysy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2alitbmvg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fktnduim.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xpbuudxj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kraswqnj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tcqmgdde.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2whhpoglh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lahlzxfs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2aatgwbhh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ddvasase.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yrqmkpud.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rtwqwotq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hsyfwzji.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qpfclcwr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lizpvytl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tdbcgnxb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2totjoepg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2bqxtgtfy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kyiswafp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evbadbwq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lvgqnmda.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlusoppn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fgqhlsst.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2yygpkkzd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jodxcwdj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xetppojc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uafsiomq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2odvkksvz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bouhodxt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2uulgusse.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmgwycgk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hxvnupgj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qntmtfgi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rzlrgngg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nufwexxf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2owshmkbx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nfqxnesj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gfetuccm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wmlxjang.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lfjobafi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nfsvkfdy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wzqhspyw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpibwdbj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fcyzginf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vrvbphax.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vrobpsah.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bbpqclfp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gclfrddf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2eudywmgu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gdygfrtb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hzansiks.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2scpkscpo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fwdbofmj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2shvdjdct.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xvfnoopb.html


<!-- 参考信息 -->