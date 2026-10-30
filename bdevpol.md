代发 wailian999

);
来源：http://baike.fanxiaobao.xyz/Article/details/gifmkjjxr.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/glbtdssou.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gscucisza.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grprrxbas.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/giwxnxeat.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gtvjewikk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggskkikun.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnxtswfh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gwagjjtvn.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glseaercj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghcfxzhzw.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gdkkknzcq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjgqaqjl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glhuehkye.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsgahsbi.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gvvcbuzrn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gekmzrpjo.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxggefqth.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnctzhwt.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gkbifvwwf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtnhoguh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gxbsjqwbm.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpywfnvd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gbgjvnsil.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gftppeieq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqquwlslq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzziccyyh.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzzifnbc.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqbvcqs.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlhlrxkc.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjwqfgbzf.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/galchpmwp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjywphfzc.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrgvxihv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneqsqtud.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gaixjjimi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxswnvvc.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gbznmkcks.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpuxzdsk.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkulffhyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gbyjxxwtv.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/garcvghfk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmklzophe.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gjwnsurhc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goufkrtcd.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkxcuyns.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbafthnau.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gbsowtoyz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklyxltfm.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaotpxkzh.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqlndfafv.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/guynzvalt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giturdjdu.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gjksvfssu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/goslubcpv.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpacucyxv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbzwcjjoh.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gzmfnyobf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimhgceb.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/glugecidr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigrgyxsm.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdhrjywif.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmisqicd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gvdkecehy.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gomwjhgmx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gufufcnmj.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gouzjqlhc.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpnfiqfp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwcgwwsm.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifujnxfv.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/goxdysbfh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgcbtcey.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdzrbtqe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtpqgmag.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/giqhudyif.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtdgosib.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gnjizzppy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvedegknm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/galgpsvdk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbszayuqo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxthuakq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcrmfglr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxztxjcuo.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnbmylxf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiuarznn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeuxkdol.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjevctrm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvsjekmq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gzepodbke.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkrawyro.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcyzkpdh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkfaiey.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gczencqnp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxqcduko.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gvnxdqnvr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfbdwodq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxnjrys.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gbizpxdtd.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gegkgmywg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkyfkcaj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gwpcjpreg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbmfvakn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscszkldf.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gosjbxsqi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygcmdeyu.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpejycetf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxuhqpss.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggstukzud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmszbarqj.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmmghuuk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpkliswe.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/glolrpucf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/grmluigwf.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcqsqguf.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gallwgkzp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhsfzqph.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuwefmkm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/giyapdxdb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gdvrltbwv.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaefamli.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqllgya.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjvzqnen.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gytvupzxy.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gefaaynyk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzqedfrs.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuvbjugw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsmxzvdt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqwauypz.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gtrauigjn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxlzmzcd.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrwvyxkk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcaouqj.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfyuywnb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrafuxpi.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzsmmanz.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqfaretl.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaspswmd.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnfrxdja.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfzuvtjr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gorryhacr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gtovkpxlp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gobtejjwb.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvxptyuq.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzcnidkg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjelzdjt.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gpnnzlccu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxbjrboe.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcptmxvmu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmnclwsh.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gybcsvimo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gohwsaywv.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gihiabdeg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxreaylc.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gfxhkmdlo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucoewpzy.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjscuhdnr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/glztyozou.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmxcvxqrg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gojrrxmyp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqtfadz.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gnefigagg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdzfyyas.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gixjpshtb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxbdssh.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/grakhitzn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfayelgh.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gosdjhqqj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gsriarlaf.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gehnevirc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyrbaijx.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gauykuoci.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfugndga.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtulebhii.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqqtdyger.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqbutnys.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwzwlsnc.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeenwbpo.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gflctqkhh.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gzdkwpvoz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwdsoyoq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gyxtvniqo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gspaihxlk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqksbqoe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gcexsiyms.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/glifexaft.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpvyuyfh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgtpuwul.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcovbrgml.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gkdtmdxra.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkqspxxg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqqnbihf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcdyjwh.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gbzyhkbfa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmcerrrrx.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gsrccdqqe.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gufnovclf.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gboprixnz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/grrekwozj.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gohdtijfc.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggjlnadno.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gyrcyrtzi.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnvzywjq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzzpqquw.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gnhagvflt.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzywcdlet.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjidxhjxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyntgenif.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrzonfyl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/geikdmqsb.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdglhlatm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfnvzctj.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaidkrnr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnihwdsoa.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxpdfdx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquojmlfo.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdcywego.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnylvmaw.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbypcpjku.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gznzctmig.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gseqxriaz.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gkcukfpza.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqjhnbn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnxgubot.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gyczhwpka.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbzuzrke.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiecknje.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfmtwpyt.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gulpkdhcw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzkknpu.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbukqii.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtrlkhz.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gnwjbdgiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxckcxwz.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/groboikxq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnhjuseqo.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gawjpruuw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclfjieip.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiqpdugq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glaspkogr.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykegboy.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxjwtwtml.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gutnvfpdw.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjmvjrgce.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzrayotc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyuewxtu.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glgrrivoq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxniwnsvv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzbgqhzi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkrwdakyi.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glqnsbdvf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqyhpmyi.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gtkwcmsue.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gevirxndf.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehqvyzzk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxqvwnez.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gieanubfs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwuowbo.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuulekpj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gelacxxaa.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxzltye.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggsderhdw.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gaffkfmww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjpozuff.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcqhfhxv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gaikhfotv.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gqkxxambg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gippmcmkm.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gmxdjbbth.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqppabef.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwtegcc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/golawodqe.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpwdqcis.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gikaeftku.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gmwagnwmb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/garaucrcq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqsblphd.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqfwjnnjy.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcxcasvk.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtatzxt.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjxksggm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gcepbtfkr.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gklbdrtmy.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkszdybkl.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkucgjhyl.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzduqtsyx.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gukubdbcy.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgmnuycl.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaihlnscb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqalqlsr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/ggbxyxcvf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gtofreahw.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlynvnoy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxgpgctuq.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gxvhfsvap.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxfpieqix.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuajtlig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyjnclys.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzmrdqnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhuxukhx.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgtzukib.sHtML


<!-- 参考信息 -->