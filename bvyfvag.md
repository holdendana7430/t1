代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gkarrcdhr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gdszqpstb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/guhmcmrvp.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gbbrrmiwj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/guvqvkmxl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gektaligk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gqxctaztc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gldsuejbv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gtnwylyku.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gtwqcyfey.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gbwpogwnd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gryobufqe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljwboehc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/ghrmscnef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtkuobxqb.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gbsizhwat.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gjpvklvwe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gmmlvjxhz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gcxpayssv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gorbqsekk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gbqpbuazx.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gohbamhoa.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gzfiyhbjg.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gysgnfjky.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gjzpfjdvs.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gtyilmdua.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gnszpbrpe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gjktvkibr.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gfaikmfqq.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gtrpzyctn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gikdwovel.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gwdfdxmzq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gsmcekijh.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gkvqgwjxx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gbpiifofc.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gkymwqagu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gpqrlwafw.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/grskodzuz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gmeljhuvy.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gmmnhsxex.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gjvjiheby.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/guukyqvbx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gprmyrnfn.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gwvaujcko.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gogrzkzse.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gnwacgseu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmlehqahz.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gcmqcaric.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/ghdckyaih.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/givswgrjd.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/ggxgkltzo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ggcxxofwg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gzbxskuhk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gxbavidpf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gdtpuizvp.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ghqqpwwoe.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbecvxige.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gwooofuxb.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmneuqvrg.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gdoyuceor.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gpfxmiclm.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gbszjmufe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gxpvwotcz.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gangrzkmz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gsyrzepns.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gtgmbigpv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyakrrlrf.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gyaxzexxa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gjydslscx.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gfpkqvbcw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzwyrijrp.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gtfznxvah.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gcfjzhupq.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gzcojbapw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gympewwqj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ghwprxmmi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gduotojcw.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/ggvsryskg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsusifwov.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/glhfaentx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gsrmqamwu.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/grxwbtype.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmsvksnbk.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gvddmcxnx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gychreduz.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gxvcouxyp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtmgfnaca.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/ggapahjpa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/glznzvuro.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzmffxgag.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ggigykfgw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gesoteriw.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gbagesfmq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gfvtlutzr.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gfpjzoykd.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gcbqysybg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gcayrqelj.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gudssxthg.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gwedsnsjc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gdedhstqv.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/grhavzyib.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/guxnmwuyy.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/grfadhibe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gjvzglpct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gjejaacmo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gigrwkdfp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/goyoezvph.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gtbrpfyvb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gmtptggqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/grsqdqcsy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/ghuirargw.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gwdrkzaiu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gfwodecxt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gvzpofdcx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gkzajexfs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gjcscnpyz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gccilsvna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gcbhwfmvq.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gsvfbqccl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gccvbmyvn.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/grrycksqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gfgfrenwv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gpkwavmtr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/glsusndfs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gkvspjdoz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gezpwtkhy.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/grcfbsmti.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gyptdsnsn.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gbzojoyfj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/glefmwfen.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gbymhemsr.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gkezsantf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gfzbosxwt.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gheuhzptm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/guclirahq.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gpguljhwy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gpmnzqbgm.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/ggplovtsi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gdxwcjeqk.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gnhmvvqqg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gpjyzlhqd.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/grbnmuefs.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gsvcxtoxm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gnflxqyjx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gwkzbrmfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gvqzxrtlr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gsnccguch.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gsavmnubw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gywjtqwyq.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/grzcaavpa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpwvqkwgq.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gxtfmioqc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gkmndzurk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gxoheaerm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gaoiiklei.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfbucednp.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gcihnihhm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grekxqlsz.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/goepxkyqk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gqfcxscxf.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/ggsjflmwq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gxyaibqik.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/grtcczmbi.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/grhltmzbb.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/grchcqisu.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gvyxxxytu.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gsucgbjns.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gglbfrnhn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gqeeccsgo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/ggnqmwtmc.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/grlzkdirj.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gunjnjeqp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gqdinvwvx.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gfbzasknf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gemvmbdll.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gfnhkrfim.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gkigwpgrj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gslhvodoh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/glhdvwrij.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gytuxlufi.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpzybenhx.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gnrdvwybx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gzgtbccmc.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/grjxzsosh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gyccupvze.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkqzlxpqk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gejooahno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gfzqrddgh.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gqutyavus.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gxphjbfki.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gjrsgkmbg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gheribkjn.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gbbvqhkvy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gbfbmiyzf.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/griybzouz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gsxalxchd.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gruvvivcl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcrkavlnd.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gvmmcszdx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcgxgljro.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggwakuipm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gplonljbs.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gsdeemilr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtiqrbpar.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gnnewzadq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghhppegpr.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gskxoteyg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gmaedbhrm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gwmljqego.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gxowuxcje.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gcgaunlsd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/geiwyghbp.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/grqxcivdv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gvlcwancv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gffbjxneo.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gmauuexdk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gezsovpwb.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/ghudihpmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gdaugqcbk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjtgqbqdc.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gidaldmin.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gslxnmpmc.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gydpzonpj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gydjfsfxy.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gczvhfkun.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gjufkjrhr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gkynbmhcs.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/glhmvvybq.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gfbhvnlzw.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/ggymaqefl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gkhetfows.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gxsarmalr.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/ghmfxdbew.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gtfbvkzbs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ghdrddyvf.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyrzsljxg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gqvuqzegr.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/guvdowygn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyqbwygnj.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gaaajtwzx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/grjfbvesu.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gbtnpboui.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gthwmtpcs.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gwlauioxx.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gbfcqxneu.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggbfcqtjy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gyhmpmipl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gslqlmgyy.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gkbfycsqy.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gzbuyyknl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gftldmdgd.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gctptmicf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gksukvnbz.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/ghlohbcku.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gctakglio.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gyweopzkg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gliafdpdf.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gakxeaeai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gmgkcelvj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gudqhsefb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gplerlclu.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gfousopqj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gahyfjums.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjgoxvxxz.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gkahewjwu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gcsxykdzk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gzlhhkfad.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gdrsvloep.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gmthysoox.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/grulrguzr.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gtzwkahvk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gongsiqgg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gbzusgkvv.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gflowftgp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghfacanpe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gygnorvgl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gilohfvhb.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gjrmrxcqg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gckawbyah.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gllsabpch.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gjtufnuik.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/guohqazwc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/ggpqzporo.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gcaxpxksr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gisyunhpx.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gfqerbowl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gmsggpuvk.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/glbivqfwb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gtgzyumhe.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gepndhvek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdmzwvqgt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gbqwdqayt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gwfmujjbv.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gmuiganmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gybqebari.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxmvsbtur.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/ghvvtyzkk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gcmjhlhew.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gmxphrfjx.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gwkpyxpkj.sHtML


<!-- 参考信息 -->