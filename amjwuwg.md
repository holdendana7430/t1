代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gbfwkbupm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/giszknips.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gsshvntoq.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gdmqfmhxx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/geyzljvon.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwjuylmda.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/ggtsefyke.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gcqnezxxq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/glvkfvktf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gyriphyhx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gdhmdmwgg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gviqxxatd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzswkyeer.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gvlfmxdxr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvduzuwgx.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gmtksznpn.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gtjkomobq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gpsoxpvbb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gpccwufyq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/ghrnidqdu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gptdyspvy.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/glxkmumvm.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gdqqtjmrz.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gwgyzkxec.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gbtvnjzut.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gdybxijhl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpujubj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gmhrctbbu.sHtML

);
来源：http://wap.fehbvm.com/Article/details/godkphrfq.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gpcmkvnae.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/ghowjlwqf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gisffjaib.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gcaigduhd.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gmxkddawx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwywuzw.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/geunvnswl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gwwuikvgl.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gttprhvce.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gfmlcqigd.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gkxnqdkpn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ghodxzoyq.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gvoiozwaj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gtokmkfwp.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/ghhpttcax.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gaxtmuzod.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/glopapaiz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gdpfoltai.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gaskuxpua.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/geqinjpjn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gnzdcbojd.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/ggypwugdv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/grgtmrbry.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gdkiscvph.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gsyeejlfe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gvsvnnvoh.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjsdvso.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glrqaysnv.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gxavvtrfn.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/glrqqdwwy.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpoywta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gdohpfufk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gufebrann.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/ghewvtoar.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gagvdzfhs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gsdrigabb.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gjckwbjmc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gorgkmblu.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gfvdxdcjh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gibyhzkua.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gfqsxfpsf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gvgtogxzn.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gvfejsrdk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/govnausep.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gvlolurlj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gexlhnqvr.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gwizsulcw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gjnhbfpjj.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbygvdm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghexzqttp.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gsffjalul.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gujxbbqbp.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gyoralojl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcbjkymrt.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gfcinpqdp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvzpozfox.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gctapusiz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gasumylqj.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gncrbxmkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gaxufsiaf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmakebbjl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gcglteivj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/guadjflkk.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gwhdkamox.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gfmtegiwy.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gkfbztgdv.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gbdwfacig.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gnptgxred.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gvavmewli.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gwaowwmzw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gffwootjy.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gmvqhjkam.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gvzuzupml.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gcaqjsrwu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gitazaobs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gyfcraeea.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/ghhpejlwo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/glrvoliqy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gfvxdvyrf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gpwkvohvu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gqpyxypsb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/ghxpvrilj.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gfggagtqn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/ghzcqvnhp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gxoltoici.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gdrdpyguc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gjwezymqz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/ghsslzpxl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdhealulo.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gmslrtytc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gpoupudxt.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/grymldbuk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gazufcorb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gzmpoamyu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gsijnpnrm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gpfigfnrw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gzpexigoe.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbcywythq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gfbpbaamk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjzxubgzh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gpxprdhqm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gardgfvrm.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gzbnftqop.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcckbcibl.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gplcvtkpi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gpyrwbbja.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gtjawzgak.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/graqfbkvc.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gdldylqmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gndpoeolx.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gpegeiqij.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gcfxhpnvp.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gzgbnvalg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gwblrkccj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gpeqinswr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gpllzydsv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/ggjvvnchp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gmrqgjvdq.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gpwtksrli.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gunolaqhh.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/glxmmeeop.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ghclcgjsc.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gueemaljl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfyexrrbg.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/glqrdsfli.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gqgxjuhon.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsbcydksk.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gvxaixkvc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghseijmiy.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gldxcefob.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gpgrlxuup.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/ghvokuqlk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gmnxskxlr.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gwgdpvzew.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gfqwawffu.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gmkxzycus.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gbqxxpvgv.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gmdchheyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gdceuhrxe.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gxrxfeqtl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/grwnpsrzq.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gwswikvlm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/geogpadju.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfmfgjt.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/glzcfkbej.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gtynjipzu.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/geilzttza.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwieqzenm.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/giqoaltil.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gvkwglxmf.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gxitawttq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfroesduj.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gbjddyihf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gghtchgyi.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gsxkljuty.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gcvigfiam.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gsdleahjb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsudufchs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gddgypucj.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gxalfdrpl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gkpszidyl.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gkramublq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gibqiccfy.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gvwkakkqs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gbnynzefp.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbpxlhtld.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/giwrjkini.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gmgjjuble.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjuqplptb.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gkgittcij.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghsiwenlm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gvbhcknto.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gowhuxtkb.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gjnsuqjvo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwuokqdho.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/giydnbvks.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gllfefpep.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gxqkacxxd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/ggxjpawfk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gmflcidzs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ggyhhzubx.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/ghgxvymkp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gintkzfpm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/giunnxsud.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/ggrliwwis.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goscnffki.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gnldgehqq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gvzcypixc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gpmrxibds.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gmmyjhukz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gizcvjzsk.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gyuultqkf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbnssonhl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gweqdpbto.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gxqfvlnzl.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gjnpxnahr.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gohlbthyy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/grcaeykpv.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gwicfgdoz.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gcbigaqpq.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gsummixfq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gysxkkfsy.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gjqrcwvjy.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/grglktxqj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gpiqusylv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gbqhsuzzz.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gzyzmbecw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsizhcyzi.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/giwyywvof.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcsnzxuco.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gqdztqdpm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gjnpaalqf.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gzxppabrb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/grvzqbjhz.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gytdiglfw.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gbgjlciqv.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnijkttux.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gooafuvco.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gxjhhxzrv.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gbrcosefp.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gpthkyzjl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gvcmxmyxb.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gvctuxxhf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gumyqctyv.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gmluuvrdg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gkvzvaoat.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gpibzptuv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gjgnsfaaq.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gcxmypduo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/goshqtnlw.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/geeyueuhn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gsanbdaei.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gwpecjnqz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gwzjiglch.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/grvurnqkt.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/glroidirp.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gxmfumdjz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gtezjwwrt.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gubpoyunl.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/glxiihyvw.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gdpedqvno.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gezqomrgt.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/glwsmliyi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gswkfcaun.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grlfruozc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gfaoivjtq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gebkuxhuu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gdwqxrook.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gttauwutm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gtpaolllf.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gznajjttf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gnvegyjht.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gwyvihyeq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gdyiqmzxu.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwhxgjxxv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/ghifpxhwg.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/glwqsvffw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gljbijfga.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gcobsiuah.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gaqxrwmbf.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gnwzocuoy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gzknnqtxe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gmzsjexyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gliuaiudp.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gzffgdmnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gaoyqtlei.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gsnehcbzp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gkempjqtq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gpojlurdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/ggaiziydr.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gmlhofggx.sHtML


<!-- 参考信息 -->