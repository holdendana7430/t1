代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gbivzvdov.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/grtvgewte.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/geifzyymk.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gmockbxxn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gkhaazarh.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gowkfatyx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gfqqkepid.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gljdemzhg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzffdngth.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/glenxhdic.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwpkvxblb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gknmkejmt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gaagmnwad.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ghpjirtjw.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gqzzgxaeg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gshgcpuue.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gflnjjdec.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/glwrubses.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gixopkvww.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gjkwfpqyp.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsdvjtktb.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gpjscrqpg.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gwcdaxhts.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gzbtjznsq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gluwllvqm.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gyotynzov.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/ghbfksbxe.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/guhbvflaj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gbjhnkbiw.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gtanxjymr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gfhdwrnpj.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gqsdfefoc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gevqrlzro.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gontlkytn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gncwdxati.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gxnamiept.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gepmhhzoe.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/geyjqfyqp.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gszqeioqe.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gqdnbeidj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/guemduiwy.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gthoxnxqh.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gepufasca.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gmwonxlbt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/grhtmaakr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gwtszxydj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqltysqoc.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gfunhijfq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmjhpulau.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/goqnedmkj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmtjztsml.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/ghgjptrqp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gohtcwvcn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvmxkpiel.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gtotsmohh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gxsbaponq.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/grbruzxzv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gzpwhveii.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gmzsizlvx.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gyutiylsz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gcvfknemq.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gepewvume.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/guubhdvjf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/grtbsrrnh.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/giekyabem.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gjybmyxaj.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gbfsdschk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gldbpbntc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gcwfrtbnb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmywrsakx.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gnuteauda.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gfsixukdl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gikiukbxu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gqqpcirih.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gdnfucsmx.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gmkvlmcuf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gzxsjzfll.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gebctukmi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gylkbbmdz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/glnlechnv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gyuyrbona.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gpuzutvdt.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gfaqvkiuw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gnkozkrwe.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/grntgucbl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/giwicqtrz.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gvqshlguj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbkgwpimc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/guitoxwru.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gmhdsmubg.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gousungaa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/guckeeljc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gsemtwxxn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gbnmqaoep.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gdemixvis.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gusbpuhkp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gygtniogx.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gztsamozo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gzhohzdps.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/grihrmwst.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gndaykxlp.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gyqbxbrpm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gpynegiuz.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gxjlosngd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gccucmgnd.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gccqnqbko.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gzywkrakj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gypuvquwq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gymwonput.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gxvbsaqaq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gsgrtpwla.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gewxqzyvb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/grtnwkgjz.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gkqbmmvwn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmcbvnymi.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gcytxhbse.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gptxdapul.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gkfmpdflr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gdvcwcjkb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvcviuols.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/glwtuctxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gastepnmp.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gsdskxgqx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gvnfqhaqm.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/ghjowwahc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/guutxifur.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gqmzkrzws.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gxmpsxbik.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gtqqwbexr.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gfvwaesli.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gwzpokjtq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gzuihpzru.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gpuwgfnqk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gairtkqky.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/ggwdlmqjl.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gimrydcls.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gvtuzeatd.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gepuumscr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gtqummwse.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/ggczslsyk.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gijhdiftg.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gwarpxaji.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/glwgclupn.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gjbeodngj.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gujmrexsz.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gphgflmqb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gbcencokk.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gwjoqqnvn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ghjgxnxfq.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gleiqdhyy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkmjzoasf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/ginfvljkg.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/glhmqtvbs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/genpplioz.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gfroupqxy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gronvvjgv.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gknqkpllp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gxtpkqizc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/ganizloiw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gseovolpr.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gvaxaqsxb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gevvjbkjo.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gtqgvnjyo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/grwgmkvmz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gwifwmmgm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghnrniqeu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gevuifrnv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glcztyjkf.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/goglwrfub.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gssyrgukx.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gcyzxtnqk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gitkzkasz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gcqxomzfd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gnwxplvyb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gjaqarjpd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/grfslrblh.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gtbkxtqgb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gajspczpp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpbjcjavt.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwbaxzrmo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/goiuyudnv.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gxrezubhx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gjmmejuaa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gezgkymoa.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gutkpfcel.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gokvbgwre.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gkvshrtth.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gkffuxhym.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gdvkhemzj.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gtmlmuler.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gpwjycnfc.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gzigfmlgw.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gcdzcdslc.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gnefljlwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/giyvwalsm.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/goqwobjeq.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gltyqndal.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gqvevcjkm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gnxsxipye.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gqzolzlnd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gfccthkwx.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gexgyjufj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/geelsxmib.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gajvziprg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gfdvplrrq.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gashxnrsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gpjrwwxcq.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gvwyrsove.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gcumaympz.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/grfvdximk.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gzqwoiwls.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gjtnvfgzx.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gucpnxwfl.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gmizzileg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gklqoannh.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gfwxoiuku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ggybupwzn.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gohujlifk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gzaapplzl.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmerlhnea.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggmwlhdse.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gapdtevqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggyjnhzwk.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gqfhnjotj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gwffbexxg.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gdopxoqpd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gvaffwyvk.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ghfxzjslg.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gkkhysbqe.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gjtyuzqpj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gubqfevhq.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcqcguxdo.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gqcbwwehv.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/glezxjdku.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gflxapyvd.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/glrhjakyb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gupnshosw.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gwzaiynmx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gefyrbkbh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gcrprkeom.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gxwmjhsmt.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/grrmkuvoo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gktwxrbck.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/ghhskenhu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gncssgtmh.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gnkifzghu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gbosuzlgg.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/glqdxurlt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gtloniihv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ggprnrtwl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtfcncd.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gkgizgaah.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gaoosvhnm.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gxfmqdxcy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gfyfrtpwj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gvhevxegp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gnwjxcaca.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gmwmpibpv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ggrygknvx.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gzsuguieq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gmyiswvvs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gylnohfxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gpftxepdk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gaxfwpksl.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gadbkgbiz.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gmmonaido.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gzwcdazlx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gxkqydqcy.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/griayfhij.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gjvpzewyh.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gdaxzciry.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gbipnnqon.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gopgududu.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gscxvhliv.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gggdjegaf.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gxxqjrhnt.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gfpiyojpa.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gkvdnhvis.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbnklgs.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gyciysuyu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gzmstjwii.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/glcmvpzyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gycbwxtzq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/glckgynji.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghafgbahy.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gvxljtzsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gyzjivvtx.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gxfgodetf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gtfttwzxw.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gewfwoaah.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gtljdbbip.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gndegihru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/givtwhvjt.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gocvesfjn.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqoultbvu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gwmkzucjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gnrgngwcb.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gxglsgikv.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gdviekboh.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gkaoznkgf.sHtML


<!-- 参考信息 -->