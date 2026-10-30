代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjzijvtb.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvtzoigk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gydkzfccj.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gymjewkbs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gqmmpcwtk.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnkfxqcl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcsbowm.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbzklmde.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgfjctnc.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gdfgadnop.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorcbjgab.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/grkxmafrs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqmxnfna.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzyehgzp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/grriqigfn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/ghokcmkoy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gjqvgkajy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbjximik.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gapoaujuc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gnmivjcqx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/goawuqjuk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrorbta.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/germzqobr.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gehgxxncz.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grovwkolw.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmqdjvc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqcnfcgm.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/grrlpihwi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmaitxsmn.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/geilyosmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gqqksisbl.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gmbjbiiyt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gblrabqtr.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gihuggcwf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwjojlies.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/giagmqhta.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuajpllb.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gyvykmema.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjjgryst.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpgnytsm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitcrgbk.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gwapkskfh.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxiybtjbg.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gllsojhjd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gqtrudzyr.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrmdeyks.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gphkqvrxs.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/guqvaeknn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goeyzufzv.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/ghpermvzp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwbvdanw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamnblomx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gutlcdnpp.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gljqkmqok.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gggvsvbxi.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gddxhhrsg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gscxrnerp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gopkbkryt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgivexsl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gyliqacsq.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/giowcqltg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/goofmqbod.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyfvbfbt.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmowgcxd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqdihiym.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ginxeqtxa.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gyabtbcwm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqwqqelw.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljnwtkcm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gpfxiivev.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyemefcd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkoepruwi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gexyyyyng.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gazxzcspm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/ghjfmjxxu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkywmaheh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggycaeyvj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gvfukvavh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwpkerjm.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gcihmrsai.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gznzcjnyr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gyarhwzox.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmriglbma.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqysueyjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gwnjunfbq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnkpwsyg.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gcatxfdzu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gviwxbnfl.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnkibkjd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpotbmnq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpdwgdecs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbqfohuq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/grqjpnhjs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxnenprj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvblbwmky.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamgqivoi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghpmlvlcx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gutjatizr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gyawarojh.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/grzjcehve.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyifilufk.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/goocaqqzi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/griqlugpb.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gaexngwol.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gustmfxap.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghziwdhvo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmsihdi.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnhagsph.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscptsrgk.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjuurlan.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqbksgto.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gynouulyx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gdhyovzon.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwzshoew.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxpgyjz.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/ghlxdncgq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gldfrzihu.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrizytxu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixkahhbl.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxrszme.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbywamagn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunkgeufy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrmdkbbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glhdoiqsz.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxtmeagk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdfeepyl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysolcjwp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnpmhozn.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gubulvdbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gtuzkfvvd.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/grvfufmxw.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gpbkmrxrj.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpxnoziqr.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbzijxvd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpdkoqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkscoqhu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpzumlft.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/garhzoavx.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gnmmrexwt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjozpvntu.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtxjwnqh.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gqcyjdqxx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvmauvea.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gorggnzqy.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvlnrgup.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/grvubtcse.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gihtvhafv.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqfqbtv.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gorxovxre.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gyrrzpoij.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ggvxlulpl.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gbheyaonr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gbwdfvguz.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrlyrqey.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzclomyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gfwszwsrr.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjsrurkh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gvxfmfybq.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gbblxrtni.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gplhygvav.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhovqexs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhfpmvk.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gnrhmvjpm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gkmuwemnp.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmejuhms.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjzpmqfp.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwqpyuo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gguprkfhw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcxbiazr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gownmvseq.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxhgafiu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdcrmmbc.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gmphwdswh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsrfjrib.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gknyvtkop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayhamktn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/grdsbsncf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/glyzaysnp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggvujbvqe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gcfqduwtg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzdsmzkt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuurhdck.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzxobsgs.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/glbajpmbp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gouodavbd.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzcvbglp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigivzzyq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/getyodyyi.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvfaydli.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoujkavh.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/giquemqij.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gsfkmbpaq.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gvhusfzkt.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gwrxgnkec.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzesqyccb.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigociwek.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqqgpqrx.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grboqkpkk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gkbpcmcxp.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gssoxduxp.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glvroogug.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gxctxabvj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjgwqkik.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcgksoje.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycjcaark.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhdckzme.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtpieqbq.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyjgqdm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpnduudmt.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gtlfsteeh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgusipop.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbrhtgyx.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/ghalscuvf.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsuvidmz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqebgriq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvjqzkwc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gtptfbqsw.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/guaruagol.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/goskeiyoy.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glevybhhx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpgagbtjb.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmjkqdpi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghsukgnkm.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guynbhgip.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhvbjslz.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugjymgzj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gapeiuweu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyfmmfig.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gshhxveli.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkniszl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwwslkmr.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrgfdrar.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gazdpzwkc.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbandcolb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grvokjifa.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmaspgep.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdthtzikd.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gglkolhxd.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwjfwgyc.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxraehymg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcubjjpob.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmgejmnb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyrnxwvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofudaryt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnslivnk.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbycqhbli.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjddtclfu.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyyrjxob.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gmczxhiyu.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gankgdvcv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gpehhfgbp.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gutdxnzdx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbjxaekpc.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gdlyvbvtb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrmuwzsk.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gemdvbnnd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gncsadmpa.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gllutzrux.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbuuplgoo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gzckynkez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/ghybmalgm.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gruvpaipv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtohucbuk.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqeukaox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoqecwbp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gffqfafno.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/ggbigkzat.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukkwbdxl.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geteuymcp.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxiqclyz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/glnakdmjv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gnruaqvuq.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gsinkmvjf.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghugbaawh.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gnplpkcty.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyllxppf.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/goovhasyc.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gaxlpalhb.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdyfokz.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzqgcjrvq.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gtucslaal.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gzwrleisl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqkvqpgh.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gdcmdbrvn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmpmzuco.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwyfqjep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gitvqbpeq.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzuwlbvih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtriahyti.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsllzuvzb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzigvmffm.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/guusjplts.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/grlfaxohb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghbcahxli.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypuwxpve.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geipfanfr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaomiqiu.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gxzylgjnk.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmfixtph.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrxyiiby.sHtML


<!-- 参考信息 -->