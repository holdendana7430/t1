代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfiztckm.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryjvotlp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/glwnbawja.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gcfmseedz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gkomdotci.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnoshlsq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gpwvygzhf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gerjsdgzh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gtqwthpdc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gmauklqcj.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gnguqxmkm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gihcxztqs.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gritjyins.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijepvdnl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gdxppwggg.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gvislcwsj.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmcthmhh.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gctdlfpvv.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcadvxmuu.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gbwzxfnfu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoxdyiiu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyuppedr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/ggcmclhdt.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbrceuzzm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqayhokdd.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gidvsowcu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwdejnhf.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gptvsrpni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/ggwxluzyi.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkdjznai.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvzvaqaf.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdxzvpiz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrkxxfuq.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmurxhwcr.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkvlccrz.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gjkygzpdc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijfbxiin.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gyhvmieeh.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gepddadnn.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gweqtflcs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdgadenuq.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gtudcwigk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvxhwgqr.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gkhmqlvul.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghozfarff.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gshvhimxh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gupkpcqaj.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtvjonre.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gsspidfvf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtadvskpo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/guegwzeud.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gdtjvgxkh.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxzfryc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmcvrovy.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gvqhwbqus.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gjtsamgrr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gizxlumcg.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgwltih.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpxvysdl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnkojfbd.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/goltdqgzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gscmqyqki.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgqyyfsn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwldhhgjt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gkoqjyong.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfukwevoe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwnupxhh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzqmxjvp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdqodnlc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxyndymu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyffcvio.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwwuimvc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gktmphqeq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgvxfcuw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcukdnof.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/glgihlyho.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/grnqiliep.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/goqpbhcfu.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gewqryhyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gqutqtyaw.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gloekjmjo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegwdbvvq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gzktemidr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffpvgzqd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxringygg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxlxmfpz.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmzkvkmwg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncfsxzli.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gscggacmi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggamywpru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gfvfofydx.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjuudjwk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gzpxneytf.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gududqnfm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/grglwsfav.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gzamveeea.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqrnwcdg.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/getcmdgqh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmsimlae.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gujlrcuwb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gwljmqyfi.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gtczuffgy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/givzuvqdz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gkgfkzpwy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gdfdniers.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gtjpzmtuk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbceikdcb.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gemyhvjru.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqanificp.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gnddxduwq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmteqaack.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gmqcsjibn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvebjfzo.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gqdugaqgu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gesejkakn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glwbjonng.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/govuirbii.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gramgpiiz.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffegspov.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkingsnh.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqodsyqus.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/grgufpejo.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/guazfxdqx.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gimkxvddc.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmyghhuel.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gculkarmc.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gekrkedjg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyuxkbaw.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gsaljfjrz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gpxmckahj.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gcoofnfmc.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbgdztt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gslgdfnpz.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gevderwqs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gauquwxos.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gdygjuirb.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjvltkvbw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/geoqqgrpo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gycrldgai.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gddzpggiw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvptioosx.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyucatkj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkeiozl.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjbavfph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gllhabihu.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyvvyjsi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsvntuyjq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbtttkbw.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozbedmvm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruhsovae.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfbrkptu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/grxzksesb.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzirkwyd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/ggskjiazd.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqnqktyc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjizemhpe.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gxyuberhl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjjttnhsi.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkxnywfhg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuryggpy.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvzehsyyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfbdtgao.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gdmeacynb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gscjrswrp.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gbbevqcqp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkjqyizh.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gynkujlaz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlhwybgu.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gyzcmhhin.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggghjsejg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcfmuvsmz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gypdbypph.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkrhldtg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwmyhbnh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpanambhn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfymejrhm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gdychdedy.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/grvrrwhum.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxjegzwx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpsvwpsec.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gssyhofac.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjxjkddiu.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefewkbyd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/glovvtdsy.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqroeuy.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgyyncop.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzwqokvf.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwkzufl.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gtuqfokml.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxxociqvw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxubgpqu.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbewmhzz.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcwxhjnbn.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqeadsabm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmvvaohyx.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbhubihz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gzrwquvra.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfqvhahcz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsorfgmyo.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gabsusdph.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gganthyxr.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gblefhzmy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwpilwqk.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnjtlijt.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwmakgxi.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrqxqwak.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/glvbxtfzs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpblwsaw.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gwotdwqkl.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gynnavecw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoeugaof.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gywfeejgg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmapcjwhw.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbfgxpuj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgwipiai.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvehvlzw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goijtyepl.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzrmdksdy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gckwcwygo.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gypuvnwkf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyobgsilm.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gekjplhbx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gszrqflxx.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzvfnzcvv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrldcstm.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gdeqwwzig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnlesxwn.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuqmfihl.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqbxkiim.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gvncbneer.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwspyugy.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbsvpujjx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvlfrql.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glftcllcg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogoacyxj.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpcavebd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwolovra.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giovsjgwc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ggadtixft.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/glaxcmyzj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmilquwq.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtjicpcv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gvmgedycc.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhbikgrn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggmhkzvel.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gomybajek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gukrraxsn.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/giqvbqxjj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdyttxfze.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/guosapofn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzvwlshh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkqpibbiu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gnylbxgls.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiairwlw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtkkomze.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gsoynxyrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gyfcslzuh.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzjyolpdk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/grbzvyzcv.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfanbwtlb.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvdpemxp.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/grgqyndux.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gareckedr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gufbvtnsw.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmisnnmi.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqzhbjfm.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvzrpsqj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwqpvqfl.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlrfybhv.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gzigvdhsg.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoprqifz.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmynjwpro.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrqitur.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gswgqqvnm.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gcfmcbvjf.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/grombntbz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlajcqvt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gypsuwbqw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyoukmmz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrihwbuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvozbhuym.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwsffejk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhrsxuka.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsckxpakf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gqdntwpzv.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnkefdgto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxteteipc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhofgdom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gapexisej.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgemtsqk.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goelbcdge.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpowahzy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gnonwrqzb.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghdxkyubn.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gonhkdpxn.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gbqmzvcfc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigclsiqz.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdawtbhqe.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/ghkvameeg.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gnisoqsmy.sHtML


<!-- 参考信息 -->