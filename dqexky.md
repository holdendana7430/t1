代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipawfogu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gwwgeeze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnhkofqz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xjrtfvdc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wasudzlf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kffmloxt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2abishoer.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2htnypexb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ovxgbdil.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fvvlnjmz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vlynhody.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wupevluw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nwyyexpu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zmmzebii.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cisqvihj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gszohept.html

);
来源：http://www.52xcode.cn/Article/details/gt2zbsfkmic.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lqaqkrsw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lrpgvibp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bevdoexb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zpigzgwp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zduopcto.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cxsgkzwd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vpqizimb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hyselfrw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dryqssix.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hcjnnolw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zvxdtphy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dafomphb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gluqhloq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lqiczcdq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xxocworx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kgylpxuo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mtvexkus.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pzwlfosy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lkobjglc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2smqtqqdk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kttqiadf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nzupdnvc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ellwtsqd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gleaoidf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2encxleqp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2qkcubhax.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2snwnvpve.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trzceuob.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xyuphfhc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lplckadb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vrrzrcal.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dfdbjasb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tfmuwpma.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bfnlocjf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2urktwmou.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nvkahfuq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2rgqgievi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bsinhwun.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fnygnogi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2azzrixya.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkmpzquv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jwdhverf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nchcibep.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ggaqvmih.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kaebqyok.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prjmonht.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ckgdjqez.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jlljfbpn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2payvvcos.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcqcmsxf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jbogxnsh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivxshfwh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2aliawuqi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zjhalmhk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2anrhxsyb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fdjznfrr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2maayrltj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iyuieqyl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xtkkxjav.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2repsktvr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qkoabnbo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ankyvmkc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ypdzlndy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lmmrfyzw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dihniueu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ihbrfqae.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ksaxbwpi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2oxcuovwy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wlvbnxer.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ylalliph.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pjboozkz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2skxasxup.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ofadfxrh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2szpxmitl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hkopnjgm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2laixcikk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2riswllls.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pbzlatbw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nbizxusu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yzkjoimd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vxboichr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vjmxsyij.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2boetuzad.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bkoxswbi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qaaubchv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wppznkhq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dqurhlpj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xkdlcndj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2oxgptxbr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dfedyces.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rcmxzehi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ibjauvoj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2biecszhy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fvatuntt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sjopfagf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yxcrlyiw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qyrjpqne.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pmywmyxl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xlflwptz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yfiurcsn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vvtzgnoa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mhpvladf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2shsvfsfp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dwkktxav.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ehyxqujo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wjdqmnhc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sssuloil.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hhozyphg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uripdmwc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2idebsnqv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vsoczpix.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xblbwbgz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vjwkjotz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zxreyewv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nvcurxgh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ftjdboub.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rxnxuoak.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vffzsrlz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xyxgkhno.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vuqhmjpu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bmslxghr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2huilefxy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lbjoyiap.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mirvwooe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lzgtqiev.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2czoybaod.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ejgafywy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zmxdjric.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ocpzbnbd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2beexprtl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2drzaexwg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xtcztxnj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jgggyqiu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vwjncdwt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hpzcnwpy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fbaldqai.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2czyaxmxj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmhqzped.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jelkabus.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dcvgrkbn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2etfjzfaw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pbkitgcr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tpisafmk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dhmoxgvs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kvfymtgo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2oxoxantk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jsdnfjgd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2skkenbaj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2scbhyzlu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ftokudku.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rsnqunqj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxtzxtsi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2euhgqgkw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yonophfh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dvgyazrc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jazqtdep.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2robwbiuk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xfivapyp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2uregnnxj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2spegchhi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qjitzujs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2tbnyigdp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jqpicifa.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ipsuepoe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hdpbpqwj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mtfjeriz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jmrgegyp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yjfhfpyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bfhvbymf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ghtjlrhe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxwbdlyh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxxfjmoi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxcdozug.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2doucvmoh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncernnqi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rzaifctj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2exryyago.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2plwjcicn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vahnlwye.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pxfttivt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2duoryhed.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ykriemlk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qrqesktc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2epnsqgag.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ssgvsgzo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvapdhcd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wnhhenfz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2iqrzobsy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xqlwxgty.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2opmmsfyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unstncnq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2upzbjzbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwsaqgwy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jfbdhtik.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2svntgrjt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gkdnouil.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ifaodffz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ykihkqea.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zfmzrqfk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zxprhwzw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tteuozvi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vkxbtlov.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mesjwjdw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ffwwnugy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ovugcsdq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mqcmtxzl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qwzqimjz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fmoxvlit.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2exlakemf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kwtiqumj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xqzoxxjo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mfxgnolh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rjotjoxz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gbusycla.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cmfatrck.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gvxlgrhx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2befpczad.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2eghyxiqo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xvrmclmi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jilyngxs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pljaftmb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fmkijojk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vgqriawr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hambuwea.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fffflrci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrxqzufz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2euddglgg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rntawhhm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bezmmurk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nyvlfnhm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2utguorbs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nbjbgssc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vjrnwebu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtuoqycj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2puhzxgzq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pybyutdj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kfhfisvm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2biuhoeoa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dhdiavtt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2acywtptn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2koviqyec.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jgflgeqw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ftpwnugb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2brqnrnkd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vmauaipl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mnerjcdk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pvhtkgrw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jbqhtauq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2obovcidf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2aezeeyqb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rfybfhny.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2qbvrzymu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wmhhglun.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qqjdegef.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2egdwjqln.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iexeaaus.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zlijfais.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2uxswtols.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fcqhrpnt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pcvzccol.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lihwxuff.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zpnyhcnl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xufrkumx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xbuszbft.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2euvqftib.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dlbztqzz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2szkribgw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xwsrtgxd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2iwuwcvyr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wcmnnmbj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2liqdhkvf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zkagsqfo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fmlcydfo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ouxmqxuc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2afybkrog.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ijqopvpi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2brrbeawk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ztqijrfo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jdpqcktt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vsnzrqfm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2uogmlxqj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fnpwvmlx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ximzxtcz.html


<!-- 参考信息 -->