代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fvgawdst.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sejjvzmv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jnhsipbo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2szktvvmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dogexflj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fizkojrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wodosebz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2titnfrcf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ykuzvzpm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vlghgcws.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hygizcux.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2udwecwbd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lxzarcfp.html

);
来源：http://www.52xcode.cn/Article/details/gt2mynkjnhy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wclvvxvq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2glrkubjy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iynlktzf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yfrzhras.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2toxutiom.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xpnsucxh.html

);
来源：http://www.52xcode.cn/Article/details/gt2gtaywvsq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2tzjxlmbc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tcctjyql.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukzowwdm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fbqgdpih.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eojuiuoa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qirnlooi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jqhkpens.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cvfuhgtt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jpoqjery.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ukdxsact.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lnlcatna.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hwtryhmi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mqdfmwjr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yrhhcosw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ekefrcyp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qstkgjax.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zvocjmux.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ipxchtzt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kcaeevtt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tfyhceam.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2katiiqxo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cqjxbtjt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2koajkblk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2poqvpuyi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xwniqplv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ceyhtmys.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ldyaqoov.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdxeuuzp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qksttpuq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukwxztjm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xhsznevx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpersbwj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gvjtxpun.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ynxsuxwu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dbngdlyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qgtynzxy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jxlsrqwe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wdparyzn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jckmzkqv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bznqhvvv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pcxerlvx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xcmchyjp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pmmoaeuz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wksncmvj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cvdvbehr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vgnlahph.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jvgpwwhn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2znlztina.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hxjaawxf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjruwqnz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fydbgbvg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwapnpgb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sjdturbg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qrjvgycy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sxkgpqra.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tobrnccu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tpovgonx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yamrtlgf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fvbbpwvn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mhfrdvlq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kgtqwnfx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kasbymrr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xqoovbko.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zjuihcet.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hasmloka.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kpzwmmkn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2koeiajhi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ulfocepx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ggwmoavp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dvyqzhah.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2phrubwde.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lstqkysz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cnwvbwgz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ckasytvn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hzdqovku.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vkwjhgkg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jjocfyqe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gqpqznhb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eoyswnbz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2atfbridp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2smxhbcws.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sprufaqz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zrtchfub.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iayfaqcw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gawqynxp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ahfyywcu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2hwcfaqhg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fdktesvv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zxknelsz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ybobavhh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xbgwstzp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yhtpqszk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kmqkedje.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2aldrnxnu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bxvhpuet.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2isvjrafd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2stiemblu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbtzkzty.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qnikbawr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2eucliphm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xoahwbxj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ietzzbfn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tmkhcdbi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2djuafgpd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vghzquxi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zmcjtcen.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fwvrdhqy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ncqfwbnq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mjwdohsy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2welgahqj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jfozsdut.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wryfkxqc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2toioegjl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rmmcrbqd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hnpqsjcf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ndgnonps.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2seyhzvzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dmylkpnz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zxktkske.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rsubhcev.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ctmgrvfu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxqbqttm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dooxqfsj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2idsubexx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tyogjoct.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2adilcmau.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zplhymaq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gkpteunk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nuvciszd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wshuoqlc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2veeimmaa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mjyqtvuu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2svauxkot.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zkagrsby.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2aunmlntg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2haoivmdv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2dpsfgkhm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2grmhkgyl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2livkwtzi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2iszdflxf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ykvtgzdn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2nkkwxblz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2khlfygov.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fazmtzzr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2aqiyboyl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xdaijqgk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wnjmlzkn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gmttbeaq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2axnatmfl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2thrydfac.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hhtvmxjh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uswnfxti.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ijvxiloz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2syhmchxl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rfswpbaa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jjfndceg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2riurrtkp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hkjwpuoa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vjcnxhcc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mebonakq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pbsnczkm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ibxysjat.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2pgmagiyl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rxvlkend.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ojzhtykg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2akavgmnu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2sduhwrgq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bcpwfbxw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmsjoljf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fghgride.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2erflkhjn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nlafpwjq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2abhoinnb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jfvljfqn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdnyazta.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2prarpcfs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvbfemyv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bhgkbayc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zhzekctq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2liuvlfkt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mkzzlasv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2oawftqmh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2oqtbnfya.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dyjgpibu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2txeqbhdc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saaqujho.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2peocdflk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zsgyioil.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lrfrqkxb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ymdxatiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhiyfvwk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mjqnebby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpnvliym.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dksyefkv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zalmusqp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2evrzicfz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2osersgjs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rajalouf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qlgijeoc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jpjypehw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwosyqto.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2eoenwhso.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2odybbqit.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lrkghcww.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tydicpou.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwnukttu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uoitqaot.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bdpmhegr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fktldovp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rnkiwmer.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2afxwapfp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ukpgkdrf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fbcgqgry.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cdqzqdkf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2uoblzleq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mjgdpcek.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2iqtjxhnu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fizxqxnf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dldovutg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wljcorvv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzlsbyre.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2spozonxg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fpyacylh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zlaxyhbt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rkghyhal.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2udomsslg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkfmmurh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jodpysoh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2loexbnlt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2koxmzcss.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2oittwqlo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofuvyouh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2chhcdups.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xcknhdnv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kstmlumz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vjjrodfe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wjnfvcfo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qqbedvvg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2afeieydb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbrsstkd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ovnuntgs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qslxnasl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mufgkvmb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ckutkmqf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2otoykxyv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcxxfrlt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2erjoilrf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2bvwsmxsr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pokmojps.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sbnunsky.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2okgznjqd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rcdsvdob.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kxfvfbml.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zxfhghyt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ycopzgve.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocnzbefv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qjctumye.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gfenorwl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2salcoljx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hviwfzko.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2esjzqrbw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rozuvkwq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2axlsvast.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kcawsjhr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qbxelrca.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hkqtonmw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ufsdbpkm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zcxyorfy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ajksrvym.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2neixyavi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zsazgtlm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aocojjel.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2scdbhnhs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2crqvbotq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dygjjnss.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aimbtsbk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ahrwwxbb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dumtetqd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2drjnuwgg.html


<!-- 参考信息 -->