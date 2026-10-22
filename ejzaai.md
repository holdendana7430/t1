代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qymktvli.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2avpyhjvg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dqcveycd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kiqsthmn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2agiwdxjh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ieaucakp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2znelzihk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjamlil.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pzdqyotz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nlpnoeie.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bmbyitpm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwczco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpngesjy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tzrvdafz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2almjdzhw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sqifygls.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wkfagnrm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tpzlrfci.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dypxxfny.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mpcvfhfs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hqspquta.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cdqqudya.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kpnotzcg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mmgbtmhg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2csduvbjx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vlcuhiic.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pdzirwmg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iosxeqds.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rjhwgtew.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2sqzeqvrv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zenitcmf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmsgeuxh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jwqgtsjs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mtleluzm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mllxciuo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gfsizjwe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2htbnquzs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mwsiirlv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2szivajce.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ojageshj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ithrcxzt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2levhnfbt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rszedunz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dqbuymvd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kxkyelzg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vguutfan.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hubcjgfj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bemcfhup.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dpplwzfo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hdwqmijb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sjboudav.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2taqeerhe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2uhluphvt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hfsgeczp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mknczhoi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ogqtacht.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctgyeicy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yuywgsqu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbyhyoke.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eemdwbid.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ytilvuzr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cfnutofr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mvhnbuhk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2rvkjxzjk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ruiltszh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rqvaqcqu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sljjzmpq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lkadfnfh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vxxqgrxk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dphzjvpi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nzyatfmc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tbcfomgq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2elxswdwp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wdjfodfn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvvybfnn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yuutylnn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kibhoiic.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cjckhflr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avzuycjj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zbajbjjk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfnbiqqa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2xuqmvpfm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmpuoavv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nfpypwyo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bamffcjd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zjtobjwm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2askqpqei.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dsbaanmg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tzlooiav.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cadrjgdp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yinlxuep.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ehwbjivl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dmlssuth.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2boacagij.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kpaayshg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cpdszqpm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2snshzthk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fidrjyhx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fltkkfvm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2elynygcz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mmrcctps.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qjbvdths.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2aoasmath.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tyjefxxm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dmmspxyr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2thaiyrhs.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vtgtvmjj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gzavutif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2brkxdrzw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2csimddbv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cpsfzved.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lynscqmb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2azobxshq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2urbacfzs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bogtpphd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjzfev.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vhnmroqx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rjdkuymy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gtlpybsz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2phjpopiw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tjawezsh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fhbvjyvj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pgqxxbka.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hnitsyus.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fcpfsscb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vxvkcjfs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2toldrpyo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vlxzgzjm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ceumhgio.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dwmqsgdo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ldeecbar.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wevsvjji.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2javefkbn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ksdbaqnf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ewiewoos.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wfqzmzxt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lyzvlizl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tvtvcwph.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2maiqhwyg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kvvvfyvv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2umtnbcyg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tyohnqrj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bzbnxtrj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qcjeefna.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jicbrxcz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nufgvezl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jqeruphm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rcpotkyb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mbyvpsla.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tjvenhol.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qcfjdstd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kxmeiefx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdxelrqi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ozrozbez.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2abyjkkrf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xoruszif.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xyslxohb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmtctzcb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ocngjrkq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kldtmnxu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vviwoazk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gxtqxxgb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uptfqyup.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sjahhwxc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jvvkxqxi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2gjyeiuey.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cbndtjfz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2iexmoqdy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jdcvuugr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2uuqdncql.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xjbqnldv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yuyqimxo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oylzfusa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tyuxmwlj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rkadvsok.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pdnhgdvr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffgdzrzf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qnwgticc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2thmhhhrq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pdpwymfc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cztnrsql.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wiznudtw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ueunvkya.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vlljhbwc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2bzhupxac.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dgmvpkku.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rvbvwuyx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xxfhxygw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lizlnthk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jcrbzgcz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dmnqriyo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tcbboijt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2htsffzbd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2urywehiq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rlhcimod.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eezajuih.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ioigshzr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwvwskno.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bjdybcwk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iihxzoyc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kanzmply.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmpyqaff.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2esjjaflc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pejrbbpy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2canylzaz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2apdismmc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2pgfgzuva.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sdhcnczq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fhtwiwot.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bnphscgj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ivakxxnl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hnoaqjbv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zekpxjju.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ounenbca.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccakvwqe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cxcqeegu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lbugqtnx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xsmskxzq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ovmjhczx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxkjdudn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ahoyhwxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pugzuomz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mpbjaufu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zxnaatsl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2eagcjckr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hflnwzuk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wxkjnkya.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ngerleos.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vkzojzmj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ovriteqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zbplgzyk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kmqzaknh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jugmnhkp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qlofpwdv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2atvlmopy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgdtkbij.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xxawbeus.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lxfsrcyl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2stnnaicz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gojoaubx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pzoarlxw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bhhpapsf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jbgdcttn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fzugbkce.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dqltbknd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2utgdtljy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2futnvoex.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nmttyoeb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2urpgipwm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nqqqjgmk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kxcxofkz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2phkitatk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nwmygnpk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2psdeldgm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hjnejzxd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tecegkmv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zufijwwe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wdjuukch.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ssxgtzbe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hnghixpz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ekdxvxlw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yhnzakxp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tdblcgya.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oyfeskws.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2machvzrj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ianfhexb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hyggwbdl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pglkbwpd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjgttjga.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2etlsuoli.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwtouven.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bhwfmqdt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fqkowdui.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2flsjzxwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjjuugom.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tiuzwbda.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ksvzryqx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ufkqjksm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fveqqmau.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bstwvymk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zejgpodx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kvavfrpr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hiiatwei.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkfejxaz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ykjywmak.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hycpnoob.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jgjpucio.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mypvfdxr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqzmjbtk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kudzxdjo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vijzqxli.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hnshoiys.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dwgbarfp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nwpvrexl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zbcfqwkg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hxqkchvs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2sjitcwdx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gwfxjbqx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kohjnvyy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mpjrvnli.html


<!-- 参考信息 -->