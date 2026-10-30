代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gfvwcclut.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/getvtmktj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/ghvnflltb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gjthjyqkp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gqcymsjkl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/goxyhkzfk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gbelnpmtu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/glvhiptef.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghjbypwzo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gksyccczy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvuspqfqz.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gxzmcocrv.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gaiqapbmx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gscnipgqd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gibwqxrrc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gndcpimwu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gffldxcor.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gtdssubai.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/graxeykth.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gkqtomoej.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmeytoxxj.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gcojhjzrg.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/ghnxoaekk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gskgohgjv.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gozjnlphm.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gygtbnthn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/geandrpog.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gwtxtnynk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gxckjbynh.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gyqdfepwz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/grquboxdy.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/ggizemimt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/ggnvmugom.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gvwwycsio.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gfpzvtgpy.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gbxgzyvwr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gfoybipiw.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gxydfyorg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gcmpbztlc.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gwowpywcg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/ghvzkrtpr.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gegfbxnem.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gxstiuifi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gjezuonir.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gwmwvuaiw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gagssjsod.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gipnbmztb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gsedjhskv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gtimatdlp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gggealayf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gcffxjsyl.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gmehticig.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyanosdwz.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gbatnwjxp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjvjewrli.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gxvrnsfpk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gqycleraj.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gegzecwiy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gdcgdwkbl.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gilsssdlo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gzzbqelhn.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gehiymegr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gddlqekjv.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gbkdnpuee.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/giumyjepc.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gtzrxnpgm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gkbassghk.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gcuvjlaql.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gfyadiaml.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gqgicoipp.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gmylqmdnl.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gjykwpgxf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gtuekqoxo.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gljutsndl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gamcddkhb.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gfobyjdow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpboxskfx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/geqsntorw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzmybqdwh.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gbbfiobbm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giakcadzb.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gselqmosm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gwbxlmfzo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/giklycutf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/goyssstly.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gibtwtyqq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmuxdqggx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gjyliarcx.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gnbiasvkd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gnntlyqju.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gmwjffvdo.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gnfoxqedl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gkgjwhgky.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gltihypiw.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/grjqkkgty.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/goztlljzz.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/guxfiaafp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gljnmqbrt.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gpuuvvchl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxrftthjm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gghxgrbbk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/grbuvlhzf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/guxmrbhiy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gwzjtdihd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/goeoitgoo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gzojkxegr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/grpqhvrlr.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gomdcibuc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gaxidrfwe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gtuhmntdk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/ghuzriztx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gmtibbuyz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/ghklshenv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gvhjwgsvq.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ghyfowotm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gtugidwzk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gogwggaqk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gvhapxpro.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/goewmthlu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gpiztcaac.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gvrsoatoj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gpvgshtuk.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gfndgemdl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gxmsfnzfk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjuoilpki.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gyvvfcmnv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gwcivbzta.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/grblzwfic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gbilhight.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gcvcopxsw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gthniwtlt.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gkzkkdgww.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grlmtouig.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gmbgxtbcf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/geclybthm.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gcjujszba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gcdqonzbf.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gobkivlbl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gjgtdiezg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gnlmgjxxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gbwxymdwr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gzfdsbraw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gtoubnusi.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/ggnbwvkfs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggjunrtnw.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gdxjueamw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqtlzwife.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gqrcsbbjo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxxsmyoto.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gomhqlocg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gebxhkkgv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtpyuhfis.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/groswpaax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxybuznlk.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gzmjlncgq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwcjofmcn.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/guxprejcm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gczkaygvy.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/giswmojkr.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gkzmtgabb.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gfcwehfjv.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gryggfafn.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gclnulnhs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gojzgaarq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/ggtinuxra.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gnbqehazx.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gyvpgzlbf.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/govjmunno.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gvemcdvxf.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gkwzonrar.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gxtxehuwe.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gpklgfirs.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/geivvynks.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gkcgskcly.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/ghgiipwfo.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gijcjtpuc.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/govumgwau.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gbepvyeuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gpotajkps.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gooyrwmpv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gtghcmajs.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmyjnosmn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gaffwjhbt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/ggtisxbkz.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gxioytwai.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gmfrtbeja.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/ggvducned.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/govszwsuv.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmvajujqw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gqdmmphne.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzhgbxa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gpecgpuih.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gpduwpwsb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdtfopemv.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gsuigfdkz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvictvazc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/giymwyrxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grguylydn.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmpvisrcw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gmnmqajgc.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gdlgiisaq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsmaddszy.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gxpindcdt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gavsgwqup.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/grwytrnvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gcfbdktvr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/glexydgyp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gmpscmfnp.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/ggbnujgwn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/goczdvoyu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grerreplt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqogbfwhq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gmabscqde.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gnyxqnaci.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/geahxbnzd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gudefjybm.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gjatpbmxo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsrnrcmdj.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gaxuehipe.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/govfbfpeq.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxicipyyq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gchwfboev.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gvnxkdxca.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gqqbhxfdh.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gimzlxdis.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gtedrayal.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gdqidussx.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gkeoruiep.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gojtyjtjq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gqmhtqffn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gvsufcyqs.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gmvrkrbsc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gbeytnxbi.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gxzswcstm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsrjgsvyj.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/galfzlhgh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gfjssqzeh.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gmqxchdvx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gsdmffjhe.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gyyqwukmm.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gkmsalizx.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/geamjyzqv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gyzibgcbv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjgozgxus.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/ggdshdwpk.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gzmytrizd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gpsrvypgd.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gtbqkvhwb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gggibuzha.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gfdqwfavy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gqdsesooe.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/grczyvjms.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gnfkkzmju.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gvboervtq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gxawaoxcn.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gwlnlybis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gacycwmuu.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gmwvqcrgp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gdzuhsvqh.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gmsvsgbep.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gsmqyfwns.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gxvnoetpx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/grgbnzwtr.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gabhddkbs.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gmbenamoo.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gwbtvjdkb.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gudvblokb.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gwigngbmw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/grsllzdmy.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gsgrthsnr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gzrvchuzq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gzljkcvkk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gqjygkbvu.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gbvkdwaao.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gsllbkmrl.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gxjkepeyt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gbtdromgq.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gjvaoisrf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gycuubike.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/guqtwkeoi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gqabshhte.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gdornegkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gcqaqaplc.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/giyxfpiqu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gwgrpmjsp.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gemzjktvz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gygpuumvq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gytnjoupi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gksbbvaoi.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gqxrkztga.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gdmqehyco.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/geewddsfg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gjrbwlycj.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/ghmpstzal.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gpqgvdrwr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gtwkaaugb.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gekvnrfes.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gomfwcgqq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gvmkigclf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gwukadvzp.sHtML


<!-- 参考信息 -->