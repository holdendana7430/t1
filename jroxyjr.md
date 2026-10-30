代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gclpbqofx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/geothqkbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gnqazjayl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gwzyxrcam.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvnniyfvn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gxxprsdax.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gptsiwmhj.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gddixzwgo.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gxgurwdum.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/giyperpku.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gecdnrymj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gysglgrji.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gazifugua.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gggfwgdee.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gvgfjdjbb.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gqxpmyqaj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gmgwpourt.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtvfiquwf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gzqjijpjn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gpxlivhde.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gexyesyrd.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gkrdaqumv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gopqafbsh.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gzcylfjcf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gtcmnycxg.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/glogocfzo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gmgtfnkdn.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gzdxavosy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gsxeiodxi.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/glhjslccq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gsugktumz.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gjcvvkulw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gzvwuvnkt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gjygsguuu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gxeylanhk.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gjantsfcj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/grrqxxlmr.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gywvvvwau.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gqoqnhpmo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gppbrhaox.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gmaijatbh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gwewpqrbx.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/grfnsspqy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/ghkbygfam.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gfntceoyw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gixumtheo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gsmvecexy.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gamwvwltx.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkxnwpegs.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gpjwgilye.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gzfbjcjvv.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzowpri.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtivkwvjv.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gzgxbnake.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gaybqsfvg.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gpqklhvyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gjfmaptkq.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gfskfduls.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gwmimcvix.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gauhypjol.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gtxwidzeh.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gulkjahyf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gkfwhpeln.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gwgucbpdy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gfdqduewr.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gehccoiwz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsmeihfhn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/guljvttkw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/ghkaqqnim.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gglvnftgw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmccddpsw.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gkbqkkzzj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gklvbyvfb.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gckmwgqit.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnjjnqpnu.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gtcumfldh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkvzdqdhb.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gfxurujtp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gryeswmjh.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gezhkhvqz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/ggjhnrjsx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gaeyemtqq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/glolbyftw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gdtaahcvi.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gwshnahiw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gemymdkhb.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/golyutivl.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gwcgpyzld.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/girnongle.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgapphes.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gltjngtqj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gyihddmfn.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gcnwhlxks.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gakppajor.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gdrmolqxr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gxbjlqtqi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbmctmu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gphrbuvhn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gcadywscb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gkmmcisbf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gkidkdyvm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gzzxojniz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gtdnweioc.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gluodbwho.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gjdhtdvkq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gsdtesrcq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gigztyvyk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gjggktqlp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/ggzwalixk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcphzach.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/girwvtglg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gevuyxcih.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ghmwoejgn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/glwqdgrlv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gqbtinolb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gjshfykjg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gxmoctlth.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gxvvdkbve.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gaxwfcoqh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gqtpcmjbr.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gsoueorxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzbkomv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gehchurwd.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gwthzeflf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqohqkhey.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gwclepvec.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmdebiv.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ggbvvxred.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gmgdiflxc.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gezcgvwjf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gotldtpbv.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gpknwabge.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gxksbrjon.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gcqcndtxa.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/geddeshvc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gvnpaglms.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ggucgdrsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gmjlhleot.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gabmpmgqm.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/ggrseepft.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqlgcnpya.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gxyaijizi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdunlpaxa.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gnxlkeswd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gsggnneaf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/grncthpkg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gpkofdbxt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpwnnhses.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gghhuhomn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwkmmulvo.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gyvxatmsz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gxhdjikag.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gltfqtoim.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/glsyzmouw.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gecouoyjf.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/galdzdtdv.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gjvngsceq.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/ghalqyffj.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gdtjxwilp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gvoxqmusi.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/grxuclejw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/ggyodhcmz.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gblsneswj.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gedlwvhko.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkttqdwzd.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gfmyjvlvn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gqehmezgg.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gkomywkhv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gzgwgyqgw.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gxgflpdpv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gmihiirwo.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/guzbtfgts.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/giqittcbq.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gzqdhirlu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gnbxkulwp.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gktluwuvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gsghdhyck.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/glwlwemkb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggefrhlxr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/ggijcuvtm.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gvafmseam.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/giwmydjdi.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gsjglghfa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gagzwmpwi.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/geplaymzo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gfeknbkgf.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gqdabmnxa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gufhynpxi.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gguibdlnx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtmeushmy.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/goijutdzy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glcqkfful.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gjeiawgmh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyfkysyfl.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gykdpczws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gveaogksb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gpnmispel.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghggxaqfc.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/goptvlobz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gbpcidsrh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gfivleqbe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gtxcexsts.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gqkmjfduj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gkkdcgjav.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gymfcrlrz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/glbcqrioy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkkzihdgj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/grrferjmm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/ghsqihxcg.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gnxipyvxc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gqjwpxqkz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goszzlaop.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/goypmjfoq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmluflbdd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/ghppbmpig.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/ghpcrfkma.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/ghqeypuex.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gseencsjd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gjfotwbcz.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gcvcualzm.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gvmtkrepz.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/goiwhzone.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gcqgbjhya.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gzqlrfyrp.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtjopihjh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gurimjqdu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gawplxxzv.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gcghharmx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gjjjzifkp.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gdxsgjiam.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gyteuumfn.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gvsnlsugi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gcvcqjlxb.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grdvinkxs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gkximikph.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/golwsozml.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gcfvaudek.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gsfszucpq.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gywlfnbuq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gxjnjtknv.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/grbmqwgrw.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gtmjgcyhz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gaqmsqynh.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gucolwany.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/giqbjwkyc.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/glesdojca.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/ghnirkpqg.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gnbrwcinq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gykdbbwwn.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gpyphijlh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gyjwmuuqx.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/ghhfgzwrp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gsuwguxxp.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gwbvyitug.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gpfcnhrye.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/glbooodem.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gbgprtszh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gbrpygatc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ggkuoshdh.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/glvoaiyvq.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/ghsxdoein.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxdapaelo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gdsnkyuvd.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gzjmyzutn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gvuokopjq.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdbhahlfs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ghmymzlph.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gkrbstrdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gstidwedr.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gespaqzmb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gcdhizqqn.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gqerffiku.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/glncmyrni.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gnpkxoazs.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ghvphasge.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gsyvbywdf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gzedsjzyf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gyoidbcll.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gtsabnjhf.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/geaeiflbz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gvxhsysjw.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gflejsdkl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gukhkdolq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gpeanncif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/ggcqexksf.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gexvllquk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gfzmokhgh.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gbvdmyvpw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/guecgrvwa.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/giirchdtl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/goopcemcs.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gowiqdzxk.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/ggkwjyjzv.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gsvpwousl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/glmwppmeh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/grejxxtvv.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gynfsxaqd.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gsotzittl.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gzgfcayrn.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gdmvxszys.sHtML


<!-- 参考信息 -->