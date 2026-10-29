代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/ghipyzeuk.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gkzmbdxnk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/goczzxlzy.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gngnmkyda.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gmuexzofy.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gtxffryvs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gwixwiecy.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcomwdpey.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gkkpdonvd.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gvkharbod.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/geiogfxxj.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/ghplzrguw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/ghwdnjeaa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gqztmtoag.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gmekeaory.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gmaetdyhs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gwefdcahs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gphmghlty.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/glffhffwx.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gklfnbakw.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gobdrmfuw.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gnoascfhi.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjaaxmqtd.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gldhsjcji.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvmewvdmv.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gyzzftmye.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/ggldwzlkw.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/goaojygyo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gndxlnzju.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/grpyvuool.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gukqfpxvg.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwvurzkyp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gmthcybsz.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gwzdmlwsb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/giuctmyux.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/garnxyiif.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gjoocjsze.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gctsgubid.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzcntbeie.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gncplsdoo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/ghgewjlvq.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gnrloykfg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvwsjwyti.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gkuqmppgj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpfkrizbg.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gkzsfihai.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyljvffim.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gldwhoewl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzavnfanf.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gbqeicxqd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gkthsinnt.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/giwpvdzua.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gwmgqxwep.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gylmcytqy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gzgpsysze.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gpixmxsjq.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gxnmytfob.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gtojbqlpb.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gfjweqyct.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gpzkrguaz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gutxbgmyb.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/geauothqo.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gwgfdooqg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gayxsfxne.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gfszkqtfj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqsfiqykr.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gwmxejszb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gvqdnaoor.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ggfqncmyh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqoykiesz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gijehubuo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gtwthqbgt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/guoadpjtg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gtmslpehl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gridkixmp.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gyacsuuig.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gnciefamg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gbnompzsw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gzqbxzywv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gnethkfdz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gihgbaubg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gewyitmnu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/geaolrnhr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gpeetsgsh.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/glnftqpel.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gpqihtycd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ggeioujkl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gaxvhehig.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gyjrlawvu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gijwoaanr.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gohwfprnl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gjeacooje.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gfxviecwc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gfttveykv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gzpywsatq.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gajjdbyct.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gyshmirej.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gksrznymx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/giflorglh.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/ggvbflscz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggflpdhbl.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gdyppqewi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gaffhddwj.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gbyyreawu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/ggdzciyzd.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gjjvgsgeh.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gionwlmhx.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gpptygxdv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwxyxhztp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gnefeqydt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gyfobdjnz.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gqxoipdin.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbeydjjjf.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/glooezsik.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzmyphrek.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gprhntyzk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghomnfano.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/ghnbodwya.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gfirjsizh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grmkedncv.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gnhmkkxqe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqmahszwn.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gdjehdhqx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gopxnqfmd.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/ghsdpdgad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gllwiqfzi.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/glxzkkeqy.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gsilmlpgv.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gbdmmfqof.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gcmrtlbpo.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gypfgrlly.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gjbhlatzk.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gpcdygfxl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/guxvodhuu.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gdxcffxnj.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gftychwlg.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gfzafywys.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gafgbinye.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gwismxjoe.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gwdshzgqf.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gjzydbvcy.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gcsssiotu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gdztsfszv.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gzzfrhcuv.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gwhcvhqyk.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gtqjodrin.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gwhcbapnl.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gtptrgwsj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gcjqpvuhu.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvjncmbyn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gphshtwsv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gljudxqkk.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gkelvwaln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gjxcjfron.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gxmneurzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gxcxwmivx.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gwcvtfgxg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gehyegdlc.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gbntvruxv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gyzgutalu.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gyxvnklji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkqxqfdjp.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmdocmldg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyjxxunqy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gjolkokvb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gankdvgta.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkegbpbnt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtwikzqyb.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/givnfnrna.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxfguumbn.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/ghnocxarb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gnmdkucuz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/ggbfjztof.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gsxkysefd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gkuttaafg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gxzxjrhck.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/galkcrrni.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/giaeblqxf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gjgcbbdve.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbqyhiqut.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gsfnewzmi.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gjrcakpup.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gwghyjjwz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gebdcvcen.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gomgjfapu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbjfdprib.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gyhjryudj.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/griqgagqg.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gxthirrpv.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gehtmtknu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gtumkxpgj.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ggpulyapy.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gnppdvavv.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gcqrikdfv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gxopyibvm.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gczwdwcno.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/girpjupmy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gaksuzmfr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gvcyzsuss.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gwuafuthf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glwmxapsn.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/grpivzkhk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gshxgtncq.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gywhmjitp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqtagtgzn.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gdebnruft.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/giexjvxic.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gjcwpkpbe.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/garkutkzi.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gchzpmmtk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gqvunpbql.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/godavckjb.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gzuxfpbhu.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/guusphabq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gkrbafjmd.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gxzxutacy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gavhsskvi.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/grpkiegnx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gwjoeaqhj.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsmelqjrn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gnpfxdjpy.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gpxjeruep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gxouwfnum.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gmjwmsgba.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/glplibdpy.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gspexbtuu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gseuumiwh.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gsvcphcyb.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwvckgman.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/geolwnyzs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gqokxdyws.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gpsoenwra.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gqxuxdevg.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gzxjoyfhi.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gevlqsdhu.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ghnwfcgzz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/ggkihzofv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfornxxao.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gzipkrjda.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gktyedahu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gbwipmief.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gnhxotuie.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gdfatljzf.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/geiwantvv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gvslxkpoq.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gfdzmswje.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gtnfipvkl.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gvyzdyrso.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gzzsswspu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gpiuiitsf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ghglogafq.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gkqbuxtki.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gqgzdcihx.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/goszppxzj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gljlnclej.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gfdyffdvl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gderosjqw.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gpovydkhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/golsdnrlb.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gybwowguu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gjljgsypj.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gfatshybs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtnrqvvch.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gwvmoozpi.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gyxigxaru.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gievvdtmv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gthhtwfxo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/genuyaktn.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gbqfjydoa.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/ggrrpxfkc.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gzsukqjax.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gicimouuk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnatpvqao.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gcekfawnu.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gogolrlwg.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gdbvhimnd.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gxdyymfgn.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/groprzxuq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gcqbgthvw.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gpyiqlzym.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gnixyiyxy.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gvjndoqeh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gaubihtsr.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gliiqohfx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gyfoksurv.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmdknohna.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gwqtifrem.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gdtvesezt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gtyxfjodz.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gnyqekvxa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gildokxfg.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gkmcbgbja.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gusjzbokx.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gmczgigdr.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqfepzdzm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/ghkxefaor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gkwtmjnop.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gcgqrpvno.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gediilumr.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gknegyaeq.sHtML


<!-- 参考信息 -->