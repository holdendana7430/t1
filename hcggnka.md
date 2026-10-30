代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/ghmfmfjtp.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gulmcryms.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gcjfnyvjo.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gkoexdhrs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gkyardqsn.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gwmwawgrr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gmllkchpe.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gqsiplwon.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gudsctosk.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gbgsziukz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gsjqwsqpd.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gfjbnwkcp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gwadnjojp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gnbsrbwjb.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/glvkgligi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/ggktfjumh.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gbunkboyb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgoyefp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gmqzojprz.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gcveqycxx.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gepyuovgm.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/ghyynqlvo.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gextrninf.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gafgeoqxz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gxgktqjtr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gixbwledi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/geiurlmgd.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gpdyejkwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/ghahvxcwd.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gtbsgbzeq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gjtxpfgog.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gqtmxzkyd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gloklnuop.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gtnzaiscv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gvecflggv.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gvgmqqxba.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gljfkhahz.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gfnbzldcw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gprubswya.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gtmzhrukv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/grognbvph.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gmkzcaeti.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpqelcgci.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gspurwpyz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkilxmuki.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gcuakkdpt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbtfqtphh.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gokwtnojn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gquqxinhe.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gdzjikxai.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gmnivtkci.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gmmtrsjuh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gtulyvxkt.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfbnfvmgn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghbdzekvj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gjwrlbdmb.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gnwyawhnn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gijchdyuy.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gpwwekars.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gjplxjbrl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/guvyollfc.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gezotvrch.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gjhyffrca.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/ggfuniips.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gbjboatve.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ggmyinmcy.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gwduvmtyo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gyysqhvay.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gdxxxmfdz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gxgwruuts.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gsjotfkmb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gmtgvhplp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gvtbzhoiy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gpvfkpnod.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gfjvfjsbn.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gfpktyckc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gjrqiueqc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gghttptft.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gpjwcttkw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/ggtkmbscg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gsioxgvfr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gjvyxhgom.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/goeqnftxy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gpmyrfbxy.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gftolaksl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/geyjmbhqa.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/ghhughxcp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtcbkfgqm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gjzwnhppo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gsqalnthu.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gmswsvrgy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gpkamcqtc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/goieezmzg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gkdwaluhm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gyojjxlhs.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gpokqkkto.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gtwmumyhj.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gyotluvxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/grluzctbw.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/glzofuiyy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjijmdbbu.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gxbbuhwti.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gzqkdbocw.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gxzjljbso.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/goxckfesz.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gmhxfqcsx.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/ggeoljoxm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gfekhbhud.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/glatppwur.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gteagntza.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gljgmysat.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gwivjcebk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gagqroxfq.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gbwtkbugt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gytqueebt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gsiouuhfe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gejrnpgkd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/ggamjjunc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gpfwnxdlc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnfwhrloz.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/grrbklydo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gaqozczxg.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gyxxecqek.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ggaxwuocd.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gpmkaiyfv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gfjbchjdj.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gnromkulb.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gokttsjzm.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gkhxwmdjj.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gdugbnutc.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gdfcywrle.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gfxxwtpzi.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gxhnihhia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gecwoaukj.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gfrlwuinj.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gqqllyjyd.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/grkatpsug.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gjawsvrne.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gtedagido.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/ghgpbmgzu.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gdxqdoqrj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gxtbpfacw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gzvlorleq.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/geqflayhj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdqiwrciq.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gzndsnaby.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gvxmyuphv.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gdbpgvgde.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gljhgripc.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gdvftjwdu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbkgppmvh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/ghgkdsgvw.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gwmubcion.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/grajxcgso.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gsupnnroi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gzcseshqc.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/grsesense.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gyfvjtago.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gxnrfbhhx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gsxjdfnbq.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/grrmtrdee.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpkhgdtq.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gmmgfpvro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdtsoxaow.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/glkrmbnnv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqfcxjhlg.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/guoeanbpr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxyfqwfvv.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gjszhfqcc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkxohrmdp.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gyhebqybi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gvrovihor.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/ggbdgqsvj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gpetlkhzi.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gkpdorbei.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gqpkydhwo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gtpvwwwye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gykoqcqub.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjpgmdulw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gmhyktwvw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/glmybfpub.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gtlffrojr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gpxyxiygd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqqngrqhv.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/guapfwbuj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glfdkaeyw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gwddslohw.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gyracymtu.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gfwvqlplh.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gsfaluttn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/getdrajlu.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gjngofbkm.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gusxbkfcp.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gtgsirzyx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gifhhxidi.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/ggbekyinb.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gskgmsnga.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gmnzhihsb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggvqzxwui.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gfmcrvbez.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gmglsnprb.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gncnecuus.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gqlktjmkz.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gglstkopl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gvgvibrff.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gezvwraki.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gcniwtoft.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gknvkrqxc.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gfqdqywrl.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gmvhmjucj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gwbafefll.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gejbkbgwg.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gezemebuv.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gkiiysrov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gjflorvrt.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gvatenfac.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gtutbqhyf.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gpykllqyc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gsqhrwqws.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjloxbkcj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/ggrwqwvpr.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gcvpukbpm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gshfpqaxz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gqbxbawnm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gpxfpceaj.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gvuclkijd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gtuqxaguy.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gbawaznsu.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gwlctwznr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gujzwiskc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gdkszuozr.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gudzkoukj.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gogztxpge.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gkgboqwcv.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gjegjipda.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gyxbbxzji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/ghlbrgeyq.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gbpjgutfs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gzsszprfr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/guoxgebej.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gcmxqsent.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/ghovccfgo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gcrbihpju.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gmorhrwxd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gytcnwray.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gausqgyoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gfhsplfne.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gdubwkbqm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gysvnhtff.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gjgvderrj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/grzmrbdiw.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gczkfuicd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtkybczh.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gtskffjix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gepnkijnc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gabnunkem.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gakidyvrt.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gfsagmwua.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/guleostup.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/glpgnkooe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gslqigddf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gwrqtdxgl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gewlyazou.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gjhosqztz.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gzpshdakk.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gzscqatwp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gqndlzscs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gewdhqwcu.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gmjhjyirb.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gssavozow.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gwrjhuswh.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gstspjyps.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gimhofofr.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gvyfhgcck.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gluqnwhxb.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gkhczdkct.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/grrsliqzf.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gtgzyjoeb.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gifgcoakp.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/ghycwzbtu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gkgbthgzm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gqknueedl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gnnmiayjn.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/grmdshszv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gpvclvxpg.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gyftlnugt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gfywlbmgj.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/guofmvpun.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gmtljkzud.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/geqjdxvpg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwuzbkdts.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gogcslmqb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gnhixyumn.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gklodqrvj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/geajmjdhy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gcvinptad.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gqpoafvgw.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gtwfjxtbr.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjnthrctr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gxadtthze.sHtML


<!-- 参考信息 -->