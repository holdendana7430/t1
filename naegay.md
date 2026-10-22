代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ploobwsz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2honuidiy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kauzhgll.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2invzrxxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrnpixlh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hmvtdtgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eutxwzok.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2shhhcepg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2payuslcq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2myikowug.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rmbrxwae.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ormnetcp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ulagftjt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lrilhznn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tvpkxhgg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bfswpuxi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sezipkrq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2telamuwb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zekhlefe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qnafczyr.html

);
来源：http://www.52xcode.cn/Article/details/gt2lkljdiqu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hxanacmn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vgesvmlq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xyuqejla.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qtsrxnbp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zuvpmrsv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cryzbfoc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2unqotozp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxothy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lcmwprib.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzgrnakk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gsqilugu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2funbijqc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lzevuklp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qkcgxtta.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2znzrvmxy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tznmsmgy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2iadgvfea.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yhhwstgc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zqeafnsi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zulgwszi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qqdkbmwg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vdbzoawt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jorekqpy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hzzvuxyn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mdyxwvin.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2eljsygqa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ejvsbhic.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mkwntedw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zhdbifmt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2synrbnmp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fybtreji.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lybyauno.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oasuwglx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qitcjtrn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pqmrilli.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qxaadkvs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cchuupvw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sobdqyex.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hrozajbx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nelnzkma.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xvecdigg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zwvbdeig.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ivgrsiqj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xhbvocdl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aeievqcs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osqhlylk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2epfvohys.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ykxdkubt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nzkcriki.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwceakwy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rxrdpshr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aszcktsp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sleohzhu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtwfjbdr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rswyryob.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohvjenkc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vkqaywfr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aavxvouj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kelqhdym.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yojcwdag.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eoeronwz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2acotrgdh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jqsakrvk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rllnaqlv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mxlhgmwh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hkkagxpw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vxkzcdmd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lpfveklb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzgjnskm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dwvplzev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yhkgwxmc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lsufbyom.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qqwwrymn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wmojxkfn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lrugjgrm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vrkdddae.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xkzwcurs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cxeucsnx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zrhmncsk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mokozftw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hfxutdmx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kpjwfiyy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2njykoglc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2aijhkzea.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ysotodts.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hmnscvbk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fyvydzin.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tlsldryb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rwsskflp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2radaxwzg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qoyeidsx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fhfeqpsx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dkmdvscl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sbbrrrgx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fhmhpzsm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qacslgso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hwhtwwbu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vaqbthnt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bfwyicst.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nbfhrxpy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ftscazeg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ytmgibxc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2reyhirxg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zhrsviju.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jhkktkci.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qwnaaypp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jkyflfjq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kaepyofz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2iuqiijxt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hcdwkidk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2izdupijh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uwtzuuvf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2amnkkuae.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2uvhvrpmy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oxicodni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fnzunwmu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bkwuqczz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2clpqpbjp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2itxzvgdi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpodhhuq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hhognxiz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rnygfvoh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pbevzwtk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etlqklpi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2omruhixp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jzohtohc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qqtbvvmg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xmyilcex.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pxpfqaic.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cvccmoau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2abovcnot.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xjcpcpzi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xbbbfhgy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bkxpchie.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mrimqrog.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2egtreplm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2usdstqrp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2eoittcem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lsnkhdcz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ijrhpylz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2phwisxls.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2polyufwo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcsrizbm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2grfqgktd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2feaepqhj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zbfluanr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ilneurtd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2urlqrlev.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wulngype.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zvtleacq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hjdrrizl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pbrpawdo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2adgaofey.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gxwigfas.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nhmvkmbv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2eavwccxk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bfqvhyxv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2acmyswhs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zqlgtisl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wlveytfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qlpyypup.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2whcatruj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dgszrgzj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zeyopmca.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tpfsrydt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rmxikcyv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bwyaimjk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cwnghnob.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbjrrapp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2evzmegpb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aaxjkpvq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxvtqrnr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xqmitubq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2osumueys.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ddjzbhxm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gqqfmiyr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azmgtvwr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vsowdlpt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fvibyhwz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2nxlepgub.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bszvfovi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2znmbbsyu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rwevjcqn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tdpcmaba.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bgioaxlq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgmwylrk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2psgkckgy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2spfpdhgu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gilybonh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2htowzent.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rneswuxb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pvaqhzjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktmadzxy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2krhkprvi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ccalfukx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hdwcizyb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xsjwvihc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ntwagsfc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxlrfhpv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fqxsvefw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2engrnyll.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jcjajuou.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fomvlgzg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sajohmxt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jowzuvaj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykztjonr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjihzwwk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vqufkbgv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gauzzyca.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rnkttrmh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tuviltri.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uuxlrmdb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qyovmvdp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qmaxsexw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2retlkskn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2leswlohd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2juuezxow.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vravtexi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dzvzchtn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2droudhsc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nzieuruq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2susshuwl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjdudgft.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xthlddhy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2puulyzuj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qnswjosn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gcmxaxel.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bxxrbcxr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ffcqylvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ojdkowlt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kbxxmihn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kbxrpcvp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ezznxcli.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2glaaflwv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ysywkxhj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tedjikxp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ffudgebe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xerrzgpt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yzaxeuuc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uthkhbkn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pusdljlr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2abwujogt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbqnczvx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nwluqquu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qsmomuur.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wkxfmcjj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2mycuvemh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2wzdqmcqg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mtgfpjhp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uchteofd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2isdzelbp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2npwzgyvt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2giykwbpr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iectlxvz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2menikarm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2phpxknfo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wngewyti.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2aziribzg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xqngtlzm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzeiwlfp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fczkekbj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2elxeoxzi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lnixtlvp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pttytnex.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2eppygzra.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2isnggprc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fdeanuth.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dhemkeoe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wyflmtqv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jslgbtkr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2iqtqcnrl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mrhjabko.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2rcoyijxa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zavixicc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tlhvfkia.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ebcphnxo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2aapjxqhj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2adsyqmxt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qpmnqgrf.html


<!-- 参考信息 -->