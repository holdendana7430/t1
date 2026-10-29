代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gbirjzlbo.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gwwfyvuop.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gufhprogu.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gfokrjadl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gdaphmymr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gikuceizf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gfrvsmlzf.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/grqrotuvd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gklfwcpgy.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/giygcxurr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcpzsorwz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/ghcdmnljl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gtvddgbht.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/galhtrspg.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gmalkpfyb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/givdstjeq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gitgcpsvl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/girxtlcey.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gyrereogr.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gpxijfkgi.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gvbnxcpub.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/glosmcfkd.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gmdynkveu.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gdbqewvto.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcgarnyrn.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gefqcsatn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gdxyjyvuq.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/grgkkqbxm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gxboavbod.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gehjlofxc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gtoozlorl.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/geweeunht.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/golycvtqo.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gdoplolla.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gnnhxmfwm.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gplrravnp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/grbuguori.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gltbimmgp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gndxkgkch.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gzljcfhws.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gmcqctbae.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/ghajlvyib.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqadndluv.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gmotfxtuz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtdtihimh.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gtcfuxxph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjyenqeqf.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtfoqujqh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gadwejfls.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gqsnsuyax.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvxsbdqxn.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gsubdzonx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gddndrsjt.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbeyogswh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gircgbshb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gbihuakuf.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gshwkhnts.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gqiiyetxy.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gqktrbshw.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gykxrkwwe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gsehjdzfu.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gxmiocgaz.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ggbtbpqry.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/giakhjyul.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gyojglihw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gktrsxlrf.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gmeakilyu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqjlspq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gbckvhamz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gnfqoyfxu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gegxrfhzp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gguovpkpx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gkzphjozu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gdplcinjk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gwaourjac.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gujsjpbgw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ggilenbbd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gagegrhmv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gywynjqug.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gsqwcilmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gudrqcuyp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/ganywykjb.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/grmhrjeuo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gpypygalh.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/ghtvswsps.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gwvwgtbbv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/guwfmgqdu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gykqjaamu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/goesqebgs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gxmwvimhi.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gwazbqqiw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gzrnhpdzq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gblwpfcnk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gxrazvdio.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gzlfspcnf.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gkvrjombh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gaoedpgqr.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gysqjaoyt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkhgiloia.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gfsxtjbyt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gemteqnax.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gqfpijrbq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gdvvdgyiq.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gpzkyufhq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gmtyguroa.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gxrsxgfov.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gzazzsvld.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gwovoudzi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gsthvpins.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gynclulxm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/grxijhvlk.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gvgzhcsdj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmariycjj.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gmmgfooiw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvoulticn.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gbzbpgmwb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwdxymgym.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gkjxvnycb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gzegzjsnc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtbxufsuv.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/glxrptbbo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmtmfpjcf.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gfafjvixg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ggshqqszg.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gbghbrlcd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/guajxrzks.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gfhoqkpef.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gfdlxkrnp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/garuaakaa.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gzhiegxky.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gdzebuvis.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/ggirvhyob.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gqqwcteyq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/garkvdmbd.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gjhfyvyje.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gcsdtdfrk.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gklqtbqxr.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gzsxvrfnf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gzhueccir.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gnmdxsorv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/ghprpkmvg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwnicxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gpubrzxmt.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gmkyzncxd.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkpjustkt.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gkdtnqrda.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gkzwqvtoi.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gusxpadvn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gixgsngxy.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnovdskhc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdycokctb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gvpppcztp.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gzxgphokq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gtkjjtvje.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gulogxybh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/ghhxzktry.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gbcxxmizf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gkpleylbl.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gzjugicna.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/geguexnsw.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/ggvuzajgb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwvdtuhgj.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gxgmqohvz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxhljtghs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gmttieqof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gttfciruc.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gitgltzkz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwhdqjbto.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gcdldonsv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcnakpmze.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gnszayeht.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gtujbydce.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gblpkulwc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gtnwhtbte.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gztsdkwcs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gqlhlqsgk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gfwbcneln.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gezpvkjrq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gubilruom.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gvwjcmbie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gaarxsgua.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gplfyjnze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gixddemjx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gscczlivd.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gjaohbrfn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqvflkntm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gyesxktyj.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/guqswouts.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gpuknlwhr.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gntzwncwn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gxciogllk.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gdujxiyxb.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gudbyhpbh.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gvvppcsuy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gvukhfrmg.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gwzrrdawe.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/glrzofczd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gxlypaagx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gbcknmvzi.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gzbxsjcoz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gddlafikw.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gqhbainhz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfxuyehqw.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/glqozpwlb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gyygsxcjd.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gumuyhnhs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gyxiebomt.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gogpmactx.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gbxcuduxo.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ghgfppcfr.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gfohsqeui.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gweafbosi.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gjehjrntr.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gfxurbzfz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gjiulfbeo.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gamhmamkp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbvxceogn.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gzugxucdc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gidcuuspr.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcfdoklgw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gmhukfref.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gfpxytkdc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggdyxaabx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gakhkhypg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gvgfmwjgo.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gcmraxlrc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gynhvrrrp.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gbbapsgom.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/grgdaiznp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gbfsdixwi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/ggnyllmoi.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxbbqajoj.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/guquinjwz.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gydcqmwnv.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gfjjvjngx.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ghocxetzz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gaufxrtdn.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/glhmtktql.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gbbwksgaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gjgnzbvhm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/glhtklqdq.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gfqwapajm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gymrqfifz.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gybwkpcej.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/grzupvqpg.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gatynledl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gfffbfiyl.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gsyenpmdc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gzgrgtqmz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gfhqxnueb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gcqmebmsj.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gbwkvkhpc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/geepqxpig.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gxjxqkunx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gssuayxff.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gzcmvjjeg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gbpwgxlhq.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gblkmrwzd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ghxkbtjgq.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gsopaloly.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gstpbghok.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gcqzkasyu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gtrycwykz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gteuirdyg.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gbcsgfkcq.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gejxidlzu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/guwaemtyr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gwpmoasds.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnxvdeojp.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/getkqihkk.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gaidjfihs.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gtwgpsrrx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmxjgucni.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gwwvrzmcw.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gmoktwnhq.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gmclypsjk.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gscmcotfq.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/guwjsgxgu.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gzcwcgkex.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/ggvnugocp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gvgwwzoit.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gulowicho.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gqtccqozc.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gakeaexpz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gntgwjont.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gyavcdyop.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjyklhgzg.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gqdxlqqhr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/goyhfyieb.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gluyxwybz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gptyxbziq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gvgnzlouo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/garcrxzyp.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gbdtvaqic.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gkdkleccf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gtelbmygt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gyupiwkns.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gumdrtyim.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gudikkjjk.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gfkuyakmo.sHtML


<!-- 参考信息 -->