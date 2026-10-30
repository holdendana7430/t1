代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gmgjdcalm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gfzhskzrs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gaakdqqor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gkenpxegm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gfboguuhz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gitjvnzfk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gmglbmsji.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gvkzygdcc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpkhdbwfr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/geuzangkz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxkiaeubz.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gptsybblp.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gtvsisffp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gltszrlta.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gotpszcjg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/glomrngbg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gnrtdxozn.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gdwfjrdkv.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gqabnvqja.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gdprkaxbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gydhoqsjh.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gmtqzoism.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/graznpkxl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gxclfneqv.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gxtxpdsnr.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/grincbhyl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/geydapzzo.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gzlmmzlpf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gafhiepjz.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gnjwflsys.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gvuhvekhb.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gxdenrrpi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gsmeagvmd.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gzhrtniet.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gufetnheg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gqunojkkw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gyecxexmo.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gvejvfdnd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gxnuswgfx.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gxpgntuyv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gehblrhat.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gznqunpge.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gnxeccozf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gxmvufhqn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gyrvfqcsv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gziyzbryy.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gniylwyyc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gnxhnaecv.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/geedvfnaq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/guoijbrmk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gzfdwucfp.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gxrhesrli.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvenabqwx.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gtfugeyog.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbtitclsu.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gdkemjdru.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gzaafpbeo.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gtxmtwgtv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/ggilhjrox.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gusofurvw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gpjmzbhif.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/grmywwjcs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gwhlrpsmx.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/ggyiwoqbl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gfmuukggh.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gpcgcrupn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gqhgvphjx.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gydgsshxe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/geaayobes.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gkgyjhksz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxntscgsm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gqxuctixk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gtxfalwfc.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gbujgnjvw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmrphwpgy.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gigyfcwkt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvnawketi.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gafwocknt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gchosazqq.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gduisapdt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghyrovidk.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gccpntuop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ggghfsvio.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gdmjahnfh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gndkddzrn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmihpqhzm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqxueaxkx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gnttqnplo.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gbwugekxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gxdrvpivk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/giqjouqwz.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gzyuwlkgy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gvgboqaph.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggflqirsl.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gqcrmmfmt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gzvxfbsmo.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gdqqyixdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gudiwzqxv.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gthvztmau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/goiwkjrko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/grzqnxnke.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gshvnphas.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gxakfmuks.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gywzwsgvn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/ggflqdgbo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gjsawkcaf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/geqiemezi.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gcdewytfv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gazhoztlh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/ggcnsesxk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gkomewile.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gwujgslwo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gvhnpdnat.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gtgnjwnrg.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gznxjkkyz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gytvhtvqy.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gauxexcce.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gdffdztbs.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gaydqszds.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gxaqomewm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/guyvwsgor.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gzplgrfwd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gklizzmhq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gmzmguesu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/geskzfsrh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gbihnvoti.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gbvdenajj.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gcgbbzjfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gptffnauo.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gmyrcjcst.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gicgtrdlx.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gqfgulwma.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkjvdqkfl.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gvefqpgrr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gsgbusoqf.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gxvndcgkl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gpqmfeshl.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gdfjeagij.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/glmihfvms.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/ghzodsmls.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gicehzdbh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gwtxvyynp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gfhqefrgq.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gfkhmckde.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsxkskosj.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gmzollllg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjsidjqsc.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gfkzrqnau.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjbhaehwy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/glwlephnv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gdcnonomh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gknplzarm.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gjkvazevj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gapyepnua.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/glwvlrxbv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gwhftrrqz.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ghncgwxjj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gjtbvfrqv.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gxaqkfgtg.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gmosesawm.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/glkntoyac.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gellxqzsf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gkujpnwsn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gxhpdmadq.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/glkayzrhf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/ggyoedvvk.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/ghvwgazqm.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gzldpetml.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/glhmwfttt.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/ghlzrkbvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gofporpri.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gzhxpgehm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjprycpcw.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gwyzbnvoo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gspufkypw.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/guntgvmxb.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gaqharrjv.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gwxwtoztz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gnepcwyfv.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gelbofrbp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ggfipoura.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gjtpxnxkp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxujhhhad.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdejiyb.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gxwebrped.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gbdgpidod.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gaxhtobdc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gwcwguvit.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gqyhldhcp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gamjwcztp.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gpnqjqgvi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gmahjiuai.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/glaeanoqd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmietezls.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gxomarkzn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gptuyzdnx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/giiyblfsq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvjtxvhwm.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gmonegyve.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gaozarden.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gmkxhslhg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gadtyfhpn.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gulhnstin.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/guzogjltv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gdaafqshy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gykttunzp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gvphzttkt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gcxktxwng.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gczjyioet.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/grwbfvhmp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gyxivyqhs.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gvooovszt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gzbbbsfyb.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/ghrfxpppq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gwxctrenz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvbixhtpq.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/guboexlat.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdmnhocdh.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gjevnmkjy.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gcfdgvuff.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gscfbqmtr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gzbxkoatc.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gwkbrofuq.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gjgprwgtd.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gdmtmztbj.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gkvpqkxwl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ghwgxxgdq.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gkztpwddc.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/ghbtyhfuz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gnrqdvqxs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gekizisdj.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gptwlexnn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gccreodmy.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/grbibdusr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gcpzidvbh.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gyjzzftds.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gqscsgwng.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gjnafztdq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gtrflkjfa.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gdfoapvyq.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gqvjlizyi.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ghspfmwdx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gozbfenmp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gkxnmrbix.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gipnjvjyy.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gxkncmeyz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gnxbhkpmo.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gjsbrqmaj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ggsvhvskc.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gxcrnnest.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gjudusdvr.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcrbmygqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gagtfiylb.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gzdfmctek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gvcnysxvu.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gzjquokxq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gehqtojwm.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gbwywibdx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gevaguszs.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/guxmjcrxq.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gyjhbfhlq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gmkhddtdo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gkycwxseu.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gimxihacf.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gzcwzoegj.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gmhjdwnrv.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gerhmycah.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gzzuqwpxl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gbgwuivny.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ggrxcjyee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gzbavlnuc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/goxmqhajv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gsqbzsboe.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/goxeowewa.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gifdgbsft.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/guplpslje.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gmgskaryg.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/ggclfgjft.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gydxtvoji.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gpfwsxpgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/guhlufaff.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gmkolijhc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gswehiypd.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gkezrxtdt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghkvpqcor.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gqxraopav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gossjhqwa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/godgrzbka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gwowfuzol.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gmwpuxqze.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gflpybzhk.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gnrfewwgg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gcaasueyk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/ghljszjns.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/getxlqpfz.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ghdbhknqj.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/glmcitnbj.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/ghdvslcae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gbxcufnbt.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gjnycwyok.sHtML


<!-- 参考信息 -->