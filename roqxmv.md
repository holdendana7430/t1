代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdtowsbg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ybazuozt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqoiseom.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ajrwzgnm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jookwafs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kyzwftdj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dtnbmbor.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qvhfebnr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zwaigyjk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oprzbibn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ntylieym.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gzafjgbc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kqrggcyp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jusvtsvf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qfntcglp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zzgvwklt.html

);
来源：http://www.52xcode.cn/Article/details/gt2yplhkvld.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lxkjbcwt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2srdoimik.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ikhjeluy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jphchytj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dmknbxyg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2znbmixcl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2iccjdcyx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mvnvjzet.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2szvqxhfr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljbjcpza.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uvvtlyvb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cvkgtnki.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2oreuvhgl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wnzqhrpj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yfuhnpol.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ebkjfona.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hgazhcyx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aglpurzh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2adardwlq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fsaesetk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rnickaxc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zjbxghca.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zjnnwyut.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hagiorbi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ccbrerpq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2irswyzzl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ullelwou.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvlcgvzq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ouyuckap.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sialcryr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rubkfdnd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wgdqawyf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2njdlcmhe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dogjpyxi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xtsbbqhs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2aqnenzef.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tcixchcz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xqnsmwlh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dovwnsvo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lyymabhy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jgyrrmxm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uusqbddi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hyfgkfzf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vsnihqqw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dhhmrcwc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrdtrgys.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mzcmljuh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cuqlrkuv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pxspqbkg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wooxagcq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2aqdihytx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krcyqjbp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2apfjedyo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lcomwwne.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kuecfuiv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tixvkepr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qanoesyd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dvxgxzsm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fbclxisc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jjtiktev.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ygffyjxc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zzzgcpbp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ttjweddx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjdgeq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gfboehcm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ofjxnguv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2otbqcyks.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rnyuztil.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xseahcab.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jylnjbsb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bobzonun.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fewfuxuq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mgrlhmwq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gvikwhln.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kljnypct.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zroovvwu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fyfjgchp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cogspnng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pknekitj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rpnyzupp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2spkzofdh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tnmjptow.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mncfapya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wkgdbtzh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ytnuccpz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vcmyagau.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sclgldpu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vmectdyp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ogaltnzi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvkoda.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2eezuqjat.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2sfzqdpnx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ymyufuoz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2sxgtjxlm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jteaqyng.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fnpdlegt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lvcgfkyo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mdlhbkga.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ypfbztql.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2evfusxrb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2coaiiheb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dspzyqgm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vjpynncy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rjgsmdft.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2grajypha.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2amgvwqgk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lvfclvvc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sryqlfcj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zugfuslx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jzpmgnmo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kwrqyvyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ixfccaka.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zpjwjuls.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ljgtypva.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rvrnxwjr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dgndlfpf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nyqnbkln.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yourgikk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kyjeqccn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dnsyntvn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gcufjmwf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hbgvlmga.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2koitzzrg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2depliprb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lnottspq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ltksjxga.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wborrxsw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ulsqxzaf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oicrdbkq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vzopgtjr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2atjddola.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cszcnavo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2oacgzoec.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2aqwinolj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bjwdepfa.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kyoyykmn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rsrnywom.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rbipgspw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hoavyvmk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kjvkotjv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jgqfvpuj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ucuyltvj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2feslwrvx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2otqrzoqw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mryruymd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yanmeprb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xnxceyvk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxbwojaj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nhwwgnpa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ihimujub.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bwsqowuo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mztnxtlq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ympqnhsj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hfdqchyo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jgsbqhon.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ngkvdfxy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jfvxpyda.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stxydkmb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2sdkthufw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lxmlrgvp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ocsiwbaw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2futvekrm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mzhpajox.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cqjnfrpc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2usueftsx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zxbchxye.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2psqfiigd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zseddhva.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmjpegis.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mehtziil.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osshfibc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2otmnrfcd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iydhisig.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rfsrtyci.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnumirrz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hlqqooib.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsqxnbrw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2obrpcsjf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kndfkbmx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qzzntqyo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xzmoggxr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lnevcpxw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zhmibblw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uoizcmsx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gfosaemj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kcrqaqey.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tazrrajb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2iswojgcv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dloesllo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbjzrbwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfsqfwub.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mpsnhqvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frpinnmv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bykvvflh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xgvkwkeu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gxmhmoni.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iktjbcau.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vuwrtiqo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqvgonoi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2usrngvug.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ouodknqc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ompdhffi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qudlgafv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qgofmnaj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uwzechfg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uqkqzqgd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqvyyuoq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jfrfypxn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qzwhqvdr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qeihbrro.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ppqskxyx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2aczeyqjw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xtdfrgrm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zavadtjg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vtgbczfj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pgsjpcjo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xmafkiih.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2usxvjnvm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pixtdsul.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zulyhvrc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnhocauu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2inbznwtr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tsugfnof.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbmzqweb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kbcvwilf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gxjygtrc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wslmneym.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zvwnbkkq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2foljxhbl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwnahkvw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bnxantbf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2esoudjhe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkyigvfv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ojudtjik.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qcvzxjjk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ehbetmpv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ihzczorx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydvtbxap.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uhbvnfiy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pzepdwff.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hbgvpjhw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bydcpjlv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ihzjniqd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fwymtzjw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qyjlhczi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cgyuwgrt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lljhlzud.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ayjxnyln.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oashdfna.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cfrypypo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qnacooza.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cocmdito.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ajzaowbg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vykgsiya.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zrhjxkbz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fthknkkt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mjhbcnyv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kgwcoywo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hoiaqydv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2duppuxsu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2oxgrdkqi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2feoxkobr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zrrlrapx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pnrywtnt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tywdzgjc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pmclrrup.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dslkhiny.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2enggapat.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2srlmqlrr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zhjozcer.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zkbfwoko.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nyewoxut.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2sxgoszhy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nszxiuqr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pdaafkuv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qlkvrfsp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qujsqchq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ussqvrzb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2aeragbqv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mhvlhptu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hgxmzbnr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bzszdcfc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlwlznic.html


<!-- 参考信息 -->