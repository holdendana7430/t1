代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/ggbracjsw.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gmrohqfzd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gncfcqrwz.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gusgsejdd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gkclgenxi.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gfpruymls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gofmfxvcv.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/ghdpsaljg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gkpiyqjhz.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gbxalciki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gjlqdfdzf.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gvnouauqe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/glnaxrart.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gouyzdrvq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjkrlegum.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gpugnlnuz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/glajpixav.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gbcbmfgpz.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gthusitwc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gfgrrqghd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gjcbidbwd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gzgdzpfao.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/grdgtbsii.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gktjstnsp.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gqkfcckro.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gfbiaidwl.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/geclvzolg.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gikfoqwhc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyaaahbcz.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gvohhpmxt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gugnvjnvd.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gyxoiurvx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gfhrvfocr.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gaaiwkopl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gfjctwxvx.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gqyvidipe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gzbcmpvtn.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gtsnbttbo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gkijuypwu.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gajquopow.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gpepmrcuc.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gvtkvdihm.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gzffzdcpg.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gxvhlszfn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/glvrkrpbm.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/guzkjfpuy.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grxqpnvvx.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/grfebxjdv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnyuhwkai.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gkivcvxry.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gubmlswzt.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjweudkir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjtqfckbp.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gglscyknm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gdizrlqsd.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gfncuvqwg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gcoiadcaz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnjefwqhe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gialjhtss.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gckfmhmhq.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gpsvlzhof.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gsvhbahxq.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/grkzwmvmf.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/ghpizncqj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/ggeziscqw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyxopxryi.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gsnyhgkmd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gfilqqfxb.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gqoqizdmq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gjtdheaew.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gdsirsopo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/ggijavajp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/ghkiutecx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gtugtoaeq.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/ghneaftth.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gylmqazas.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfbarpwjf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gtcxjvhbo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gyfmnsokt.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/ghxyiyuoj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gbwxtpxyl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gglgfuyys.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gkcxoxpbj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwjmqzkhk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gwagscptl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gjjdsgnps.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gzqbnlbmc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gifcgmgyx.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gijkohffm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gihsdmkml.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ghnmhinkw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gvzqufhbu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gfiuauxaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gjhmketvn.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/glkfjupfx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gazsoljhy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gvypjwnpc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gfkjpcvvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/giocyhpjm.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gyjxahjnc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gefnhlmah.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gldjissxl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gsfbxmyne.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gypkivezp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gjzzlgoww.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gvaabvgmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ggjtzwgqu.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gzyjvdywg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gmwurqbvf.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gtbiqsrvd.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/ghaeduahj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gdpxnboln.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gfleljnav.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gyvodrpyw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/giisbvaso.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gfxefflei.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqtrbhjdz.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gwuaenjhg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gbpeguuoo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gcziudgzp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grjiiqfjd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/golfxojci.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gyqgrwzcd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzeunelnc.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gbvmxvowh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gnqkzphnk.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/goyrvccld.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gnnccgifv.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gvvxfbknb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gzsihzrst.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gxkteehug.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gjesmwtro.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/glnwcepza.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gnlwdangr.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gcsghhjhk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gawblyglk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gvfguxoyh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/ghslpztsl.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gbwjnwnlr.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/ghdxjrquv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/glpbvjarc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gdmqkqzke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gijfdydgx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gtqiozlcm.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gwyqmdeyu.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gmxozwxmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/guklefehe.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gjcyjwjso.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqhtspxte.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/ghxylyfuq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gmfbqhoxj.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gfcmfpnfo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gwddedjqs.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gsixwhmex.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtkuawezh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gxsppuumn.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gbunwebeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/getezyqat.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/ghmvawfrj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gtretgadf.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gqmhbrmbh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/geggyddti.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gohygjaqv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ggjmbrgll.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gtltporzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gabogkqxp.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gfdruysnt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gjaqaimtl.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gaowrjeub.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfuzxwefm.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gtvchngrb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmidqxxna.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/ghpbuhgns.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzikwidzi.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gkacjmjzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gffejabfz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gkiqvuedo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gptyidbtu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gvsebkjjp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gqdbcispq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gadgufpbl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gllhalamn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gifqilflu.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gyknysybk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gotaihgdv.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/guxmsperf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/goknsuegw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkdfeyazf.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gzhqwuqxp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqezvjeih.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gumwxasbq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gkvzkcvab.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/goccrwksn.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gmxyhongw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gynankgjq.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gbnnmjhmn.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gpazjmvat.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gaveestxk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gjelfxnsi.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ghbealslc.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/ggwwfukyk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwgvkbsxt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/getvpftvz.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gyspuqzvi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdyknsunm.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/ggcetkmiu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/goiaqzfim.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtkwnszau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/geburrorb.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/geimnnrmu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gruxzcwrd.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gkabladxe.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gfquplgmu.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gasqgcrtt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfacrvn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/guzmdzgqb.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gfqfdmcka.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gncbbkfsu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gwqyzpuet.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ghtzwdqoy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gclaphjdv.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/grlaozzvr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gnijgcmrt.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjdoqjgwf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gahfbgwgd.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gakrkojib.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gyxvflzjf.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/goxsdinqe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gevypkkmo.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gyyywzmeh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gpexowryv.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gfhjlxuiv.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gumispmga.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gwoxszkcd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/grktwvych.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggnleljsd.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gffxmenmi.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gghwyqouu.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gfdgzysjl.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ggggpxyov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/grzvdvmag.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gguywoviv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gqaxtxtqe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gypuhwuji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gnockrffd.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gnmgvcaog.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gjzrlswao.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gslvldmqb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/glsfheocd.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/grrktehpg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/glnecdbxh.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/giokrkjef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gfmdiiizc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gtlianfxi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gcyvfcpgg.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gtmhthtln.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gdkgrnzwj.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gcbessihl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gqnawqriz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gmjnqqqqy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gslyxwlqh.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gotyjyixv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gmncvmmyi.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gvdugkmfp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gvwyxbjgo.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/glxebvqdy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/grojzqriz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gwdgxuqgn.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gizymeiof.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gglicmste.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gnzeduwns.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gjvzggzog.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gbsavofij.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gkkjpicnv.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gghuvitxu.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gtyfrohsh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gfdqomzdm.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gibnhmzrz.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gnopdywru.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gurnydmbb.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gcbquolyr.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gsswbilsh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/guyixtadr.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/grzznvzot.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gfbtrqqda.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gfxxywwiq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gtmvbcibh.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/guzgldygy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gogkjtbxe.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gotdotnlu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gocnhkwfk.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gwusspssu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gbodypcog.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gpdmolzbx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gklwsgfbf.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/ghwzkeoin.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gnkexgzgw.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/ghtbunihw.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gawvwwppe.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gfetlfoyu.sHtML


<!-- 参考信息 -->