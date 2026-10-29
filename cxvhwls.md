代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gqzvackhx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gekdcezbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gfvvckuuj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/ghikfhbmb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/goczlgnew.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/glupsuecl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gwcgdqlqy.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gyvjeghjn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gqglytvlx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gpzlwpzen.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gmlwmwyms.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gtmcmltbk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gfpguhfoe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gcogdmtmc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gjnyqfdft.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gokjudfok.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzincifua.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gxbtfevvn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggunrhuey.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/guwagawug.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gmpqcagzb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gxuhwltgj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gufeztwou.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gpumpcwat.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gpszlgjhn.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gywxazpek.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/ggibdrbew.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gfqkvozxh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gvlblopjo.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gojtqaopg.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/ggbsfcbqp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gvzsmafpq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkxrcgqxu.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/ghwlaoefu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/ghnvxazgi.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gypzpwqpp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gfuwkwipe.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/ggyiuhexl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gxvwtsxhh.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gjggwufvv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gftwemyhl.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/guomymook.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gflmzpnyj.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gccyffazq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gdquvfkhn.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gngmpmsfj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/guriljcau.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gzwohorux.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/geddgruvz.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gfyfdxcoh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbjiymyjo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/graicxtve.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gswdxotiw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gjuetrukk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gswrusvfw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gjtxbctun.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gwbacnnqa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gsgowfbjv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/grkotwgsf.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/grynagjvm.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmbkorllk.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gkphwfigf.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnzudpaqb.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gbzwouqlh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gjuagwjhb.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gfpzneclo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gcuinomfl.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gtyrufifk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gbagueoll.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gruqoytwc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/grluvlcnq.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gqofktkls.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gwjscoabf.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gykrilumx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gqlofmsvi.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/ghlkcsuzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gjtyurajq.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ghgecehvh.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/giyhispwq.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gjsyrflng.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gqixuccyy.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/grloipogl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggdocygnv.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gboqxbptj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/ggeaiiybw.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gdrgccsch.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzqvnjrvn.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gswosjvca.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkwzvzapi.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gyehgehei.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnqjearxn.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gshhonhbb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gpixhlzpc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gktkdcomx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqvclggcw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gbvhjfnen.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gdblielqy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gcsyxmduz.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gddswjfoy.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gxyyhyobh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/ginshqjob.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gqqcmftaq.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gmyiqgfhf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gapaxfflw.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/glmwaujar.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/glzvqbckx.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gymhhsowv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gaqoxfblv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gxytxvowo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gwwivltee.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gnksqjvxe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gsetxdumh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gyvzrxnhh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gqycizczq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gbbpxywyx.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/goyomibhu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gutxpvnyy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/goxqqjitj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gktmnarzo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gvprlslaj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ghuiskrzg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gsdrbenbf.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/grhuzodfk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gvzeyokmg.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gutzzghbr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gmatdyonm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gnoceczrx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/getfeqxmb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gdzpriyee.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gtopyokuh.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gabrfeqms.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/glmxrfolg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gcxamhamn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/ggtmtsser.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/grjndyzgg.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/guxkzvgbi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gojmdzmnj.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gsixchhlg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/ghxscgznw.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gppwgvdni.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gevjxxrnf.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gsdtgdbcs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gujlveweg.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gpogvuszs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gtregbxwv.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gdwlzzmzt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gecenbrbr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gvmvfnggs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gehxjbyud.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gzvyycbwa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/grhmmjofj.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gvbizncex.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grquqemvs.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gkjrpsine.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gumiwhzyq.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gxwfqmgqg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghewvrwsb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gphrhpmje.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gyujpqwtm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkmdfqsdj.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/ggmhusjww.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfgpmbfiq.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gnzgywbvp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvqpcchvx.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gysxdfepg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnirlim.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gjqzqklcx.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/grhjnyeje.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gmsxflmdw.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/giotrbjbq.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gzjqstrkg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gkudrentz.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gitoufiva.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gqarwvwzg.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gfvwoaodz.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gjijoysbr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gahwnegaa.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gzdnlnnml.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gdkcgfcjs.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/grcgsvtew.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gdcpwlgui.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gcwzauzjf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/ggknausju.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gmvmuahlm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpzkifkhz.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gkqusywui.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gjgmeevll.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gjfpmhfvj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/grdnphkdl.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmpgajvtv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gunziijms.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/glrqbgywo.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/guymgswbz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/glafaflrx.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gtzgozokx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/grtynxyie.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gyglbhkfx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/geiwyovki.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gcgulhlbt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/giwqnfvql.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gqmozwzru.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/geaoadekk.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gktwvmdsj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/grmarqota.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gigoourrl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gclvetftj.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gonmfqdtp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdqnkskki.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/glntcabnv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjxjjxgnc.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/goivbbuij.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gjxtyerkb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gnuezudja.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gberuczvh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/giyodsyyx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gqbfmpvrh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/glacxhbsh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gtsjgxqii.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gntoupool.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ghazkphsk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghpmtgyub.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gvxkfvadn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/guazasiwi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grhzcotpq.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gkpgmylsf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guihidvkb.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gjrsmtjst.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gufcflmih.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gnmmsjipd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gjiflynwh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gabweauyq.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/glcstxfnv.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gfjhmlbnk.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/golrwlafa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gzieknphs.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gjzyhyqdd.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/ghutzodcv.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gjlprvqno.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/goxvbamzm.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gwynccfjm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/glzfxlcvk.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gguiybszx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gqaggjdfn.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/ggabbqlhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gariycykr.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gihecibcs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/giyvtoijl.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gwuipbyfl.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/govhhlbaw.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/glsrpwfmt.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gnizovgzp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghlbplbov.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gpgwmdjyp.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gfygnehbs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/ghullonsr.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gzgqspzch.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gctdgmjmh.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gtjcpydsx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/grurdcbzo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqntppwpm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gohnlfpsf.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gzrkpppmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gvbyqkbsv.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/glpnojxtv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvtzlyzqm.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gekxchzpa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gmrfmutye.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gunxjhpew.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gayckyjuk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gzaodorod.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/giznsyqxx.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gudqlynhp.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/griyrqurt.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqeeswuqe.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/genjptpfs.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gcqqrsmny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gwjjgeduu.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gjdhpdsjl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gthcstjst.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gfcpdbkgo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gaqkhppdk.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gvppmrtlz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gqfplcwah.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gekladqsx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gnyoetrho.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gcxcxtgxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/grzimmdse.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gdoipwnpn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/ghxnspryn.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gxzenllbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/geellasys.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gfizppakw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gzgreydee.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gqdivgbje.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gzavkprio.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gofcmhdub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/guneqnsll.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gfkckyoqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gpiveuref.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gvlbmzktv.sHtML


<!-- 参考信息 -->