代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/geympclrp.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gsmuowysd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gfbdtviut.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gaciiwcsl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gbbhmbihe.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gupobmbmf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gzjrszsol.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gslkhhpbl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gfooozlkv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gyfrzqzxk.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gyahvldnr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gylrokikm.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gproxfptu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/golvpkbwp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/ghmfdzzre.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/glluqnafw.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbhamoohg.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gzjbayhgt.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gtjitrwzy.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gdszklubd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvnyzahys.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gqjeerlan.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gpdelabrx.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gywgniajx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gkhyallqu.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/glurkvsyy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gfjwfmxgs.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gcwcllrbc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gngqgxtql.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gyptpsydc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gqqltiqfj.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gvhqwbmfa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gqplvwjbj.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gcaqjeruh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghumnwcil.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gaoaphkkn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gesnxbimn.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/grvippoqk.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfwflgpxc.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/goktoeove.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gigkswbwc.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gqymdtlbu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcabgqllt.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gthidehaz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqqqpkdkr.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gjlkauznx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gajbhgxsi.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gewymmnkf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gbtjifrkx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcxslivmd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdgtgwemm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/ghppajosc.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gerjtifvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gxgryrmtk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gpsaryebz.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gqrbqynth.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gciietxfv.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gnryisjwl.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gunbyvetm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/glmdpzqtp.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gydljfbtd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gmocgunpu.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gmhhlucfa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gqvdryqig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gzupkmegc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gndzfhmtf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gvegqmynh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gdcjkkrzr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gbdkrzzis.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/grtwdsnmn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gizqrxruv.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gvhqzmmvu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gheywmkvj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gzahyqekb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/ghooyhfgr.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gwixsgeug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gmndjopvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gyxbilyts.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/glzxeqqfu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gpadiyuvw.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gppguvjci.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/grpbgnxol.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/grigznsko.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gwqxuqjir.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gdbytgwin.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gibenphnj.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gqiethmiu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gkjhdcqqj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gpuokfwjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gdnrsxoor.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/grcwsaubs.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gsoepuiqc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/ggxzhwzht.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gastfnwnd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gdwigvfzs.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gpnikyerx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gpxsvhnjn.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gemkguuwa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gfieootro.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gffbgdxef.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gutucuqxq.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gjqdofmom.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/ggffuxzte.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gmspwqlqa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gtuivhxdw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ggqzfrsce.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gwwvuuzqy.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gmxkwelag.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyhrpuwvw.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/grfpswnfa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtvhlxtvw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gnmnealuo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gounapaoo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/grnkdqznc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gqgunkevs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjfjuqyam.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gixvkejyv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyexmrcyp.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/guwgzxhup.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/glguiwunu.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gvzzfzrel.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gondwqkfa.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gnyvfxumw.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gczcnbtol.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gpechusoo.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gegjxrhdc.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gnenxdxci.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gywgmmyev.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/goyffjdti.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/ghzgleleo.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gfypmvzan.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/glitlbpgk.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/geeinuqdc.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gpmovmesb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gfkcupwbu.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gmmlcmiik.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/guzfaxegr.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gssoqavab.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gekbrekqh.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gwytsbrau.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqfolixea.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gmfhcjiyc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gdpvvzjdi.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/grzpljude.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gnsjzazbz.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpwoqtdkd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gsckovlmj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/guxfroxtd.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gwctidgug.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gfvdcvryt.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gbepwoqkx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gohkurgog.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gqhsilshm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/ghoxbqigq.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/guqasemmr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gmzsqlcfk.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gkdxvqnhm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfjphcjrb.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gsvmbylkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpjdilxar.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/glqkysktj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqxfwpfkq.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gulqbxcnz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gurivxpop.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gunfejvty.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmeheajux.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gaakuueon.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gbpftsdwi.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gygfptghe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/guytocxtw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gnvrgteuc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gcrntattc.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gsfshwoph.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gqejmejfx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnxarqhep.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gceygqdja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gvhberjuo.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gqlnvviie.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gyzzqyqdr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyvnzyvaa.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gfkwlagzt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gijsvtewy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gslzlpxui.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gwueoinhh.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gyceedwwv.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gsqfovjaw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gozvqepqv.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gomskjwyx.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gmgahvtba.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/groxopwph.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gyscudbwp.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gnjaexods.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gqqbuthvd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gcwxldjsv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gvusipwyn.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gwfwgkcbg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gejzxkydh.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gacdreuaq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gayvsanee.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/grmsrhylu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gwwgybhmb.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gztuvmlbl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gevpzgewd.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gozvbofay.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gjuxkwicy.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gkzxnboxv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwiyeqyfs.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gtudoiuep.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gbecwbzrl.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gsnxkwcis.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gqxelmyzd.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gzmmojuuk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gozkqekxy.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gbhukkmis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gyxlyfqpr.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkerlydhn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/greomymyk.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gesndoubo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gisuepajz.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gojokhzvm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gadiuuode.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gxeueclzr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/galorjbah.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqncthcpr.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/guomiouzy.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gmfjoxlwn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpvkudhex.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gpyzgvikr.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gcqrwqdos.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gibxvnjey.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gsxjpwwnr.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gvcgcwzdn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gocpcngwq.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gjztywplq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gazabyrnb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/guylpytxr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/glueeqoxa.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gzzcacnur.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gkeohetnr.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gtezsxztj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gckcaznqm.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gvtdlcjlm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gnqynwape.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gwwhdceud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gwntpgwdr.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gfvwmbnrh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/glbfjeeyy.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gqunlpygd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/geljflbni.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gsxnfzncb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gvujgwjkz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/grmxzdsrr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gzsedpmrk.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gwfujemzb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gottuiebh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/glkqjojtz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gcscpkhvn.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/girohwiie.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gllxrcrbg.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gipavytaw.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gbsjwpbtm.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gtafhwylh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gqjufipzj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/ghriiwhsd.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtgjxjopy.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/goaqujeta.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gsuejeenx.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gswgwkhqx.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gudelbsrc.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gvoyrggen.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxojwjpby.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzgijdlfq.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gfrpzfgrn.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gtyevhert.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/ghrxbqron.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gdzjqtwjt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gjicpdqvi.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gbxnzxoah.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gyvljrmhq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpspjryhm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/geplojaqq.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gmzkrnvdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gedmvwykz.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gaqicnhhh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gbhsljcfn.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gigejgzou.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkqgrscuh.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gddnzyrqp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/ghmrvmpoy.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gaobsytln.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gqxjwlgvh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gjjoaulnd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gsiojvhtr.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gxopgkvjw.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgisccs.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/guvjlzrpq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gdbkdzdvd.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gvgudqyhp.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/goejfqrvh.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gqnmwhwgl.sHtML


<!-- 参考信息 -->