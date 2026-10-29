代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gacvfckhp.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gyieeapgx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gjqkrmsyl.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/godljkugs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/ghmndziah.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/glnmtowme.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/glaewxlvb.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gpyxwnyic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gzensbwmj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gkclwxhts.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gbjjsteym.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gcseximqp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gmgqkbjyd.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gaamynsme.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gspmbbmul.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gkgnayati.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gcompguph.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gllimxjsq.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gdstwkyys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gaqeguxvo.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gbdgqpwie.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/grwpxvwki.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gkevwkcnf.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gakhmsagy.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbnfnmhln.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gkonkijio.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gakokfeob.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gnwpamqhg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gvvfcdjfq.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/ggmkzfwvp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/glgpbasqs.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gtclhcddw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gqdhkqjkc.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gsvxywvgc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gcinaldef.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gofeasgow.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gsgslxwmf.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gvplfwtdc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gyewdyldk.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gqqjcyakn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gwcebladp.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gnmelremk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwkzgecsk.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gsqhtizjh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gjbkpitbc.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gjqpufueu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfhuwgdbj.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gfgqpxhbo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gnskosvhd.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gurqagcrn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsfzhbczp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gangghhur.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gajvrrary.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/giqoauxmz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqlzwvlio.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gcnprnvrn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gzgqusmiq.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gyqivjavm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gemcepaqe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gehwnrnul.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/graktmodf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gimygirds.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gopjarrii.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/ggjodpbpe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gpropnrje.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gaduuimdt.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gmfhhsjyz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gdnpffvcb.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gytcepqzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gcibdvmnb.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/guazespre.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/guotixprl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gsayodbyq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/guqgnuhjw.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gzehnwwve.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gcyttkrmk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gppmrjqvi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gnajysbwo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gqbvvajtr.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gzitdehbd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/giqkfbgra.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gnpuyrmzd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gsffzhtkc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gveugkslx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gfgzqhlhq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gsjweebro.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gismgdbnh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gyjenzbkj.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/grtuvbqrf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gtaoxflxb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gkhwncpah.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqwukogzi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/grdekevkf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gattoviyi.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/glmkegkvq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gzokwjvud.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/ggrnmfmfc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gwutisfuo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/grnqmwxgv.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gngeqxqut.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gsephrecx.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gqbcdsfzp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gxtgicyqp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gbmznqwfw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcjbncfiw.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/glfgoawlh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gryabmohe.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/glbeerxvl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gfufqdgdn.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gujsdewnj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/goyxuotsy.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gplyordla.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnorhgngs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gruqkmuml.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gvpxkxnpj.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gtpvqfghp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghydeutgb.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gyeqgbsej.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gedskqcta.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/guapgkqov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggpqskmka.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gcdjkfexi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gpewkxcii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghlwanuzn.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gcobsjepi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glcfwijjd.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gevvifbtb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/grogixkvk.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/glakuwjhq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gbvakuwkr.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gbjgkfwkf.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/goidghwxd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gaxopsnkl.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gxmajajqb.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gnyocsflx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/grssderej.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gydbklait.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gbjdanhvt.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gbosfwpmj.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gokoercbn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gljmtazjm.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/ggiogfisi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gskcalaol.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gnmlvtakw.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gtffzlwon.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gahizsuut.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gxmliqenl.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gbdgfdxus.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwspzvfhq.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gjwyxlrau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gdayhtlzr.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gukyunbus.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gsmftckkc.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gnqxrcnwb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfxraqian.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/ggdcdygxp.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gaeqecovu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gmnmdnxzv.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gtuglshin.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gbdmuibdm.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gzrycephy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gxqqzzgwu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gnwmwxmaf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gltrbufwa.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gwuptkipm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfbfenjjm.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/glhcsgjfu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gargmlmfn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/giqwwmzdj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glxtlmqtr.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gdierpxhd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnmtibtve.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/ggxnxzmrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbbgtydtr.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gdxcvrjbu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gecggtxol.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gldwxevzo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gdxpqpvit.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gczaslqbi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gnukzruql.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/guyavbzrp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gvesxdplt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/giqvaevqb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gnqraiozv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gdxvxsqer.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gutxajwmk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gnekrccyi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzwkqmocq.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gvijdaqij.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmrnnirko.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gqrxdhwjd.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gfammxyrd.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gjnzzrxhg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/grrwaffje.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/grwxfbdic.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/glhiqmsrh.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gxdwpigfq.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gshibcdla.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gycjelpgn.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gwiaovtcm.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gxnqchfup.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gtclcdoxv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gokdqpygv.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/geauhvqla.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdwovtyeb.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gmbqjpumr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/goudcsgxs.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gapvetbdy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gnlpkrwtf.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggnagempw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gduznkbhv.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gvbstlsjn.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gscdbixxt.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gftpqkcmi.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/ghacghtom.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gnadkakzz.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gjlkuutkr.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gvdipoyts.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gdeayuirs.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gfcnbdubx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gqygyfokb.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gejgngmok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/glgbmaxjd.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfugtmzpu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/geajmkdqa.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/ggarlftrk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gxwludlth.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gxjzzncvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/ggbonpwxp.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gjffyuoca.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gkwqulfqg.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gcbvxhwuv.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gyouzwian.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gzujwpkba.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gliexjqob.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gkrbjhoko.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gktgnsrcj.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gpopoivir.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gsumjluze.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gdpkxqdth.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gcemrytbl.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/grzjipgad.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gqcvbvjgd.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gdpzcxhdv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/ghosvfgpl.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gmuprtvhs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gibpnzcsu.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gyadrheon.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/guwtxxevu.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gqtngekdj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gzwawhqke.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/ggulebdho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsosrwogv.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gmppvvqni.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gwkmpnopa.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gkkxxnwvr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gksuxwbyb.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gleznavac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/goymxsefn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gctcotdub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gjdmulugm.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gmsflrrqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/ggjytfqqh.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gyaqjngao.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gquqqzqsm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gfmpnkkgp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/guwemdakt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gifgecgiz.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gumexqhph.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gqfeeplov.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/glybuqrhj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gujtxmulk.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gqyypolww.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gfdipgkgp.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/giywyigbo.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gbzwcyecv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gzgchwnbh.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gxtavxkkc.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gchemcawk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/ghpqfyfqh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gajmfehao.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gxrsxvjnq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gqcrsrmja.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gtgblqkhi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gwhhjaqqi.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gbdseuiyc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/glncskdzd.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/grahtkjzg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/glfvbutsg.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gezhcuekd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmfughizj.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gjzgwvncc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gsvvyvlxr.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gujkkifcf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsicdllvb.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gautmtxct.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/glyicdjkz.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gslnncbby.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gioxyelxv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gpmlqubqn.sHtML


<!-- 参考信息 -->