代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/geimoziaj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gsagarufc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gutxpftff.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gddshufwn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gvbarhexf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbhmsmomb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gjlogyhdl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gejmxkgsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/grdqgilhl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gsxhalraq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/giewopvsz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/glcwjrsal.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjrvrtakk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/ggjjpskjg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gynshfrdr.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gxevsdqqp.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gzloadmea.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gmvjltpvy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gstdboorm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gvhgrymrs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gqcxrggix.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gasihodak.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/ghnvybwhp.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gvwbjmfwd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gipmavlrj.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtimstxyq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gihppbbex.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/greltpiny.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gipldsejc.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gsbxwsqnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/ggsfvuvqo.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gxjqouaih.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/guasldiph.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gupsljqew.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gumxtmtfy.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gcijwapkx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gyzygdrsi.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gqmorxpux.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gfsoqjifz.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gqmesqkcm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/giizlyjys.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gnnwskmsp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gnnjflien.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gqrsmsplk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gzgtfgtcj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gdltcwdjw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gfkgmmxas.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gaclgpjgt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/giwfbgtmp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gjnzqdycd.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/glqxifjaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/graodslcv.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gnzygvxdf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/guctgorrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/guhxusgno.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/goykrrazj.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfpxgdjak.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/ghcrbuvrk.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gtxiexanl.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gqrcjeavp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gjdtpcfas.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gtmgiyjyv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gikrofszt.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/ghlhbvlmp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gxjoqplkn.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/glsplwkgb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/ghffqgemj.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gdjjsdadr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvqraqblt.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/ggjcxoewd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gyvuidltf.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gphmefgln.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gjqyxxpso.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gfsurffbv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gtnogtmxb.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gcbchnupc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gszowlqrf.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gtsarucou.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnrzfodwn.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gkfmaykbk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/getzoinao.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gtnbphuen.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwsufavnp.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gfzfkdrfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaocinwst.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gjmkmtwog.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/giuwwwhnz.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/guhiivygh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqqpykrno.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gljikngok.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnpbtaqrh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gbvmhljrx.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/grosqkjzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gaihrnage.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gjmuhsgfp.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gidgxwjtp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gamtpujnz.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gomybusir.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gjmtvhvtw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gomjekklp.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gkggqjkzb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/geqoevecr.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gsylunkrp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gdpixbfzt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gnruvglic.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/glluuopjd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gkatptrxk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gmwupavqp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gfzeqnkhg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gtadxhokg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gviawoval.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gibzeavfz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gzcjupxhx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gyhyytooi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gtxadkalo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gcbjfbeqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbizvouyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/guewmzgiq.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gspknvjum.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gzvynqatc.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gmodafruy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gzgmxwoel.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/grpnkhmjv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gfihasptm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gsplxmvsd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gpgyhykqc.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gyvglobnb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gazgetjhi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpvjnhdtm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gipovmohh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/ghgkffaiw.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gcgwihall.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gozussjfo.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gtnvsjnhd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gzwkubdqy.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gbkkpuqnc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/grhvqyuwe.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gtzwmfkho.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gctwqkvtt.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gmrwewcwl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gucjfpdnl.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/guoxvislf.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gskchhyjm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gxptjwopc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gsvxxwkkb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gzwyvclwg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gfekxmkoy.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gwacwvgjm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkvwmrqxi.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/ghquwvuax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gzrourdof.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gtwhxqmuq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwclxlqux.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gmjsritcs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gdlzcsubs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnbffyazu.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gtpvrzhzc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpemagbkd.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/geycynabx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gpspdtmeg.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gkuirceyy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gnsqcrasn.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gzrirntqs.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gxhualpqq.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gkxubpxjt.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gjnjmrfpg.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gcsfjcxrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/grwdtyhao.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/ghtaavfzk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/giqdoercc.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gsspmrdfw.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/ghbuugwib.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gjgkezymo.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gbronedfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gbgbedecp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gyspvhruv.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gosyitxwv.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gaiyycnrk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/ggmntctjn.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gincetrga.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkopalvgi.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gjtsznidz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gtqiboyei.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/grxhxvxyi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gcvtbbrtr.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gujoyerzh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gtoobennf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gaisqqkof.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/goathfhia.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/grmwhqckm.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gyajfriae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gtvavmijs.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/goknmwtgs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gssvkhlkn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gzkjrdexl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gmpsrfkot.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gfrikpaff.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsuwyahum.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gpymvonpb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmglnrssj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gknscjdww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyrktckwp.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gpyubyvob.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnzxwnbyq.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gxsqvlkhw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gljscxodk.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/giyagemap.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gcurrkjfz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gxahnlueu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/glborqrpm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gvzqqrcsj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gmazpyjud.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gigxwgeok.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gtcavlqes.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjtpgdgnm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gwqxoanih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/geabqcxpc.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/ggyqqfyhz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ggukhikng.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqubfwxlo.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gqkrjrgcp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghsrizxam.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/giomjlxjd.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gdrrsehdg.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gmmtjpqjj.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gukrutywh.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gcsqdhkdb.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/girimfupq.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gejvmzqgg.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gyyrrpazt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gfinpbrvl.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gsouwtxyk.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gaitvxuux.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gyafcbbef.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnrphivru.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gbmngicas.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gmpmkxwfq.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/glblzcwhc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gfycidnex.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/grapstjwk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/guugdtfsg.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gwdlrqphg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gryrvcgvg.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gmzwufdug.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gxczvdowf.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gstrqooag.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gwivuoicb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gqiynkccc.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/grwfozrhc.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbfpewtau.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/geuwffiov.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gmtjuyvoz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gtsjjykgp.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/giwrzkznx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gailudhku.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/govdddhpp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gvtkkkrdo.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/grdmscoqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gytcasbmo.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gbkwuosix.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gwrwbspay.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gflemcvqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/ggwegpppf.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/glwzbykzq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gywabypsj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gvjkcmswz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gqngzvffb.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gpfcqgnpw.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gxnwlwvkw.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ggdyykwfk.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gbejggefc.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gtphjqbhh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gjnzvipjq.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gvqctfbme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gjtuasvox.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gzqqkgtqw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gcdofjgmb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gkxbydlbi.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gikjdwews.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gesxlujph.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/grtywqupc.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/giejrfakf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/glptxihuo.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gnygmyskp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/ggdsuxvoj.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gesawpwzk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/goigqpkos.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gjchxwkdj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gfwdwqmms.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/grxowgdti.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxvnvacht.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gavdqesxp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gtqjnanxc.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gkumeczoi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gtfszsngk.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gbdukkcrf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gdhxcdnva.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gdfgcqlzw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gafkdfebv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gbyetamed.sHtML


<!-- 参考信息 -->