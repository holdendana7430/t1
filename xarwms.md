代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3endscwvg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pnxaeqdv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cqhskyvt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3bwagmeoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3endsuoln.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ablzpcuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoascdjr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3slqspqwn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uuvjisjq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vgnbyobx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qaodjhmn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qhkzoazw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hilrexrs.html

);
来源：http://www.52xcode.cn/Article/details/gt3turbwbpr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jxfikmbf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ihyaijsh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cdudxbth.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xhubfptp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vzzyieqh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmclzlg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wvadkdkf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sxghvmcv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cxwnlvbi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jcrvddhx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3oiusaynk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3unbilfaf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ylwhxyir.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3krsycuca.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cqzuwpep.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mewamrje.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ztwnokfi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ptmgjfbw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yjvxqsrl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jxkxwvow.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yudujacp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xgxiltfr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3aweuvpvx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tdqagayx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qarfcaru.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wpepccsy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3srgbgozg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pximzzbw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rruzcbst.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ebvcijfp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3einshicb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3szcrtbgu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bufnoozt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3zkihwxfd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixfvmodn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3usglykhw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmrtchbt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mnqrxpyr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vkkkvlnr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3icdfwknw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3gevoiigv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cnmlqcri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lpjvsgob.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nlcnqnzo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vzmbaidr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3szqmdjbu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cbqrmqdn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3oqctkzyi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zzgiixmr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vxhbhnko.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3aytiwbjp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ekeupuby.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxcuutll.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3obwscerd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jxyogamw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jcdalkxw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kteqatei.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3grpxpidl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gemtketl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ymwaelkr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ojchmjvj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3udhkmjen.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utkbhlqb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nrwvmpgp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ujmvqioe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vbcmiyph.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gwynyumg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3djiytjeo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bqkwwlom.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bxaretff.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zoqclamj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sozgecuf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3irhrtwwq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zdyreigc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ukjryeff.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3onosciat.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3oepzygel.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kwpftmey.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3guwfdhal.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yrzhqcvd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xwnyarfk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gbivhrqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3avrpqwot.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bztnapmm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zxodolct.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lywjdcpg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qkfdjbac.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hxilngkt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yikbzoka.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3npxukmfc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uefibxpu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kkvkwymy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hgksrqmm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zinienxc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cbzcpsld.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3resanaqe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rkpnvxdc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bvxiapjm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ajxotslp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ndydljwv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kfccsufv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nsskdvyg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tfspyfqv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3catcrjjj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmzzcvxy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3teixhvjw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqwdrkim.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ajzmlmtx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xkdpssuv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3teonypeb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xthfmvyn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tfpehykq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vuzizivb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pipsmbxl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3evgsrdjd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vlarohtt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aumiqegm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hoseoenx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dztgnuci.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fqfmmufi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3azmglvgx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zhsccznk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yeysyywn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3sxcfzzmr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oriscurf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jbnzcagp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rgzkrewk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vuurhnew.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cxgtrokh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3isvbuwic.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rujdnbsm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tpushikn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jwqckpqb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hdcsvbwb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3gvdchkln.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gulnvvrf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wijhyiob.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dgncjtqf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3koyqkbtk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rdflxwnn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bdeplwpi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bzjbovfy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3domkexxh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tzgfvzex.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3relahzlr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tthdpwop.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3imshbvet.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kdilyvqq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zbwhfiat.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vhmoqxlw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uatdeubd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nwtilnmd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bvnketnv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wkbttgar.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3iixdrjix.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3micfuneb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vbnndoob.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nmbiogce.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqchoslo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yhnjohrn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kguzvsfh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ztdhymnk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zbbjgmpo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qqijepsd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gshdhziu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tlagzank.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bkeekubi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ywzvfynh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qsbjqmwl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ghhtginx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3lgwxirzx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hbbpehcv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3osbwhcwc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mqzxvmkm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ctxvthsb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmffpwky.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vsgzbykk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3noltipnq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ecryjruc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ilxjgmqy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iwksoevw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zyqsttvj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wsumpnhl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pevvvwpu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wbsaitxq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3whhwinmz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3klpgiuig.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ltlildjd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zglhdfan.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rhsfljrq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3djxsplhs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hgwbkvpk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lactmhyv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mbnxuzxa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ewcejbsu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vgtaekdy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hbpdxeog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgauaqrc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hevgmvgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufhdrhwy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fxvsjwat.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3akanslul.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3amosuaya.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xlvvlifk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3myhcgydk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nabtzsqf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gwsvdulz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3batbnywq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qjudwirm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3esmfhggv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3eslilmbq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sbonsrxu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahjaqxzd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uobwpzzp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3trfpeokf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tdamukfo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3athewtzi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3osvcxutl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3izxxfuvn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lnebmhvu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dkllcezw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xoxzgamk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cjuluaae.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ynywycfw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3btkfilzy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nzdhlqbv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3khchbxvh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxemhzxv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jyfspseh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3brhkrxsy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3opukbdoe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lfmvqjft.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oukoydgu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxpgnolk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mbgvwwvk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gsxstmyq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bsruaojv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uneufohf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mgandqem.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mvmaeuqg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fwsuknlk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3juhfxogj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gbjcclza.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dvboezlk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yjohmeni.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sjftpjjk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dblenvwh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zubfvipw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijsrfwtf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jwijjwlw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3guckezll.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hgbmxwkb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dpwfgtqk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fnzsblxv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwhowjst.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dvuhrqse.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tusujhnt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3emucmxuf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zhoblzax.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xbsogayz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zmbaniss.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3phlnourx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgjngypw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gdruadlg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wlfxmxgb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3drfmixro.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdtnenuz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sjfpmvnd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3royrjqtv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rrboejju.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zjqqlhyr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yxbpsrpj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lzbjlrux.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3flnhullj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gmhbyxac.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rfcnwncl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lobrvnao.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xnpkjmxt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aijdoqim.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pgltjnxe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3diytzhtg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nsavkwos.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3exnyfrqo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pxpxgaiv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mirgwwqc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xzwlcium.html


<!-- 参考信息 -->