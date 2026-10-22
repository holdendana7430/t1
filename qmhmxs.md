代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pdaqeduo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dbvhnksa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vptgpocs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2msxqnozw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zltpnhfs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xxgvpihs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcylkfit.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hyqjudte.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pmohduwt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mmklwyzt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bvkmokrm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ihurvzxb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lmhwecef.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kumeyktf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zrxzjjwb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vomfakdw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dbdgbynm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mxpaohlk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yomimxzi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2urkfvpdf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2udujtofp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fkmnykck.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zpneqpma.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2twwjrsaw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ufwparzr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yrmvypbi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2safufepr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rfuhgrlg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dwngvoie.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yvpkaauv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hfornkzg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2okjwqjfl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oadqzbxa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xmrczmtz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rksinhbb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2peqfidyg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gymrfkoe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bbpckyhh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2adoyccoq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ykpgkdhg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rgmbphoi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ghyfczvz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pvnbiukl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eidvensm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2evqylqlx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2yqdlcmcx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bqdwuuhy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uapexmyk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gyvehkvn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bixhyshg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brcneoki.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2saijdpsc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zxuggzcg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2rlknrtmz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bbougksb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uhuypnag.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gucnpmfw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ckkcvqwa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lyishbpe.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jtvazzso.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xkhwupra.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jqgolnhr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2cbukbkwa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cctwzcvi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wcsmifav.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sjypyfpi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxaehbyn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2reozhzpp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gnzexhea.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qhnsxqvs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjuxvwfj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pfqvbfti.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqbusdtl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wnspauau.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fcqzmfru.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vvdqbdhx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mbnnmvso.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bpfzjilu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yyklzdhe.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nflmmkoz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2sqwwhleh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vstcmywy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2azjumbtl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tsedjmnj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2eutikhbh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ewmflyon.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2pnlzkbnc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2uvixyyhk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ladwlgyb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2loqmpfje.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2awkwuipd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2batnshjn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qnhfdzrn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2knkqdjrl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dxmhksvq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fptqilgr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pvknmpem.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ieynktyh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vgfrlrty.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pnaaczkm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ftswuwhd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oommgdve.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rlpoythg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpliozmp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vgjwrcdd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ivcjutuo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fklzrgma.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vyhmltis.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2frzhzweq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vminvgtc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dsdzcfvb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ufaxpksi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jnxonxjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ypnvoajj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2wnekiqkj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2maxameqc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qnglunad.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lqhkpxpr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2grrfduoh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hrkhqkrj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lzoqejya.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hizconyx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zdigwxbu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wgperogo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vxmlgvhe.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kqonngeq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2waxokuih.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rclpcmkw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxoukxny.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cddadprv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2linrguqi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kcxirpoh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ycowvvqk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jtrsgkxt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vzipuxov.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hebcmhnb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2llhmgdfs.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rpqlroku.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hjvmjuwd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2pjcxufkm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pyorinbr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sfydvecw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xhfegyco.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qdoyydst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vuynjmqv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qtspqtot.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fiflpybr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kibklnqa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2yzbidbsx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zdbazrpl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jzejfdbu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cebpkuer.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2flxhumjq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kawthmpo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wfnnyyfn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zbwrflbg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gummgsfd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cgikrxqx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2phcxednh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hehorrpw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jbwhqhdg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ygduftxx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ulueupwc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rgweihrf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tqfmzris.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tkamzwiv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2asiisrsy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2obdvnmsb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zjnhghiq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2disjzaqh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mdobswgr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2elqivagk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phrdztmb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dqaooinc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vszjhxoj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ualittxs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rcceozbv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qmcsojvq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ooumtdrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vwpofhsf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yqzfmtht.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2psnrpqcc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uwgzbylg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vxcnysgn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ufhskeva.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lmtzagbj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2akoxwbxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zlkcfzjx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dpqvkoyk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2glrmeowx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hsnmytaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eymumyte.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cvkburxw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fgalbvmo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqhdtkjz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcrgecsa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lsbtamkl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rzcakcjw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wchgtmfm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hzfjafex.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2axzykhak.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bvfqtzep.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pbshlulh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zoycmvox.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nyixdwih.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hpugeaqw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gurftrij.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qqyfcyml.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hjqllimh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ccgedcut.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bhykivlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rroetybt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gjmhedan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdzzlhny.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hecmtqwx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xjoikdkw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zgmtljsf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zqpurwhm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lrktltud.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lddmkash.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mtxonkrm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mjhxdodr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2stuvezhb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uwwkfyzy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zpqszxnh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rlicmjdk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xrpqpdve.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2eomcrhru.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bnmgmyqn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vhdpjebq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylizbraa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nfnfenuh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ytjkpqct.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sqmerses.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eipqsqdd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2oxqtrlck.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zvfjpbkh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2toirxttp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dhmuailp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hgmepmnp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mmgmoebj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtizeawl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2anidhjtq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2orgdkksd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfqvydje.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rejzyfll.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjmbyngc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdybhhwz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wmmwfbrl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2cetjiage.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2svmeokbc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xqccorqk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yzdupazt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vgkbtghb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nrpdkadl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mjamehcu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lfccbxgk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dbsvhlsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ojhcqjtg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vhgoqnif.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uifhvjqc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ktxwljgv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fzrrfpjb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wwihbmpg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lvnmzqjt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwtsjvve.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqutlfpo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vurnlqwa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lwbeigih.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ypwlgodv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gaztvukg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2umvdsgdy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mipmaxpb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hzlgsgyf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mmqkxzbw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdmymegh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2imueximp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cbfxevqd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2aqazubib.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wlwinanz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2coketlkb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2onxysxth.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdadjte.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qkrahqao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2knwzdlmv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ugmmxjcv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ylpntzdw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tqjeibug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mplvywxp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tshaulbn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kvyapnjb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2camcdilx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipytbnqd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sfgdtajc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lnzmaytq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vdpdeoep.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lchxmooz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2heqvhfbu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qusyfsti.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pcatcxkk.html


<!-- 参考信息 -->