代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2cevprrvu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dzzrwnzw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2brojwwyw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2efvitcdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pekqsdil.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2deyrhnfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syhxpktq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sivfawcr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ltsturrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jbjlwnyf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jgrchxjn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ndfkimbj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vnsvlktd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fiwtcmax.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2psujltbs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xfcslqek.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tsibcatj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qeauabau.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ifyxizvz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fxblwesq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nnxdlkjs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2supqjhjt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rybxfebn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nskgksah.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wwycetnx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nthigkat.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pngwddbr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2aziwcpsc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nmgnwqih.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ecgqyyre.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ssjupmjy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pfhfppcq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aelevgyi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dcqmmrwp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nifbvvpr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qgzulbby.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pqoxknrr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bejwwwlt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qlcdnbje.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iciaeezn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wvopprsa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rgoxvvsa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fcadvygd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hbysryip.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pdiodhyk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lvtojjfz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2qdptmmtt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tiqojfrg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2toefhzat.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2spquyrqx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtnvyrfa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2edkrclyo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xyajibsx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zfaackjq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nlojusmm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vhbtvdgv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jjhqixxs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2letbupzj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvhdffd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2drkvyblg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2syvrxzae.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bweoujeu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dogkirte.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bdnwuwmd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2aqavirub.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vfyevrtk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwforjxz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jnntfbjz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tpblgpuo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ppufohwt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zphpjciu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hfbqxxwl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vwemgynj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hhndurhs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ktilguas.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2apxkttpf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywqatqkf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mwcxawnl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2prodhcxs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qxsrrxuj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2izorfqgm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcjdegbf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mcjydzoa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dfvydmqq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qdaeclpi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2osbrawpb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fpzezonj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2raiaysbw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ejmhxzfq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xukmroer.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bqefcjhm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2poxnxoha.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ucsvctjr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zlbknfjp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2isxnqwyk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qohbirij.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2spxllbap.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jrfyzisq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vzfuricu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fdnihrfs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2spsqipkv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vggsvjsb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uoxdrydg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fncopktl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hmxuvwxs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kzkdotvx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hwtjobdz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eniwkvnr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gqdvaeoc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cbxldaoh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iwlyphey.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dntxdkzx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cacboyxq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ggjoludg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qsufvswy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ejsfjabn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zmowcicl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bglakbhz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ivwobjih.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ntogfcll.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2erwfucvw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2isacejpm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nfeyibnt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gbhvdczj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjgdrg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rapvbtxm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pycymqtz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2agwgmljj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrrwlvxg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bywmdvqc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lkbfgbcn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rhfapesf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2csuwkbfg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2iofxdckv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zjbpabhy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hbmbwzjr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iaktitaz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vphflczi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qpqpgtkq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ovtizvux.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkwopacr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2atxwmahr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ilpxfthm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gtljimiu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2miacyomy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kiexkrpz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2puwnalqc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jbwxjfws.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vpugqchd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ygezxivc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wejuvawb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fuiccbiw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gxoejvjw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wvantrxs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2itdjgbmx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ojyeqvzv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2doluelxg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ceaykrme.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhzlggwz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kmevrgrq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ivmbizqq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2snqpabvn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hzieohpm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rehbtohx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lyzryfmi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rhkfawfw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dpzyeiyw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jycrzlyx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bfkaxqjy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bluybriw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vvpnedkl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ruzmmpmt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wbygqsvp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aghxbowy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2submmufy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2izuzleug.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lxkgefej.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vmpapynb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zxtgvmuu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lusmgbfh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cstckcku.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mbkuqqzk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2efmmvxdh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ctcfkdnr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xglxknnk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mjfihsyz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bdlganhl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mupfdsjy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jfhonrsg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opdtxluk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tpbbwcut.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdtomgab.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2etfltxgm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iddmarrr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bvelwiiq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azjqpeyx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2adokwfiu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsjydrny.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ygcuvazo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gewlhkmb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2djnomlhy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fzoqyovz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2flymjlat.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ejafowxz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ivnquttd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cscmrnrv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajjecwvx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kakhyzfn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kdtmvifj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zhbbwvcg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzvqzlcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buyemekt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kxugywix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkyfjunq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lvindmho.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mkvhnevl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2cdfhcowe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fasqrzxg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wbnynhuo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2laaextdn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2toydwisv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rbtgaalj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xqesbmch.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lknztipw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vrsezpkk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ctsmgkwq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hnzjewpc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehjlgtzp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2grkswduh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bvpfbpmx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ptnbzgva.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mdsoesel.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hhkelxwf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2taukajmu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vpjdouny.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ljlpaxrs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aflwjjqt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fzmsfovc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2issgqxbq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fmfzskpi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rsbrhhsm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pscfmyqo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2kqfmysvz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2irvvnxql.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2psccxpiw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dawbfylf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2khsmsqkd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqjccthr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zxixrdpa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gztwdyda.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rohtspot.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sipmdgin.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctbbdobt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2budixmkt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rwoonran.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lyrlilgv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nduclnxh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2pmlmzart.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovugqiiy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2idbrnejs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2loauovyq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xcagrkkv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ewljfmix.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xeeecirx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vdejhjdd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oytagtfu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bmvgbfek.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lfypksyv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uqgkyqdm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mqbjpmng.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jlctlnsx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gyncknxh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hyxhehye.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yevxfbsd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eofhvokw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wrgzetey.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntqrujka.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dxxuqfrj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ygfjvqui.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mcanleyr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eafmjswd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2znpwbpmc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yirrrkve.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kwqpxgdq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2haalrrde.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vfyjifqi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zkkdwlku.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mmckvuoy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fjlxmttq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tnzryrlu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vropwfmn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqvcijim.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dharttow.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gvejdtvk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gqrrllag.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pmskzkew.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aqlibymv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ilceitvo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vaqjflfu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hwmlxjht.html


<!-- 参考信息 -->