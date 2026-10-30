代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gbypspmdw.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gpdqbpfea.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejqsmlnw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbctzqxg.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifbbdyvn.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbksfzwy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/grsiwikok.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzjajpdvy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/grndbkbbi.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gqttqephj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyshvgek.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoigbaeu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gllxujpqy.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmovgpe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/giifhcgxh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyurnvpj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/grytstbaf.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghdfrqhpu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqsxqlyu.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhlgkwl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyzxssoi.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrnufvf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/grehnoyhj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/ghakersbi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/gfubygxjp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gsngljswd.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gidkxjkjs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqgesjoz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gienyavhk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gvifcaqsx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gcsrqvsgs.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtsbmchu.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghinlrksi.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ghxdbitjs.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwlafiiwj.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsbnzrks.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcszqvji.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhpakpfq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gslgzfczx.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggvuafxvl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybterego.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnkhgcwm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gioqtpvjm.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/glputdgxi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgrkinmt.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwjasiig.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmubeifu.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gdqskywzz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwmnhpoh.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gojxmmsth.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gozbbqhbz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gsddyywwf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gcbihbuxt.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gdcccnnan.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gphiagrab.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtghyujvy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfxfigws.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/guozwoigh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvttlule.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzocxrot.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxiqhdps.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gujgdmnud.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwtzbrgl.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtszlymy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/guyvpuowp.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfgxniyko.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoewwonk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gxxgocxlh.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gvuqlqacg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/garzmbtpo.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gpfakghux.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsvyvdcq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gysirkepg.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/guovcwvbl.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrcybfis.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixyajcjw.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrosvhun.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnxjviiy.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybgctzn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggplypzke.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwwthawf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgkytasi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrdxqgd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/greemcral.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/goqhqmsxl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/ghunkxkzp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/genbcpsdg.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gnfsqipzp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gnbrfexyd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gblksdbai.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/glfkujual.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gquvyceam.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gwlpuovvi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgxzxaby.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqqqsqjd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqqjejrr.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/giliycxms.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gobvqbbdl.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gntezhvxh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnuiiked.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcydfbkdn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwonvwwo.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdndpzgsy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/grlffcyti.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkxmjhqxn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwegrelq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gexzsmsxd.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkbuhwvb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gebbedvjk.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/glpeyjadw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gxqusbihe.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/grfgglbep.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gncpnpalc.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmixmvwyu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmngehlrc.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbpnwojz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gphtzypai.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gogvulpiu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlkhdtnj.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gniwsvffr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gumvdhqbn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gicwunpbl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gufkdinky.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gaqkfiyfa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmjugkqv.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/goyikvsag.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gticlnrvo.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/garmpetxq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbgyfuul.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcxtpzel.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gpziploof.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gudgreitn.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjgkuahk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxypxshyr.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gsmapmexl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnflihljm.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gugahrbdy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvcyrryj.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrwmkfrm.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhaguvvy.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gariitbnv.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnhgxsag.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gguvlehek.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gdigrqdfh.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gwthnajks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofcvptts.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsdxmjcb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvuctpor.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpucmnnop.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkyutrqc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gktmlevjb.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gewwdjbto.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleoengzd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxieryde.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gyumdxnih.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjfydlzi.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfrhuun.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxqbsid.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gpkryjcli.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gpdquavru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gudttefmt.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gpgdaldtr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/grxqahjkj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbmnbvnc.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gdwmodgja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnlqbixx.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gqlehjdzw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grshwaidm.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gokbpdjjs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/garqxnxah.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/glpnafiiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcluexh.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaumbmkb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzgwpktfk.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqwpjbz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxntnlrle.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsaivyasw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaohvdplw.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoywncwe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwhebot.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmimfdrp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxvtguzu.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gfalbjdul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowmjijqz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gokequwvr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcofzbo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtpilalm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gewwhlvqg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gposlplmr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gepmzegoo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnfsbzny.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdgcaaxoa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gskqrdced.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavhavql.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gojqvtcfo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzxvqcjdu.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gukrpowdt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvjprufq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrvwunds.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gldakozcg.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmakuccw.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/giswyngdg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuwoxxmc.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbatlwwm.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbupyps.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/guurqxitq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzubllnyj.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gptsiilxj.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsvruvzrt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girrhkobe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwvokmuu.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjxqpmvk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsvbmiwa.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/giqycquaj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsicjzohf.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gplcghuxg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffjpjdoj.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpbcvkvaz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhcbfmpi.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgukzvgr.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezqrgvol.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbookhfn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadocomtn.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gbryhjoma.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/girkusbun.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvpgrwoz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grlrkhfni.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsqzbmgef.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmabswbbr.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmflokqcv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghaoxbxln.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxnldxx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumntary.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gejgwbndu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvrhjrqgp.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gbomfrzqy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxnzuqejv.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvysuecph.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggjedhlwc.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokpnsmun.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvriuhlxm.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsndfxkzh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdulkxjez.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwxdwoax.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/geilsjozm.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gealqgvgr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxpkbfj.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gztffurhv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gggpbldpo.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxmayimtw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcjpecwz.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gulsvnefi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gausueron.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjffqseca.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdgspmkk.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gekavmmli.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gevskkswu.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbatqtnfy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/guzvssgmm.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gaaaqirur.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjzfwesmt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdveniipp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gljcvyett.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gztyaqrzq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzictuttl.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbtuvhod.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghccdrkmr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlmfllt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gxjnbxsdj.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gyxeyqmre.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gdznrpsil.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtnggegc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gaycgndur.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkklcnbbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzyszggf.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjpmdqnmw.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkehgojfa.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyuuncwg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqxmelqic.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/goywahhqu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifwivvpk.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvqllbqxn.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfwswhfhr.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhdpuder.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/glndcujes.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gmefjevyq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guqmytwsg.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gogbhzeye.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujjaexn.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gorvxogye.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghmrklxzi.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gaffgfifl.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtmyufiw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrtdisal.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqibvkfw.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gztwgwesg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhixlmxs.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkjzvdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjosfodwg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjmuqbvyw.sHtML


<!-- 参考信息 -->