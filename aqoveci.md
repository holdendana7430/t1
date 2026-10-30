代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gpvagnmoc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwjpzbnc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gyisaqznd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gsjcdphbz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/givwqsant.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gumyyxpvv.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/glqtfdlgf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gohuylinp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gsyahomxu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gmdziqtqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmimkdaae.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gayafefri.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpllufjwo.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnqjrvov.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxixuasyz.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gdoiunyqz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glfvsbxlp.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghsbiivet.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gnixzcqgo.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqauutjt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/goufemegf.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjoegom.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmsqbymk.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/geltkwuje.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvqfrwf.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpvjidzh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gvtboiddl.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/getmuhbtz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/grhzucmzv.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/grmftremg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgjmtcko.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gwhybtwrf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gofwmvynq.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnubhzmyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glkowupat.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gmtybvfiy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoyvapfj.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdwzajko.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvtnullw.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gchkapmge.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbszabuyj.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmnfsivv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gldbtasgc.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/granaepmm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjuqiyme.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goltsiwvj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkoqocda.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/goafchutv.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoyvmyqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gysnfhiyd.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/grpppskbo.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gljmctxvy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmaddjzv.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grdagoxdf.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gypdfxfxe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gowwlzqzu.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gcumwrpsp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjjphttf.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gfocloiaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwzqyhjk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gqxkevhpm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvxunffb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gitmasqiz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gfehxmgiw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygbjycwt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giubhertj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnapgvfs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsylndhb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjxlsymj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gdxhggrwi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gopnwacej.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gafuysweh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqgjroix.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gupqixwbp.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/grypywrgz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswmyhusx.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/grjdsrqaa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gvzckeauy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/guaxgmhjq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcmxvqje.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gppythejs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzksgpsl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieflfkzv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnspuxkfb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbgevqsuf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gotveebzr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxywmoee.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/grzqzkjad.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gqcbxuhin.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gwalhywrl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmunuvyz.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gawrvvzwe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gthqklruv.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/golrylmbq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwhtzoqs.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlosejtd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gmalplqwp.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtewsjoy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gjnjegkyf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjmxsmyq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gowdxluvc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/ggzxigmoy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimuriozx.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfgihwii.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmanlkjbt.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/girfptkyl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgpumlyg.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gicvudjuu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfplzeyzp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhggszxx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gpsjzgidl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gijcfznqy.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpugtofq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/geohujbpz.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/glanzxhvg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gferygvsv.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimkraclb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghminlafh.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ggzlejkpx.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbklnbeao.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyommellz.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gmeksfowg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyxwubtn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnrvytqo.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyfdeneu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwqupvbq.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gtphnkzcn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhitydz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glcwjnswk.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gadftmxlo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/geuriumjk.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqfchzde.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqylfyxr.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gzplktgec.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gwzlxeizx.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/glwjrixdy.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giiijvojh.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuclfesh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gfteycdvs.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvefuckl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/ggpgvzquj.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvrwlefzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgpckzpp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/goncrjxkb.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuwobbtr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/givpevlnh.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/geouytnax.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/glghcmsjj.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/garuuzfmt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjvlmpik.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnzcxaav.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdgjrwde.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/goffydqal.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkddaoxoe.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gestiibwr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdpkgvswd.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmvcorbfs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfzfxura.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyqtdbnd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpfrusogd.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/ggyhvogil.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjncxnev.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/griwgrmpn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gsptzmzwi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlzdtoqs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gbkgbcbli.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqrcaaw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpiyujtb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcjnxmsh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/guhprsjuv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdvajqcjy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjarubxvp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyhnwliq.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gxdjpwaow.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gjkjufwtm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gptjqmaur.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/goqpwkcng.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedgrvejn.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gtvmuogbr.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gkmpzrcql.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gezjzhfsn.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gwxrmybxw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdojkowxo.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkitcedj.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/ggewozfxz.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gndbjaasy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/guhlzwgxr.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gwqtzmrzs.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtznkcjkx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guzwgruuj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqzipugwc.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gijmbvsvq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gftotbjfp.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghsfuqovw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gugxovmow.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfwspxir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsiaxtbm.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/graxltujs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gblqhgaae.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gaverczmp.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtblshanf.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gygivdifw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhxgszar.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvhtgsuu.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrdbplke.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzdkcrkq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqyolyp.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gznvnnrsx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedcmfvhx.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlayplht.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqplngmc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsazrmgmz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqojzstuu.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxacppno.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guxoespew.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszjemspy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigpwgqfy.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfbeaxni.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gacjpzdgb.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnflcvvei.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbfjxbqs.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhwgousp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzillcwvw.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhqfebts.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqefaqx.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gycrhqsqb.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmotegnjo.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gocwfrogr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmarvgn.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyminmph.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gufcruxhd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gclyuxztm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxbfjzo.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmyezkic.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ghcqokhwy.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/geuztagil.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/geqvaeiti.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjsyfqxze.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuqirlez.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gljunebvb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/goayllvfv.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbwnozjge.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdirkfke.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtfcmvssz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrqdfldw.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/givtyynbx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxptctmt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvbmpmhb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/giuyvbciu.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwdfsucn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/giyiyqmgs.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdcbvhlgg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjkakgqx.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnevdlbtq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdyzbwvf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzddddotn.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyirckron.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaqoqlks.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gokxhopjq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyvhvztz.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfduwflkq.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golehtbad.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunblkccr.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmasskiof.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxmyvnhuk.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtixwssv.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzogccbf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzistquux.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ghznzxvfk.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghbqytzhk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjynjdxl.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gldertbfz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmknqald.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gilndihkq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gxewfucpp.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwhsrfnn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqurodpl.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gouvobmgg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpjlcxee.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gciumrbvk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gxoyicovz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gifsrghyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gakzvcehu.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbxksjxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdzzaodb.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkjlvsgl.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqbqajgvj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoufwfsc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gihxmkzgq.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkzpdyel.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gswfwlzaw.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrpekwyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gmbhikprw.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqkmmxkfa.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gqcxsmiys.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/goqcberlk.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gpvbyezpu.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsqmdtda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlbpkcuv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqnlbhbq.sHtML


<!-- 参考信息 -->