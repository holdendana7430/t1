代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gissjmtea.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gpfkmwgsq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gewpagxoa.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gudtulyny.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gnbhndhhe.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gulajnivw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/ghvmpiuky.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gepvgufdx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/grdxqmdxp.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gbethzrqh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gtxntbbnk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gucwbhnnn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gintytntv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gatnurbgz.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/ghahbiwus.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gcyvygtjo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gpexqeqbb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/ghqmtrndl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gmbbbnggy.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gnxiejfpy.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjpmrrrqe.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gzmbowgfs.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gmfmzkfrq.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gzexaxrsu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gzoyslagc.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gtzyyhvoh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gsjuxtzwe.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gfivkwurh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gntlxwvlv.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gpipamane.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gdamvcixb.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gejgbnlub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gkwjgxmko.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gpswmqsio.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzfiwrysv.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gebmsrwwe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gnyocxdnk.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ghmpqbcfg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkzdluluj.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gfwthoohk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/guxlwipee.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gyrqedwrb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvnsjnjbs.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gvmtlvxbp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfayhhdeu.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gqyxlxddn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzdtdflsh.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/ggmicozjy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gugeutzis.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gaxjqxubs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/guvhppudy.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gybccfrry.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gxtwslqkp.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gevzheonr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gqggjavrf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/ggrlgefvs.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gbdeidtth.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/greywwvhg.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gychsntlr.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gdnjwfwhi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gpvydunvk.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gsveamspp.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gnmympiwr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gomvfbwzv.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gleerwipe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gzdwgoalh.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gonxndjao.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/globpelsz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gvvrqkqhy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gjoeusazm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gjffoyzcp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gisjrqrta.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdcpimmzb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gxtobqntp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gbplhskvw.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gfxynhkfg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gwidoqdum.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/glqvgsqqg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/ggbefxkbw.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gsutfarrq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gajgzbwpc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gkwavqqtz.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gxwdqvkjx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gbenywxuw.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gstdwfpvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gnkqkhyjk.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/guoxpzgvw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gnopqchbi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gggxcyxny.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gttfqzwdm.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghdejsqjz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gqmgyuctj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gbnjrbnja.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gbnmbcleg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gyuhzsnex.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gkqsmivoe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gnazebtcl.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gezpxrbsp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gicnhlyug.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gahqzlzpa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gwnxxgmfe.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/guaygglsp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/ghqdsokiw.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gkjjqpgji.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggwokxaph.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gavxwtagv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gtvnoxlka.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gvorppkyg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfopxayc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/glqjjijoh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghcgjjvnk.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gsguttsxa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfzqgpzty.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ghqsxqwkd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvcpuqjel.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/grycqiarh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gntprldlr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gaqkymkie.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/giagtapea.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvsoplgga.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gfysqdxfw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyxpcbzak.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gdxdodqal.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbiwvdwda.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gyvqrykjs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gilmfgkhh.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gvywzcwkb.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gwmvfeawr.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gmcusmuix.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/glpbeiirk.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gylnvtect.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/ghuoncjud.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gbsarhoyu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gglxxoxfq.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/ggtofgisv.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/ggdkdswpn.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gyskwwqeu.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/ghiwdrksl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/ghlmtagom.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gobndmrtk.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/ggujxcnvb.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gowzmhnzz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/giaamwftn.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gqrdiexqg.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwigvpote.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/ghgrmbngz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gmyshbwxi.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gfrynlduy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gwrhkgvvy.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gstxusjik.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzumjxzap.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/grbvlgzpo.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gccooneiw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gfuyifkwf.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gfvterqce.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gssldpmls.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/ggjuidvua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gwssdyooz.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gbewichwv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gbhkeeoye.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gcewnjxgz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gndqsdpdt.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/geqlclgdq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gzfmxwkvr.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gexeeoewr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gagmsrkjp.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/giulgrlca.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkfigftux.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gshfuggyb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gftdpfjje.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/goqvqltrq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gsnxmsmqn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gpycyntrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gblrddvsb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/grihrcagx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gnjhaxzae.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gkprbvdmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/ggkiqqjkp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gilpabsxd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gbbrfyxzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzsudaqaj.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/glckugyme.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/ggskrpizr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcoldgjik.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gpgshenyb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwfnotkfh.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/ggvmaietl.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gkdtwkohs.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gmhqnbloz.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gvsvwjfvr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gkmhfuzwt.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gmyzvuzil.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gxupqktir.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gsgyyrtap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gbaqbcnfl.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gviylbhfz.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gekudpxyt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gdfmusvbm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gtwvjrcya.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gdrtnomtd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gizdzdikx.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gbgsupnqo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gbubvtliy.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gwhbnjvtn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gpwwvlvte.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gdpceidew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/ghawkwwod.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gqlerxydt.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gqmmvtllg.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/givfxvtio.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gapbabprm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gnxdgmjew.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/ggkswpwzh.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/ggsmbrbev.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gleceavqi.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gstpevbie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjgeycavx.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gffyjxfbg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gciykoivl.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/guqkcogqs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gbfyprkna.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gsrexinwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gikikzgwx.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gamkejzbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/glxmlpjjm.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqgstwabh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gorxmmopk.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gyzwlauem.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/ghswylglm.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/guujikhfu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gjbezxxfc.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gbumdbmkh.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gstjfnmfv.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/galvpvbpd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/glovdkllu.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gcrczhbje.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/glqxvlwdb.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gyhbtlinv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gzjigtsvt.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gsitrztsr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbrmzhjcr.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/geazbjftv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gzxlxzssd.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gwubfjtgz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gmxgjeowi.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/getpoykgc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gktzuihdo.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gikrrglua.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gadajbyqr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/givlcfave.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gngpcsqbl.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/glxbtyqfv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gftlzecbh.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gffmsvsit.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtaupcalf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gmupycxgh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gpfaruuwc.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gxcfdgkkd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrkxoyq.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gwavkvnej.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gglalpzer.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gdbkkcjyb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gvmoupzga.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/glvhzikph.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gjvhlgxvb.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gkprzaiyo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/geswnfiid.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gaykjrlxb.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gsudddrzm.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gdyldtrfk.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gocjhtydq.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gkdumniju.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gthdirhjc.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gqvaxnuqv.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzpttyxwo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gbdnhgogp.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gkihzdmcj.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/grfxgxedp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/glykehtei.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/grwdlrfsd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gwyhwzogs.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gcjiezscb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gzvmzuxlh.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gaudlqdfq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfofxgnsi.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ganlhlwuy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwqbtznfn.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gqmakzxwu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gskmzlkgl.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gwprxtatd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfccfwvbr.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gpaiphsea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gvzlxaxjj.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gmewubfjt.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpsungmge.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gmmybtbow.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gslojeazl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/guzstsknb.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gbydwkfbf.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gaatiifuv.sHtML


<!-- 参考信息 -->