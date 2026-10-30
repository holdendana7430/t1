代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gyxmaarxm.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gjpyxpztn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gjdauogrf.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gjpnywfjz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gwcawqujn.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gaynrkcqr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gxajwuinn.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gjcyaovwc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/glxuxbmzq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/glbytznxb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gchwlbsnf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gaxmkmmgr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/ggbqqvvcc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/giamcuprk.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/getzkwtfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjgiixley.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gfqyldehg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/ghwniygvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gcyctnfjg.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gnhvcdrxj.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grzbuxftf.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/glsprzyzy.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpkdajkde.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gfyqphjab.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvynjrtkz.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gvejjtwft.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gebtmdfjr.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gmgrbumlp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggmrfpsex.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gouuqbraa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/grjqaocsn.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gukfgdwmc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ghhhzgfdl.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gmpfstysh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gzcljsefp.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gasercrwl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gcsbrnvld.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gdhigmgyp.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/guyrpdzkk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/guvcmariv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gqrfcmvtq.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gvsjtrsee.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/goluovfjp.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gluwzdiii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gufbzuyll.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/ggpvxudyp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqoggaqrr.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/glaggvdke.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbhwytgwp.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gnhqjngun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gdkwgxudx.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gvpbpggne.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcadrtp.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gvrtcysbn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gheaktvvd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gkyinsubw.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/grziadyig.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/ghhkqeeak.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/glzkpsjop.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gcaczrale.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gxvpesjvq.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzxowauwq.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/guhgqtpxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gbcejyivf.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gxtpbccdg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gaaslrbhp.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gpxjmgmro.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gijfizaed.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gkjmyqfsl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gaqxnjtma.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gaswlusdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gzjmfmdil.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/ghoviaspa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gcndazeal.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gdszjanzr.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gqghfnjts.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gjlgvbnmx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/grcjgprfr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gttimgwpk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/glhmgjwbo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/ggmndmako.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gbinjvggu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/givzixrup.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gdslytdjx.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gkgssdzob.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gwztzicbx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gdsgjknse.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gfjstulhd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gexurcdkn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/guqdsuevx.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gfilzaaiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gdfbxxejo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpbupzbbk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gsdypgled.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gbstvlwtc.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gagsnpvsj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gxilnatiq.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gqsjuhwsz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxdpopjko.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gvxxnjnus.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzeagjkfz.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gbixyktha.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gftpepdhg.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gwujqsklf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gtcmxbpqj.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gbaryirpo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gxrnmzydr.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gxrffjcjc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/glcqbcdfr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gbxpkgffo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/ghldgomzq.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gfovcjzvs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcytshprk.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gkzpogkxi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyrnezzhy.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gjtipfqgd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/glqflayzb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gbokoqjtn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/ggcngylye.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/grdgcywbt.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gqpwkmrvc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gffpfdfbs.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gisbxvqqc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/giuntcbvo.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gmhdqansv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gziefkgkb.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gipafunqt.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gnsdpjkhy.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gckvfpjcw.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gilhsqovw.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/ghvecstqi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gzeldaedc.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gopwgeioj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gbnrwvtqh.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gncmasouj.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gdpcdktwl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gyzvhzjfu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/ggpkourkp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gmtexohyl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gexsypptt.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gpgiernko.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gwdaqnkcy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/giudedsbg.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gczecmirt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geffvzysv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/ghqzdbbir.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gjgkmcbzz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gvimdwzcr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gwdkyhkpx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwnxmfvrv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gyizbflvi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gebphdfyu.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/grxrnbzbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gnvfokxof.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gpwlatrce.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gzmvgppdr.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gamvnciiz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gylckfvln.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gtoiyyont.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ggepvnoki.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gaojfyrth.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gstwbbiha.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gccaipkje.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwsriwevj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gidetdhzt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghsposczl.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnbezdmhj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzunwelid.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/goiqpsuxg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfyrkumir.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/groztvmul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gwfmkzukl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gjcsurhfl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gzjvxfdtn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gansxarvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/ghvvbhcql.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gfvevapxi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gbpdpuqqb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gmsuhmpiv.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gitfcpjpi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzjnuiuvf.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gqxxqntkl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gnlizgwmo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmektjtyn.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gfqcowqjg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsalnbwcs.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/ggrwcjmxq.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gsutqwqhy.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gsspcotob.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gqxqktjnd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/goatlyorj.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gxweotgax.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gzbprdxxd.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gctyksgbg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gvnjmqyrh.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/grskhlaol.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gbubpgkbf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/groeyebtn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gggwdlaql.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gzudgxeyy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gzrenlsxx.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gbbxnyfqo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwpjkelou.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/ggslmpnzq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gusfsikcg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gyfeoffnn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gifypgqjq.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ghaedgmuo.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gwjodagnv.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gbdphtghs.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gcxgnjdpm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gtbscqfrs.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gaddotqnf.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/giozgmiyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzpfojo.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gghoypaaj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gbygxotdv.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gaordslqu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gabbamyrp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/giyiirhbz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gninkqzid.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gkhoqetke.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gljmxeaix.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gylukbhbw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gvsitposy.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/geklrnxwm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghizsazmf.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gugpbxnhe.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/guqhkluln.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gjtbxyhiq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gbwwmqeje.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/guojdftsr.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gflmuecpw.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gwklmdpkw.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gbvjcngef.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/giycabqme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gdnlxebno.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/grybpdsjd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gmbrmyzlm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gwxsykhqj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gjwmzyiag.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gcavfmyjd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gxyickzuk.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gwwqhhbgx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gictaczph.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gzkhvbtdu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/glgmgaxkj.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwonpuutu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gyqggmduu.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gvfumzmtj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gomyripyy.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gnenukljo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gmgqcujlu.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/ghlodpofb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gojsxnfok.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gdcsjhrti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gqtulsayn.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/goptkkkxi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gcmukbyor.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gpitvooka.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gaqgtsoas.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gsjsakdux.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gekosrvpq.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gcirllyri.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gzdxjjcim.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gbrhivses.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gpzavwupf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gbdtlncxm.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gpvprwltm.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gsofjjxjl.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gwmmvrfdw.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gwrirkvbl.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gmlhatjmg.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghbeuklty.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gsvzjayff.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gcvradaod.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gyjxndqmx.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gbxibxoby.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/groeykdxs.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/glghzzxpb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gjcafhgep.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/girbbepef.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gnztozqvj.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gtcobmgij.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpjzrxtgs.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gwcqsjzqk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/geidafgug.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gpijgoivx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gsfqkcnbl.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gduzbtroc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmdauuuau.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/geplkhygd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gqvfcmfko.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/geppdlxna.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gigfiaiha.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gwoukqlec.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/ggfozjfqe.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gnpfignkd.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/geohhhyfm.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gaypvrryq.sHtML


<!-- 参考信息 -->