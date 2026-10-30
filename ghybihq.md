代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gzisazusn.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gkpvtjbsn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gfxzpgxek.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gabdgcdck.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gatwzbmdw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrpuvhbd.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcfivyyc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhppxkev.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gzgfbnvcr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpefuhln.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gltlagumi.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gilxsgcos.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gathhsmyo.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfobnles.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyznnetaw.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gukswvpnz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfswkbjet.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtmfoeueb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/grqecxktc.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqjuwial.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjweribn.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyizfufm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzspvxip.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvsffhbm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gowwgtamr.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gspqvtobb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtomywxfd.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gdntsxldk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrobhrlm.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkvugkum.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvklvtzbu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvbmfxhb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsuupdbx.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/ggrpfzxbh.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghlyeevoz.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gykgzjkjy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjnpcnca.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsiayfqn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsienmpzr.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/guerztkeg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guhlkwzmb.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gjliulocl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyefzwaf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyyxxalu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbkswtud.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gewsoichi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gskxkeupm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrzoauan.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/graqmfovz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gqiafnjfa.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtachuvvx.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gyrhxmdca.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gvptcjvif.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfxuljzt.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdojhpio.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemjdyshf.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/glcrmjcmh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gqgivsolm.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvuxtzav.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gredsgxcr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gbiaduthb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiyivchh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjyfooyy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gbcmchgkd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gloxiyune.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/givoguglv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlgqiblz.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/geiatcwwn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/givgbkrgj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbklsuz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/glpihabco.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezlzwifn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gbsabaxic.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjownavz.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/geaefkkjw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/girzfqhse.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glmcdmqrr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gprosgang.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxpmics.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gybgvqybe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grawxteqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/glsmgsigi.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggjigjsyx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/graflhzrg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwldkerzw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijdtspck.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ggakakbkv.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gowkjftyk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdklviszj.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gomvifajw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gixljpdbz.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/grpojifpe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctovteuu.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfpbzsxv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwfqhdnp.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gnlvzoqgi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/giszuuzzp.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnivhkbuy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjakhgfi.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcashwin.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gizyjihrd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaibwfdl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjdalaw.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gaisxmkoq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gijpfgptp.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycslsqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxuznclu.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmrvcutg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlouyiwb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gmcflckkj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqniimss.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxkroas.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhtqyvdg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanriuxw.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbonsjgl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gknxetmxe.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdrnypwcj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwrxgglg.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmftfev.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggylujnvh.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxxnkwwv.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/ggsnhfpvp.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/glstwdvey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddgdqamf.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrrffdnv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbgzemzl.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlsjzvqg.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdurfyzu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnljppabt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwodkkokx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvdywojt.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcouzhoe.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glvdpkncc.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gxabwqkbr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqmopdmr.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/guwtnhafo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxfsiuvb.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqrsrszz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gydsszart.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/giomndlif.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvungbiac.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gehxosjmr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcyjslgqp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjezwoxn.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gjakkuzky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggectcjgr.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gujrzeygz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxonmtnt.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/grdljtalp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gapjhbcpn.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlfjgcof.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/glukklngh.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwuxlfrt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjmyidgi.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvnsjcqxh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtdsbapmo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeygtyyq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gforyolhh.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gavwphgkq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvcidgok.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmtiymxn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gilianefk.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/ggugwqxfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gaevyvkyw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuplhjac.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecumbuvg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbqwlsytb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyfekaor.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzbcspfd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gfoznnppp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsanssvcc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyzkzppz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgsjazja.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdptbovh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gclpwzhgt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkxippcfp.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgzyxlis.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnhymfwhg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdnkmzdp.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjsvmbn.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/glbpmglbr.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gqdaseuwj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjunfnjhi.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gapedlgsi.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhlbzhme.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/grhhduylz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gravtfidz.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gullfugel.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gknmemszr.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gwtxojaff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyskctey.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxynotbz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcevgsyub.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihwznkcp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grdqjyvhm.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grweeyjjy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtplmqbr.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvcdfadhj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdvcoohc.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gmsvvgqiu.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxydvqvz.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbixtuszj.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gctldkapk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gaajhwntd.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxzvzoua.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggbitshom.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdmxoytl.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnefnzgan.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gokhadlky.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/guffpkwno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflvpmtrp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyulgxkt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdngzrlhx.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggycdtghn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gisvlhwuk.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gwjpnadls.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpumljevs.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlabpquu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfaznlpce.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwojldnkz.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gccjklbrs.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gcnonzphm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjrghguac.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/glkgwupbh.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcnilovzy.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtblbkfgl.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuhkegmn.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmvahqu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbwgquy.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydghzjc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdoprnnz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gejobtrss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjqgglfe.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrovuoom.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdicixixd.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/grcousfsl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjntkpda.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gnyrexlfo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsptuauqh.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvchsxfv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gsztqroji.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqtrcedt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxxqvacy.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyqbigrby.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmcndxzoa.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfevxjst.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwszcbnmu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqldgjjpl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gfdlyblvi.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmofccpao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gvanjmuyt.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcnoepab.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvftdbxu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsghdlpeo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdqicevq.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggioppiei.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbaladmg.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/ghbcabhcx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjblmszxv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkuccho.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gixyjqale.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gajfjmevj.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gejnldyjq.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbjaxlj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbviucbrd.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxanrphz.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtmyayec.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gytukqfqs.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gicafplvr.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjtynumh.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfnycoeuy.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxxvpudu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gonicdmyt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gwqzabmcx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeerskpx.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqqxbcdmi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gttxniwfr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqccouga.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gligzugti.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcheyrcr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/ghabvauex.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqwrpjmp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grdxyyigp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmdsicjr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/galchgvzg.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxoodlv.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbckqxvop.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsapoyaa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdioejmju.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxlktszsr.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gewifpwkw.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnwxcqpn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhergrzv.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfclinvbp.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gegpglora.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/glpazyxgd.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjmhnmlpp.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwegykrwl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gqiwcjeey.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvrhrdoz.sHtML


<!-- 参考信息 -->