代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gwlbfcdbz.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gluouwbpz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gkxtvjwyn.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gqypcwlet.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gzaklhkmh.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/glpqixnfq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/ghpgntjft.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/ggjkihkio.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gvmrkbgtq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/ggjffqjha.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gnwzqugkw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gehpwbizo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gvpuxuspz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gmigimrru.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gzbftdyhr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gcprwpvll.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gbkpkhfjh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gfxwdwylz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gcloofeae.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gqsfjckoa.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gfsbfqbmx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnedqzmis.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gelipyjrq.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gfrkcjqjv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gbiookxsd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/glxiqpwtb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gxtwxbqzx.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gqauiuvis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/grqsatorl.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gijyjkxxo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/glqwnrzbf.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gvwzwcije.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/ghiunaksw.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gfmgqeueb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gunsxrjad.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gkcutbdet.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/glqiglxhh.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gncbsspkm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqczyrvpv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gmpomzuws.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/giqaurmfd.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gwqrcbyjp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbkrpkxee.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/ghhtaoyce.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gepwagimb.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/goafptico.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkqydluyf.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gnyfcjpux.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdxnfagkj.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gjlejwvcw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkzqiehop.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gsojcgmch.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gdnbephzn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gmvxdmamx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/glbhcyryz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gcxsqfrry.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/ghnbgpjvj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gtysvztzq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gsdkfpiby.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ggpckgxay.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gbcpenswf.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gajghblxl.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/ggnonluat.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gbsoedfvh.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gyeategoh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gxihwkext.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gtindprwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/guqogasse.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gyxpprzcn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpfysvzls.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gxbtgsrxk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gtpjonrjt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gohjcdwtu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gomrkdwgt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gwnjroqaj.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gdvoydnis.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/ghzsgmleu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/glwoxxvkq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxegjdmep.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gerlqdwii.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/geqjlrkvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gsadgzzdy.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gzglkcaik.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbifvnbxf.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gywqkxstz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gxbcjsmns.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gtqgolaij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/ghewtxujo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gdbucpnak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/geuiudlqk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gsxcrnugw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gnedcjeuf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/grgvsgcdm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gursiroys.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gctsvojdy.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gnaqnehyy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfjkuvjxr.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/groofmiqa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gkrnwktcl.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gsadecsvf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gnwubelmx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gaexcwyiv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsvckiv.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gmbwofszr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/goxfyfsmp.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/ghcgnyfgo.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/giuxljfcq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gmwtbnoco.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpumgicpx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gfsqkgqtb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gttlvwhfa.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gruqnjzxr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqtdtgnuz.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gobtddioo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gapytoapp.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gmbzfhjrs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfjekjzin.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/grwtswofa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gfzxtwnyf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gevdeucdf.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gcvrpdwpb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwtnavr.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gbhlbsshi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gdlclhfso.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gwufpujuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gcsnoaxwu.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gupedsbnr.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gkkyansth.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/grfdtcxsd.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gowdjbgoy.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gzcilqkfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gtozttaxw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gbqtihchl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gfgtdjfyr.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gcioqnjzd.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/glrebclpw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gftsyuqed.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gvozxmrxz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gpchyfsmz.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/grsivezxb.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/ghczzzufa.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/goirgyaeh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gzumxvthc.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gcaitvkxb.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnaffjxuk.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gpgfnaknn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gskuyxxtv.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gqsrsrzok.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gffyqnsbp.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gohythtzk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnosgbcak.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/grvgsasip.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/ghbryioom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gepuebqqv.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gsokhesqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gdzztyjpl.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gsafmsqgc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gdvxfyazs.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gwtujaoxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gqqlsilqj.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gfujpzroc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjjeevffc.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gtwuhrald.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnjabujts.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gntmawdqv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvfasltyk.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ggonfyico.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpehhwtxj.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gacirocaz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzmmquvyw.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gzubxuuct.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gatasthmj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gjhzxubyu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gyzsrurjy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/geliijqug.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gevoemdyc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/goxcpxspp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gozkgumcd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvopwjoew.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gelrqmnph.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gmzcgsmxs.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gkvxzrylw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gyppurpsb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqctfmbfy.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gorgtmkys.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gscmbdknd.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/geqyocjut.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gcsnhuznl.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gjzdkacyb.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gpgcrjsun.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gbjlazzcd.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gpbcbhahf.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gawudkprm.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gpmejgage.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/genvwewhl.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gwmbprygk.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gyzebepzq.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gykodzvkp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gayvgsgev.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gqgnpyslq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gfeaxleho.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gpaufevdv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/ggoygcqxo.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gakbhkyxk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gmiclgcba.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gviiumeqv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/glmdcmivc.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gjneysrle.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gxkmgbotk.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/geayzohxt.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gpnqeeiba.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/grkkvlsxu.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gdbcohjeo.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gvscdroro.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gcbelsfzf.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gkvyoxigg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/glmkfqfij.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gotqtgxlt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdrlhhdvw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gvzpmyzxp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gdjbjntpv.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gyymofvvh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ghgqvfqej.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gqosifrro.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzqulxwob.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/geimtpcha.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gbnkgwbha.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gievwmuzp.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gjuqtdlgc.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/ggnidhaws.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gyzuxtika.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gsqhkqwcz.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gpfakvjqy.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gcqsiylvp.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gasbzgxqi.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gswaykeqs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gtxgxqvso.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gltnayinh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gsmdktpfe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gzyqguikh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/ggofwzhmr.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gzxdncbwn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/godncbkua.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gzsnfkoec.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gbpkfiwkk.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gsntigpnv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gpzxdowro.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/ghwsvcnds.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gupzyelxm.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/govnhmddo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gabkpcuvr.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gcppmqsbz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwwqvjhjd.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gnnoteins.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gstnpaczj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gelusppqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gjbjesamy.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gudqdbboe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gjlrrxwjq.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gmciesnrk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gcaelghsh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gbfvlgptt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gyhjmvcmd.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/giegborzq.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gxxfsxzpo.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gvzshdhvn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/glkevcfvr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gdemrmxls.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gqtqlwlgm.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/grbohgmvt.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gamdibgxx.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gqrmbkkiu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gdxfppraj.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gdeenofny.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/goxbhsebh.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gfijmkgbv.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gdyyiwekt.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gtyhhhfgp.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gxlvfyvzp.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gjaybgrfa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gfpjtxoej.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gbjiqttzb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gjucaxzjm.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gbvvococf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gosagfphe.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gyoikonng.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghqbrnswr.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gdojrigdc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/grqunptur.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/giyhjencu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/ghzgrlobq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gecxoadhs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/ggjtogkwi.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/glqzakjmp.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gdmyyxunz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/grsuwcqjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gpekjtftg.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gubtsgnti.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gsdkbfcme.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gajsjziln.sHtML


<!-- 参考信息 -->