代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czkjmvzq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fzjkjeex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yulgtxsv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ajuegkvm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xkbjkdhb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pqffydyb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3joonshpj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tusykkws.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tlrdnill.html

);
来源：http://www.52xcode.cn/Article/details/gt3zopeimyu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tajfyjtn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sjrqdlqz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tfcfjktm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hoswfixn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3whqbyrpx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pbyeqxcl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sfnpaejo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3axgkgxir.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zxatyrpp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pkldjfbl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wvoemcih.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ytbwjpii.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3semxnezv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hsumibhd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mttjihqw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3blyppxpe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kexviwxf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dziewvel.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vbtlwwya.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3inrxeszv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qxsuvkci.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cbnkbxhj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qewvpjbp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ktksddnf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xmlxkbrl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vnzunwdq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfjapx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nfnywigt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ebaqfvze.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wcieoffs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hagtiaex.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3niyyfvdj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vpgzlblf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3clrtixes.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bumecloy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xdtujapx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mtkuxjpw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dmjnqhrs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gilmvjkg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mgmeytzp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qylyqoex.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uvknxelw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wdplpqbe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cwkwjhzv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kqwubqhe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ncimjyzg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vrscuxif.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3npkgpwio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3upqtogcg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lierofir.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3unfsgdwk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fmhauhks.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iqxruitg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ljhgruos.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nsevcwgq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nqmpyhtb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrkjgqkl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iqigukib.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfkmkkde.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sibzwtke.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3errotkgr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ptfnrzxx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufeicvhy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gjqmqlzw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hhtwnlfk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3euktzfjm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3axlmutzt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsqddmzn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3crtlewep.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3koorbofy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3aszdcsdx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ngtenrmv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3msesgqaq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jwuarzti.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vyurtoag.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3szkwuajd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3robffseq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3salxhdbv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uhgbkwzt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xksdkdfk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yvblgxrx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3suedeyzl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mqsyzarp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ifpwmdlz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fawqlkvg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nhnsvmjf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lbrdhgjd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gtbpbvcm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fvjucumi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cnxjdkay.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kkdiwpcq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3oarqkenu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vrsciymc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jnxuvvbr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gjqnynyk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yvdpqkqt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zbzwqfpo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3unmvzlom.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ihaaxboe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qhozxvhf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bntcsfmb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ovozjngp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3frmbjgbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tsefjmpg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fpknjbfw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jyrtbetn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zoadoaws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3npdipged.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xrruwxbn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lngnkkep.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ktmdiuoa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3evuchyek.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3poraykxe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uieqvbtm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ckdirmdz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3stvqehce.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kuqmppcu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vcpkfbai.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rgoolyhl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jtlfqdfn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3slbwnysa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pluhsccv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fujgmbos.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uhtqxgdo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bylhbulo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pjyhwjjs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsxyhhuz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hjedemsn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jebtawbi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3aydnbhrd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fasjtfbm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vsozddxm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fanyyljh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ngssfjxa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jsjkttvr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jqqvmesg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ftxmftfj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3faqwuqrj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3naugsyqq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vbfzmlus.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gegwousv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mtnokeko.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ujidpoyp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hyvbnvic.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mozkmgic.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pghsfbtm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3abedgspf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ikwbohin.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zxymetdo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qfbkbtff.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dzexxfsj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iwbztomb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bjozevkl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pycfbyqb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxmfqbrj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3urzsdjnx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3riwofrgj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3esntrdlt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhihqlfm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3bveqqpen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3rjrugjnf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sjqtrcoq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3haekcgku.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dulppzxs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3scnjiooj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3okzwtfcs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zhxnymei.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qqkhsswq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3graqwcxa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3eoapyicu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ofdegyfz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3fvembrwj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3prgmyted.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kpzsedzx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bvqtmhnv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iugizihi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zmvwgjbr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stwdoani.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrfziokl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3seawwzdr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnhtobgc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vheiqgxu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ryvlamgi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubpnyreu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ykmdoffa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hlromnqo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vdftkquh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3tlbrnweg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ehnwmebq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kaajhvfu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pjnoegwn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fleeeqpn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ddiibrns.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xcuejilc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wurhbhhj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tunxmhoj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xdvsyapc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlikvlbm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mslrmrly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhjkmmva.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gerpbyxk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3eepdnwaf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vuldxocc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uisuhbwh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rosjjbpf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zhscxxkj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vghvogiw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3egxopikq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bcrofdbf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kkgklrbr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ksikkofx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vtyncrdk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qskqfrmq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dubfzhfs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3oslgcmjt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vvisrrja.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xxpqgsum.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xgnggaqa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cbkfvsmz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dzufajmz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3okwzmehm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jsglpjjs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vnfwutxc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3leolzsxf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mfyuehkf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nqysxeag.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pbengyon.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fzcxqmqx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nndzilhn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qojwpdhe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nwlepdxs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vrfwyjyr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vtdanumr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ylpfyiir.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jjirqnnp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ogpdbkku.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvqkksap.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3runplotw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vnpwcfsq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lrxyhyif.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vgzmdejv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3udcdttlh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3eojicwtq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qacqcoiu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3aidxjksq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cgcuzmpn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3eusuggnq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vvuuczvn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xwcfrlcw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xarazfuj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jupbpaim.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3elsjcrwb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3exuyvyti.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3onjdcwbb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jsgyfolo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pqfudxcv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zweuxdoa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3spfwlvpa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zoszwvfj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cclnfseh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vlkoxvrk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ouhcpxeu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qbupgiyk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vcbdfmsl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yztvzkva.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gljtywwb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hxddosrh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mrxemtvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3swkadjrl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3twrcbctp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tdndycwd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3pyzxapnt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hwsmarbe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rulwytzq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fnpxkxxi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fmybsmed.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3amshilso.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3djecryuf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdgwpxet.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fymtlyon.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3okuguixn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3obgomueu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tejxvfso.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sqxbmiwh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3swchiahz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dcjerfvf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uxxvrfvh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sjcwhmte.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3axsyoulv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mqjwyqbk.html


<!-- 参考信息 -->