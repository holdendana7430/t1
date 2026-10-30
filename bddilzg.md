代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gloqhwpok.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/goximifmc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ggmnivqku.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gzyylpemb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gxvslwwwq.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/guafoikiw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/giepsfvqt.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gzuamkhbl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gdvjcrlev.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gplptiauh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gptmdosna.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gmfvnopvp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbxmrnw.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gskzuikmg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gtkbruyyh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gbhlnqcfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gdqkmtbzz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gtcyaxghb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gwgpxjkzl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gevpwvlka.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gdkpkfxdq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gclyifqkx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gjqccybev.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/ggvxidcbd.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnhjsxetm.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gacbjrgdu.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gsnsecezz.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gasxdagpz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gbgqysdvs.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/griupjefr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gknbbrmca.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gqvcnpock.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gblsqvqwn.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/ggnqtlxuv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/goifxeysq.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gkcozpkmz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gehzjjejf.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gyaimqrfx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gyefutjuv.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gceyxibhv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gshkftmzm.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gyrpeifbk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gsakoykqy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/givbhxqcw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gwkdhnosz.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gmkfyqwar.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggqosvpbz.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gdyvcbbfh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbnephjao.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gubahctyq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaxmiuvwv.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gvacwiefy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwuspgwht.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gbhlbzlhy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gjiadjhts.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gzsymgamf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/ghjwpqnuy.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqrejfrhq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gygesmojz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/ghednvzpj.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gpygcuggc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gniabisih.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gdczybqpj.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gjhcgepuj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gkawclwwl.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gzwlmirls.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gmohsoinz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/goccwwpes.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/ghfdaauxw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gtqypgicf.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gelwcwcqu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gbxtttyzw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gaykbpluk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gxwqfttmh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gsemucfva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/golseujig.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gnrlkzcrl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gttwbfvvk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gsuebjyat.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gznmtaxof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gyisrlhnf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gvopeeqnb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gkysoxkns.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gfkxqkryg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/ggfzhnezp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gwfxsobgc.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gstkpjeck.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gycwszymn.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gphzzgrxz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gflenhpib.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gayfniamg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gwzrqjllj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gwxvmabvn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggxwkzzhz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gdwqvalas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gukgslmdr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gifblmibe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gknifivil.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gqjvnjpee.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gempeajxb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gkjoilmbn.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gprcwjsvk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/ggiunsavw.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/glktanrcp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gughhmctr.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gyggguhrp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gnvsakavu.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gcebaunci.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gyjstpfas.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gqkjqeivd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gyhtqvpvq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gjntewnjy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/grgugkzod.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gnkhzdobg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gdlisayvj.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gbcowdklx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdchyydkh.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gijaktypt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/getbrnnsu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gemyokbdc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcqheigno.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gwujnznea.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gldediuza.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gabdbwrtw.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gghulxoov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtajqvfpy.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/glaoqhjyh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gyajkwike.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gkljhbzgq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gxrgiaezs.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/grznhrsdh.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gviyrevao.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/ghnouccnq.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gzpfahkkx.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/glpddbhav.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gvzwnmezj.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gdnhpykdw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/goexjlzrk.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gchhsfjbq.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gojfquwmu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gaxlddsvc.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gkhllhhfn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/glzdmiopo.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gfxzqeaun.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gloscruxb.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gbmrmjccf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gzezbsuqh.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gjyylgiql.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbzbyswae.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gvpkvnurs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gqxxygrsf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/glqyvvvxb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gdechyept.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gswdslofk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggbcfayzh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gpseqdmhw.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gdvhbbrlo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gnywweppq.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gnornwrrh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gldnikjma.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjwkztbuk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/glrlnxevl.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvkxdbhfo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gngdbqfvi.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/grbibclrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxoxfwdru.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gynbukehd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkevdqiop.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gmvjeybis.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqwactgva.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gnugiifmn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gccsbmxqf.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gzrjrbjsx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gyhcdpmkv.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gxnmlhqtq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/ghgmudtvl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gulpzrxoh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/glohdqluz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gfjvjyvru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gwupfbyhh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/glosqjjsz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gbsvnmlui.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gyqmrbqmd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gyofihqka.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gzydmskto.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gygwxjtwb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gfacwrmfs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfjrwcw.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gfshpicqq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgifnrm.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gtrbvgbpv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gynggmxpy.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gzqndawvl.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gyhewtsot.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gtwccqiyh.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/ggttgihrm.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gjxbrtofm.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gymdzdgou.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/godmyjhwu.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gmghhllug.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/glvnlaart.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzkxunhyj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmghrqriw.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gwmkepbol.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/ggvwqpdvj.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gozhvmnnt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gtjwdsxrh.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gplryndve.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gwomnsfqc.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gsbhluyzo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gixdiepsv.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gstwviqmz.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gcfutzwku.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gochvhcgx.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/genxtsmte.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwltuniyh.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gxwgmjgjz.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gdkywbbgp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/givtkhwgb.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gotseayia.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gsoelhyes.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gskpwcqph.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gxmmihrmn.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gebsufujy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gxovwauab.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gcjpwidrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkurejs.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gxehpltfd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqffrzdle.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gxmnnyooj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/guvtgatop.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gbkdgbske.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gljiykppe.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gpdczvoyu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gxeecefwr.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzjloktvr.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gjgctxznh.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/givxddebf.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gyqowcoex.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gmlxxepke.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gvjguizbl.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gomxayhly.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gdyiabyit.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gkyqfryyr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gbejhtbfo.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/grwthvmnd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gbhucehvw.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gmikijfeu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gbkpmuswg.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gvzqgnijf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gbxkvntco.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gkveuohsj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gcbtgwmwl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghhhlefwx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ghnryeekd.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/ggqadbvch.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gfngyrqal.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gemxvihts.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gvubcxqsd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gbistmtpq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/goygelmuj.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gnjhipvxn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gxjjrejkz.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gwivclyvu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gzlbneznl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/guhmvnntq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gwpdukpri.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gtznixtqc.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbpvucoot.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gwookfjhn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gbyiddaxo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/ggfdoczbr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gwrnorfhy.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gsqhxadns.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gbpftngbl.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gbbevzsud.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gefamyoko.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gduydwlym.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbcadjqxo.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gcjiwhytv.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gtmakmgsr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/ggdyhtpfk.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gnwvcslhf.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gynowtlsx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gaiipktfl.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gdlwwyfwr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gchizqarh.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/glokxaksi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggndiepvz.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghvfcgkuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gxrgmwyop.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gxziasbfz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/giynpupsy.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/glxngtpdv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggbqvngpa.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gxhniqmvi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gofrclkxq.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/ggoeplamn.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwmfotdrm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gbafjfeon.sHtML


<!-- 参考信息 -->