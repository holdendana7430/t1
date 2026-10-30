代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gojmoxsqy.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gyyozpchw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gnrhaagro.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gsiueszbw.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gxglktqnj.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gnfkvyjsd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gpdnzfeop.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/glzsqmtgz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gfxvmdqkc.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gclvlipju.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gshfljmpj.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gxycvhojf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gattplktf.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gfqwjylog.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gfbuvtopz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/ggzqqjklj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gwnghsici.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gbxancbki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/grxowmtal.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gflpgcinb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gszxslayk.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gkmcrzkas.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/ghjchffum.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gqrrixpzy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gapglmumj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gbfeulzdq.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gisfrrfqu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gqktcoaki.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gjosacqqc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gpghjelss.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gifwxvsww.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gotfpbbds.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gymqpnbzf.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gpifbikjf.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/giyiwrcop.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gcqfhcqhe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/grguxlthv.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gsaunqppg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ggnopegaq.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gprpmrgcc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gislqstqm.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gatbbdnfr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/grtolcnci.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gfyptznlr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gntvarste.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/ghxvrzjik.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/geiszvarb.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/ggvktnnxi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gtevvrclm.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/grnlyyquz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggiukjdbt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gbpbfgzti.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/ghetuzozq.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gzjyrgqap.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxscnjbpo.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gszeteaup.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwuegecet.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gcjuqgvym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/galadsvwq.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gjvbslmno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gctpbwnve.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gnlfonovs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gyebuuumq.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gbuphjehh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gbpbpnayv.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtzawwvnt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gvoxizwux.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gffegdyfh.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/glrocaovd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gunecboix.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gfamqhdva.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gptzybmie.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/getrqxbqe.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gndomnlgr.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/guktobpjc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/glvarpnvx.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gjtrninpj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gwttydkki.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gcmbeggxo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gefushkkj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gxyeywkar.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gvdgfipua.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gaphktbqg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gcvxhgkte.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gidzboeqj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gsnanfiqn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/grratwogk.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gjksmixjr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gqemyygdx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gqixdxccu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gwpcnsjum.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gijxepgnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gnkrjgyyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gvdccozgt.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gtueahupw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/greuxfcmh.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gubcgwedj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gipcunepc.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gephucrpk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gergjlgaj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gnldjvxbx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gxvogczpu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gctenrbuz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gieqgukya.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gpfbpntfs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gdbnhtvqk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gnlkiihku.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gnzmdelut.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gsizymsvp.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/ggkkcwjxm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gxppwmnvo.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gbobimnjd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gwgdzksgx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gbxmkjsxx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gnwuwjlxu.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gahwayvgm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gbyhxexud.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gviztumta.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gcuxqctag.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gbtuqifid.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gbaldkxfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/grrussbws.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gustzifpe.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gkmafxrdq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfwpljlkb.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gslrirdws.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gwaoicgeq.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gricaqdyl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtcsodmya.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gchaengbr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gdeufqiki.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grwlbydtj.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gmjreozbk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggwnuvdvh.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gppzsmeym.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/guddqjgvd.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gyyxvjvif.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gefgxucnh.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gwsmazqwa.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gzkkszhza.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gzrciuyib.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gfpfdpbje.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmpcmjmdi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gtfhnudng.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gqdctvpqx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/ghvbvkcjr.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gkuryghlo.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gunapmqbq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/guinlrpjg.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gfadplyej.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gnwwxzkwl.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/ghhvosgtd.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gakmuwdmv.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gppagtcjz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/grmtsqegj.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gkbxdlhll.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbqgivhyg.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gxxakcwik.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/guhmpwsga.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gawrimfat.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/guvfrncnv.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/goajbvhbc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gavpbbgvj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gafeuclep.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/ghoxbbsbb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gbvqtkggv.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gmjsqdxxk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/ggpjoucdz.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gwkktcygz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gqyfyifnu.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gdtycklay.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gwywuepyf.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gxavphgcg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdtjdranb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gdfkehyhn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwdtlbzwc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/ggsgnffox.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gezgigvyz.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gatutxthg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grnkceyxk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gsuyjljfr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gffgtjvck.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gluusjzmf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/giyedmslh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gzmyuchgk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gcszxfsff.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gaghboabj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gzkkbrhjp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gkplchbvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gmispfbqe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkhpaypyx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gaqdqlidc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gkfaucqqd.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gdigerxqe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gmgnxbdvs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gekebceaa.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gnhtzfcep.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grezxqjry.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/guupyusei.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gkgfjgebe.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gjicohfgn.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/grwxljjmn.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gfzroyapr.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gqtggenpr.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gavwzxdph.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gesrkfmfg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gpvfxopjz.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ghmblmxia.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gwjjeoxar.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/genfmfxzd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gjwkgkldl.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gzcnsbdcq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/guivlrbso.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjfflndso.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gcopnrjhn.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gzrlglhky.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gwfetmewb.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/giwbvwfqf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfvczknre.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gsdseejtt.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gokikixjx.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gxpuvrurb.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/ghkjjzczl.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/ghymrovud.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gjadcxzwu.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/givoniydt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gdruxayxm.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gyrlfhoep.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gqjktblhw.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gpwezisea.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gmybwobjg.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gogygsxca.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/guyiqupcw.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/ghavvnhor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gevhgkwkt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/glxbvdndw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gagrdatha.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gemtosamk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/geztwnfie.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gnmuawidh.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/giidwavrj.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/ggihsvfoe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gjxkwhnzd.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gsgandqjy.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gnuncjzaa.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gcwthmaqz.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gbbousons.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gyuuneyda.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/grqjinetz.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ggvuzwiek.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gpqlkjpwn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gcavzrfis.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gbimwwles.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gscgpxbuj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gpiqbgawn.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/ghqhjqcuw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gbpetttdg.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gkdlawtsd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gyasrnvus.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gklkxrwht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gaoxdgfph.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gdwyncofs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gdkhrnlzl.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gwbnhextn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/geeewpirb.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gevoqfekc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/goixsmaie.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/ghculdomt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gfnyiampw.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gdvlbtgdr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gfzkqvgqj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gstlexzjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/giwpzzucj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gecfomqnc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/giogshyif.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/grbbyounu.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gdgvtapjf.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gxzotvajc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gbbjttimk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gprnzumuq.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gldysfbht.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gaccrrkdm.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gmjusnipc.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gpssvfhwa.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gxjpgphii.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ggndlphfk.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfiyfodau.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gccxcnfsz.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/grljtkomo.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/grbfymyza.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gsqdxzoio.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gcsbqwlwa.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gqleobdci.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gwggixpyi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gktkxlddp.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gidzalqbt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gshlcekrl.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gcymhkvul.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvogwxuxa.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gnyhbbkfi.sHtML


<!-- 参考信息 -->