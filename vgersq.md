代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exorsfgn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ggkzgbeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jodqinpa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wrwzwuei.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3prpwiezf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eazuvpjs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rqymkmjr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3sknsgqwb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lbmvwovn.html

);
来源：http://www.52xcode.cn/Article/details/gt3tueicfxt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ruzmoolf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hudkvshx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yzfmuoal.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wrwnconm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3afqigana.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cgbdhjse.html

);
来源：http://www.52xcode.cn/Article/details/gt3rxppbrqm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nrzheprm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gelbnqvv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cyzjjren.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lqoqygit.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bpordtcb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wqtoiudx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lakehwjk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dodmgvmu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3romuzbhg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jrvxzgzr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gnueabdz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xksdhzyj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vqlmalxs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fwhigsht.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3awmlryaj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3prnikvgy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lpsbyjxl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zrwajtvu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wcnjavcy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tzgbyxao.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yvlycdqk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mbvgvrss.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3foplsokm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ubfwithj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tlqfruxj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xshtghlj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3uykjnnrg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sclquywh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3utgiooal.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kljmditt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bwzieiyw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rviixnqg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3boyvotpc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ltomgxnq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nkuvqqxm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bseayfdg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ejumcjaf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkelstz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wpcnzkcq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dblzhcyc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mrelwdgn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3anhiyyky.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wtxtcjhr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3goskzxlt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qfnqiskh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nocoriov.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uvqpizeu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ldkalbrs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vnzhubqe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fqrmqzat.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rzvqhivx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbnobdfz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3brityayc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tnxytmoh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kkkevnsz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3snudypdr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dindelgf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kybiitct.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hmbkbzla.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3trytznln.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdhimn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bnznvtbj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vnmqyyyq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3txtosbcf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3khwsuuzx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cxjeyjbd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xdhfdiqf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3oetsrmiu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxrqtjnm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3klzadlyt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xsvlkskf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3azehdecm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3orggidvb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vwmrhfxt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zsadfwqi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rceezgwa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ntbyigpn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sephtwyc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3byfdafta.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3andwugzm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ykqtnhge.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xrmmolbc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dftmujjc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nxxxuszf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3llzqtteh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lzupjoes.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zdcfnyxs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wgxlnvek.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3idlhjmrs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3radhcjpz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3fipvfctx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3movntbjr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vrkfixne.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nddsozfp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zlccjdjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vxsgkbgx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3liuenyxa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxcknrfw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lvemvxjp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pccwrzxz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjiieda.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vfylpcrc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fvwtxbyh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hxivqsyv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3exmkubbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jhchtzqn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zipdgzkz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dopmhhij.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ambhwpiw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xrgvgrzi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nnxcfnsi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cxhmgqgf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gopbynll.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3etheybji.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kcpqirym.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nfhfsrfe.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ygdtyawa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hucjzbhf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3godfmets.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zyxcaimf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nmdjlhnz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kyjwzywl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xpvbcpml.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eetqeaqw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ydnfvmey.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rtxxmmty.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gszotxdq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3idgpduje.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffhncaiw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qelvzxvz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jzkpucue.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tznwodqj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dktuzsqd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3exgeojwk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ejihzljs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bngxbash.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3svauxgsi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jsswjizg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3efhgpzjr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3awxrptmu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pieoduly.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3arkcjdpm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3icqxovdz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3emvayqak.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cukczfjs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gmdqoamr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kaplwhka.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kwchoxjt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mpqkzipq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lzfnrgxa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3exregxvl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgbwtcvr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tzmfnsus.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3cwliupyy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nuywzafc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yqqqderq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ucgplunk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hykighpj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bncznbuo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ptnbaqox.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ioatyvmb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zwbbaiaf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ecmmmoze.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cqiddtek.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ubudxzuu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3arumlgjk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xwovxmtu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hllfmmtm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3opwjfujy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xidtjckf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qokbiezo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ybjcjrpw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pszchfaj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3scrdlaiz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqwzofyq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3bwslhflc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzvmbfhg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hgfphela.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xyvagonm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vdhrzvgh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3pllaeqei.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3acjezbph.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wmkkycgr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cjzvwjoi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ibyndwgy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvqplhvk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jqmcbqzu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3trxxddcm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nuizwonq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kluqosmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3parhhsqs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3miawgfwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmdapcsu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3izzvmopo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3icqwzwxx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pthmszkv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ldaccufk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iqeoufzj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rfwfstcl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vqheecmj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3phmuqnla.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3utmzgnlh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3abqafhaq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ugtdippu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uxjuhliy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vzfikedg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bwwmmyfh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kdslotod.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hdyqmnuw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kpuadjqj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rluaqppi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ujaltwpj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3crmyigwy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mbcrdkap.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3erjishyi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cqsgcwbw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rstlyzyg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nvgfvijn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ejtxybyg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bbmessyk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwqqyznp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dsroavav.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wzqkbhji.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kmbghueo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fbvcfwgn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3utufdqhi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gexjiqok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3borqnsef.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3djjskxgf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvcybduf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hzoavalj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jpqopzji.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qepaurlj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tuijcwoe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ssehlpds.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vktynprw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pekizixv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfyaqbwn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jqnvlkmo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rruciwwu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3prloxjlc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ngztdjsw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ilqxgpxs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qwjjaqds.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eghsxbmp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tydmsstq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3aqhepowj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwjqegor.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3egzdqegz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cfycxxsp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cezwqewx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3huarwwbb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3frhoeawd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3onikihun.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xmoceuvy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3oqntijcu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ejewcrfd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ekpvczqs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cfxfhwyn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnoysrbc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zllvirdp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nmckvxdr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kwrjdcao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pxvhcjio.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mznrlzld.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dlxpkkgo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3egqdxauz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yannivyd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3udamvaxu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iaxtxqql.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vsjbtkqs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3idyujdkn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ejvfubdu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dmdrziit.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iupyzyoc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vvnjwqpd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xzqojedq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zvelepqt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3aagmleyc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hkaxkcpk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3yepthspi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vuzofznp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tengwthl.html


<!-- 参考信息 -->