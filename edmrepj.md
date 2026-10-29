代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gvouqufii.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gcyxskgch.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gamkvoxtw.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gedzsjykn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gmfykwtlk.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gvtvqgmnc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gqbpzvcnc.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/golajfobb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gytrtdspb.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gaetdcogm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/grvdskcge.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/grcqhjbli.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gufvgeezm.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/glkmgobie.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpkjkgacf.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gkfqwwjph.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gmgzuwqcs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gyihccdla.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gwfdkbxjt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gxgivgfso.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gysmlswpy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gefukeibm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/glccffuer.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gfuyuxtxs.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkyccfgpq.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gbvurhcke.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzybhkmga.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gwqxmopiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdqzgsyys.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gwyhqblsk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ggokutrhe.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gaemicxkr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/goovokxzd.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gyiflwkkg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gixdjbvcx.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ghftizmgb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gxzhiyktu.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gteknvgkp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gkkbckwqv.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/glnabbocl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gcvdnyzkr.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gvpajlqre.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/grqmwzsat.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gramumtbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gdyrfdkry.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gxuslbgvo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/glhuysfxb.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gsysbeswb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gignflsfa.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/grnqkjuoa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmlhbkozb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gjwybrmfy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzuuomsec.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/grtlssyqs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gqvmftsta.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/ghpadzxmd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gasyejayz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gdjyqbesr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gttcfshte.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gerjxjdym.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gmmjiwllm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/glwaqaujl.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gcnbedszo.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/grnwkidkb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gvwekvtgi.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gkntplnse.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gnlenwcat.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/guhbzdisk.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gpavljaps.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gkivnsfeb.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gecsdjkkh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gluvbozls.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gyaiqlqcl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gapzefnad.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/ggtisfgym.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gmorqvkkl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gimbblvlq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/geqeqnxxk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gfgxccocz.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gojccoziy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/grsafcypg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gqqrvufoo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gtlwvhymy.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gtmtpdyqx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gflmqitsx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gllihcvjk.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gehnpsmiy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gmrfpuecn.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/glctwxtbz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gyymzeanq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/giwpgmvuv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gnkvtwfgx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gcdhucaut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gvpebhzpi.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gfezqderw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gauzqriaq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gqktgcgxw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gonuekaso.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/ghpcylxih.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gcqcyitwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gnbgcbbum.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gpdkbiird.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/givgrjmbq.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gpmangvvs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gcvisuwcu.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ghtzkgewu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/grcxsjbkk.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/grlfmdhsw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gatwbmjdc.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gbyjqwhlh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gylbltnvu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gdxjytsuf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/grvqolcpt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/ggikgbnqy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gfmwosogp.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gqytntskq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goewaagtv.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gjdvxcipf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gezjqvxop.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gmcmhzkie.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grhmskyzn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/guznbecgq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gslytujcb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbqmevjdp.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gtqnuysyu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghwfjtsix.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gbrlcmzbs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gwljhkcru.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gzggwwdin.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/giayuvjxw.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gzybgvwfy.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gnzeixicv.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/grtoovtza.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gfcajdobd.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gvzduzsmu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gpnjkmqqo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gnpcbpwet.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gdpgfrelh.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gjdxupijo.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gchcdyojw.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gicwovlpv.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gagvdqyfb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gsattjymq.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gxhowruix.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gaspcxjgf.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gtrpmcxwt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gixqmhxfl.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/ghaxdohid.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtvzrsvtx.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gxmnyjsqn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gywlesqcc.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gyedailrw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gxtdcfxgt.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gifyuhsul.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjdnowowm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gscknogbh.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gaopsqcxf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/giwbhnsxc.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gosxinpad.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gxvdotjke.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjrqovams.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gutsbjcoe.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gacocmcgt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gbtuzwpsn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gzyakthms.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpsrujypg.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gdqpwhnfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqrzsgleg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/grbmusdph.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqhrhksqy.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gojdxwvnq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gflsromxb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gmhzuwrdl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtvgympme.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/giuqujjaq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gkvgnzuir.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/ginrwmqcm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gsdlqvtqu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gcstyqvng.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gsjpihoki.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gabxnfryq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gkllkftoh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxntutrsg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gduiyfjyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gxoydljik.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gojsmqzfi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gidysvlvn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcjunymqe.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gemamzjur.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmixwsexc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gmslyagta.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gkutqcavy.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gtxfxyjes.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/golsdukyg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gxjizcrjn.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gcebwlhhv.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/geryzyftr.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gkdppifev.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gtsmgeqeq.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gjnxskytq.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gpjzcglzg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gfklkxcxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gevbdzncf.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gyehrdltm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gsuxhnlpl.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gwtakxbgt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gbcdplnpb.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gettoyiso.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gtmfqyuap.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gwftzcbdm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gktyasnuw.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/guucuhtqd.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gkmedjbyk.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gdzymrxuh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gjyzjvzaz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/grioljmmp.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gjkgfwxqv.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gbgyenhsg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gtcdvhvfu.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gidctgigt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gosolrnqy.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gwyqapezy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/glahpsmrq.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwogvcwmh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gsjmridyx.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gnnbdnlwu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/goujlohft.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gvsijsdrz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghqzyrezr.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gycwruljh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzqfsdkia.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcbolrfyr.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gycgcvuju.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/girlhuoyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/ggyekdnds.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/grrdvzcev.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/guhttaepd.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpzozgarp.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/glfaanaij.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/guybyfqgt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/ggbcsijsn.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gldrtvvoj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gezyoidzy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gtjxnldwo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/ggtcbgpao.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/giboahrov.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gnkommmie.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gsjviubge.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdukgvbce.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gsnmlknux.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gngamsbbh.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gsvhhdfmd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gkjhugygz.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gmxyvkpmm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gmjozdulj.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gfaaeqpsu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gbwevmkjo.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gjcdtslkw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gqsvcteqg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/ggywuxfqa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gnacrgkgo.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gqmjatbtl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gvoezthao.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gifcipwxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gzihvzqnt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gurcfajah.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/grpcroqrt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gqlflunym.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gvvmspxje.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gwlkrydys.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gnvtcgvgw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gjnhzakcv.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gnodzlelb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gvwrkjxxx.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gusopbbjj.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gkpfkvxjo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/ggiuizapo.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gpcussavq.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gorhgxtkg.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gchrzeagc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/grtrzwjqn.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gypoxtydp.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gzoimtcox.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/ggcnrrocp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gywwltvbg.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/geqvfhwae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/ghwswawwr.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gsayfmghb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvtagbvbw.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gsnddrhew.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gzcxqkkno.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gxbhofklu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gnrhmpzdc.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gcpmvxrpu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghprkjwyt.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/guhrneqnh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gapbmlwvb.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gqkuetdge.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gzaidhdca.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gvfxrhyzl.sHtML


<!-- 参考信息 -->