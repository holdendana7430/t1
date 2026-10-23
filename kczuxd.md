代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3blmbxcxh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3edzpxqfh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vammrsac.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lzfbhqwx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lwylckcf.html

);
来源：http://www.52xcode.cn/Article/details/gt3iapfzswb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dehjvzkp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3eepvodkm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kyywrpqh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ochirlwj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uikzbxtb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qylgtobg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kzugrkol.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3csabykol.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oghuosra.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3appzrjyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fiomklrr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zwealzyt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mnrtifrw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ncfofhcu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qwolgiom.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gsbdfsxf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3stodkwlo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wexyikxp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gdfqonof.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eoxfqtqz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xpmmdqvp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ocjlxvor.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3liodjlzf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3brzyyxzq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3efcxnsdl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qveirvyn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ggufssxy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ddzzhwcx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3srlglnjv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qizbaane.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3uhukkwbw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ghsteyxi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ygcwtemy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vvmxhjds.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbaqebrk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qsbnbvho.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mzxaskrt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3soynosop.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tqbqbvgy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ofeihkqg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3gaobdgzs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cpmphbli.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kiosxzcl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ubnjoktj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dxnionpg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wzkuprot.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ipkwuifr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qjadkpgu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cuknbsoo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3gdohuheb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ngedldmz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ghvibeii.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfkcsaic.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3quseadid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cqnsqbda.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xdyhrkaq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jyzzoago.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3eyzbbkhc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3txkiatmq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nxuuaofq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pqmbaxht.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3skmyixjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgbbctna.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lfaglrhj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ihrzhgzu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ryzskyij.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uuwzkeul.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iykirapo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qqomdrkh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3rcahqevd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hojbzccr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3umkrbbbm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jimkenrw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mmwgxeoy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jlgvsazc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3atotqpxy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmhjhlxq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ibpgigco.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vfpfzmzh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ibnfizoo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wejkcfyz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3facprohc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ywzdxrmf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uzyvmsdr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jvjbbnam.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zezsjmer.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wilxhrnx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cuigotbh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xubxqhfl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ehoulhcy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3trhgwzqo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vzxlfmmn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lkczrbfs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3saczfgyr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nhurxbsb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qpcrseyf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iqkasirq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kvrvkwsg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wwtwiaqw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3obajcgom.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lnpyufsj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oldigrlp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nvtwoshk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nwkwpvjb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ptorvfev.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fagdycaq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qvodsjub.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wgeicolc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fyypckuv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pcbivdfw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vcfreoeo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3alboqesn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qovnyics.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tkklvdzh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bkmdticc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ndvtahdy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3azejtdyc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jgtqbhbh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3magcovqs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3joghdrqg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uvlnyrae.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wadsmlhx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vwsuhfbp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mzbphuuf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3duqxumux.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bxdchznn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aitrtmke.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cxrfumjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3trlvgvmm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fradvtkk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sijxntlw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3oltpldvv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nevsqesd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mcalmota.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3npbyenor.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gmvknpuh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ssebutcy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3apelrzyi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xmmnqnaq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ypkwepdu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pdklinwu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3stzpycws.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3isoddbnp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3oxmfqyje.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qtthwyhx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3guteetdc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nmyrvafh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dnuikkdf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cxvvdquj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3haowfuys.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qrwucaiw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wyzqfkjr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sfibbrcs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dcevzlnt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kuyuqifb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hoputobx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3uvmrceqv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vwuwbrpf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmvirvug.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3umkxqkkw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3iwzghqsm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nsjdihyr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3owvwmjho.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czyrujgv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ywgphnwh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nljsvkeq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dlmihray.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3adzhhuht.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3brxxfchr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yuypdolw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hvfkyhcy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3omnrrxdv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3epcebuky.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3moftvrtz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3inlutipq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agoqhayv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3emcwhwpz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lagnwmtj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lynpqvgo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3httsfqrk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3scyudlhz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3csovpwvi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vgylemnq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nynwarsi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jcnuwbhw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oxabaxvs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sroxpwsi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3prbvdogw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wwsxzgqg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tbwprjqn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3kaspkbki.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ycneoqwy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpwebcpb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wggbyzeg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ppkhirjq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dnzqleez.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cyxtmgiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shgwtyzw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cqvtsbsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfrbqyxw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bfivydim.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yjlouzbh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wtpgsamz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kytczrvg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xwxedccv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tffdhugb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mvpqgvxq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3engzkvsc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zshklcbt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxiust.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fnxnawni.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ncagetxr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rmpvokan.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3siaalkuk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ntmhkwcc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ssjoqwev.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uihlmkvr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bzntfazl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cegmnwfu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oggsfuoe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wkxybkoq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hcdmwrtk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tjxqpwmx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ogbebtko.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lsuawpll.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tregaivh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yspkkwsi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xxcwzxap.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hkcyxvfx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qsfoeemt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nncauffj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ohiznkuz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghhifcxw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgbhwwck.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jjztpstz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vozzzbim.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xpvcuelf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3txkvhnwd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yznnphup.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzbrayqh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kdzkyrbb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gykstfuk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifysanti.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pghisgnu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3sazphewr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rkswreld.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ewwjtocv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ekammmwe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ummpeitm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jabrjfic.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fzdmaevd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3abpfiuab.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvuihbwu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oslmkset.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kjfovlam.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3trgycmmk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wynnifup.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3onkxsaps.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3krcbhcno.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dpmvvpan.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3legafjqi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jzgirkoc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwvtabil.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3objhniwq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3stauxnyd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jukdwwtt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mhltkowb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wdkziqnp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fhjbnsja.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3udadnbug.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3motwodot.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fyjyzlqz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cmgjpqlr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lnzyrmcy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dckwblhm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nukexmeu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3eelofdor.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdvynnff.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuusdjyv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rflswpye.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jtzjjtzy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bvemklph.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vbogpvjj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ewjaphol.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kbgdzznc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zozhrsem.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tytvvras.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dzmbitix.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3coayvtdp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pymtisxf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jmxkznib.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3prunprum.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lvnmaomr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dxlkgtda.html


<!-- 参考信息 -->