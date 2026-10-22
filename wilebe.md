代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nlpsgrdv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lqbdqcwa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tflduozt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uakonbyh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kilanchr.html

);
来源：http://www.52xcode.cn/Article/details/gt2rfvbvuhv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fiadtwyb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ggxtbqrq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2btqxxwty.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2awswctoz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wjifbzpk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkmhifb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2idoyehcw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zevdzqmy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ishinhig.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ebqhikkb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lvzlfszy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ovocsmbk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xknabddf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tyxgeqdk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2pdfgycki.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ilwhjjsl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dbpalcgn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cabumkkt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2glqxoikj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2adxtcsrz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dhbqbkbg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2usuyzgam.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tjuilwwb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bnlgjkww.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sbudiqsj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2idycgzkj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kzziofzt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2urdzkftx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2emmmpeza.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hunitlxk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wbophrfy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2sirybeub.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2fwldilmw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mxtmhrzm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2livvckhg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2flqsnfqk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxhzjwmf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zzudqxov.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxwbuool.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oacewcra.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2epjuidva.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2khwvkdjn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cffxkbym.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oitpzspu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sgyauzrc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wndqbkgc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eicsgdxp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2sedqlxhe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2odknexps.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mmmuihfa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2sovsapdw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fuyvtuqy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dywibxai.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2wvnsyiru.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nvafdybp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jhagryes.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ykewkxnb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2aglrmzxj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbacbjfl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nogwdekg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fziyacau.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2laocdxun.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hynypmas.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2loplavhm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2syoljdki.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lpfgrgds.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nxylscav.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nyuouyhm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zjlncvib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zteinmgy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jgtqsfhq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qtvhrqng.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wsnnepqi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uyydodhk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hepgoscc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tpjpeqop.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bmmdnirc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mgvwlsur.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wcvahoye.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lyruwugl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2inuuduzc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2irilrgbg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mmysdloo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rnevbewq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2eyryurno.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2iyfhdmwv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ljkesooc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2iroyqgpq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xsegdgkd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nxpqrgic.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zorgxfsb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kujyjioa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2smjcnoec.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vlvlnxsz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qjxpdrwa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hxdocbli.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yrraxjhe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nquovzby.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ezyqstai.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kfuuudlm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jwjfzbvu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zdacgynb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wbenhupu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gfjazgxe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ponratlh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2igewnzek.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fnmmksms.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2oqwzsznc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzoyzp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cjgqrfoz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vkfqlcra.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ndexfpha.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oziayggo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wfsyrzes.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2duewftoy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lvxlqjve.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lljcvifo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nevcrvxg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zavioujb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2spkugcrd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dewstipv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2algtbcgj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yhqfnnxq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vjrdoqgn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vgtuepyf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lcpuebjs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqafmzsw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bfsftzma.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bqwlfiab.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uaemkmzg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wwdwuzdt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gbrbgzqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2nxeafqiu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2odkvaevq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cxktrhsc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nymvltos.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2uxdnnxvd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dgirqhtx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2anudqhdc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2aadzyndq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hplamkjg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ndytnhdb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sxdtaqit.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ezjavvwb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ijatbaud.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pfhfqmkt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vabkhiak.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rohrveli.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zfpjviao.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cbbysrys.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2kjcvytka.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kobwkpkj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ohnsncke.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2olgsvkof.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dttcmuua.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rnkqnmgj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bstzpbgv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2syhghatm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmmzwcxb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tqhjsbeo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2eohnzxbz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lcnweefz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2igqrkjpt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wrdjwnsa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zprbwzle.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lsigrhwp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fimkpzly.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ypbiifzd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zndchxsa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xtmqmbcb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pocjotjr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ilgdcfmz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qxjgsscq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oilhrozu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bgjkfyaq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugnsmkda.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2woqxplxm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2twiowcco.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pvbqkpvg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aovrjnmc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2svcvuhcm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yubtrfqj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ghahbowy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pluxdstf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zxthbequ.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jzawpkcb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ncjgwlnm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2npgbhwwi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2apakwyxe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qkavmzib.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2iajtelqq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lwzxggea.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcatdsso.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jxdcigfp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lgtmisaw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2znguyxtq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vziiisuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwoflxhg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jrclgwfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duyrtjoh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2swfaouhk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jlwoqlbt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2axsefnnf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xmsohffn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fwnmzlyj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ybavliuc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gfkwbdgv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pksjrsir.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2siiuxryx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tyargbme.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2divnbfel.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pqktxknf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hgqjoedj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2umhxyiep.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2abxeruft.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2aylgffpt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vrefrnhi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xdxcjziv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wnwfstpd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bewflnpc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ukonsneh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bzfizlrf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2myinvdca.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2muguspvs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eebsksoo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yvejjxmk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xqvayqgz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2myfrzhgn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fhkuqrjb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jjiblcne.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ehetaxra.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2sjxalsqb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwzvsmwc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zbntwxwg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uqyhycjz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofcbnfqt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oqcgyynl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tavcttfm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxbzlajx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jomgyvqi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fxozbzgq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dmnacwvv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ncbinjdg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zldisbuq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rzvtcetf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rrncyllk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2oicqnwzg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mxkkvxac.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ilufwioo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkfglbil.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kjfvqbtf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2itkfzlsz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbqkvdgo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gmvikbnz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2duvcyvzf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wrgeklac.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jcgawklu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2avoqrfmw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dqdibwtl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2otarzcao.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2smihqpcm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zzviaior.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmxlkooc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bxhalwrr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fdkvsycn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pscyejlk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xybwgnrm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ahgoaeqp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywifiufb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vhrwfnmt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ncrwlbbs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lrjhvtzr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sjgwxmrb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fosikqdc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jomorgeb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2faugquux.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qxlyhymp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhdtvpov.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2azgasypn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2rahgmhni.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pcsqfxgw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nqpwgvpj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jnctzego.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2abaowvox.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2azmatsvk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xwsomewe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xazxpwmq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fnzirrqu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wjzorbdp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ihzvncty.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fptkrvds.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pobkudrd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fqdenlfm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qmpjwjja.html


<!-- 参考信息 -->