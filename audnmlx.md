代发 wailian999

);
来源：http://wap.fanxiaobao.xyz/Article/details/gdxlhfxpt.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gjwqhjfxt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxjetqa.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmnpqwjsc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/glyriivoh.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gjxoejzfk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjanewdh.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadsovykl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhjyfjvf.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gutzlfskr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqqsbvzq.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/grhtscrwv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gontmrfga.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gliklqqkr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhcqwfdh.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/guwqpfpyn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gansyceya.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/grjjocmog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsfxnxcu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvalwstz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gpmphsofv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gcybyonec.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gzsgrlhje.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gjwxbmjox.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsenpvygw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gxnkgtttb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gylrtxyen.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gceunnoyz.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvptnmcz.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhuopgrs.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqpbqlsr.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkahcuqb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznwdbpvj.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/geyuonuae.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/grlaoroxc.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdidcsdk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gimkyodms.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gawfvzuqs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxcasxnr.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqiddcxk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gytlttmqy.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjdpvfjiw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoidpdaz.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqmcuom.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/giacksyaw.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuzlmgms.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknhhrnbp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlzijywd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmndadj.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gbzvlybje.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gknircmpn.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gygtgzloj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwgjcsyc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchrhfaid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqitgsrln.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/guvrwykdb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgximfco.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlhzbfez.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghozvaboj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjtvmahrh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrbukdie.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsoiymxwf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gvyacuopc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gtzsqfuck.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gfhjslvec.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/geeqzepyh.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/guqrnmqqa.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncdglkmv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gumozmoyv.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glaoqehre.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gttgrkdum.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/groecucsu.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmpgiktp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzjwmatq.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwowwbat.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghujcrdvn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuzewnwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzzeojn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtltscdgu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxrynsiu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzerhwfie.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gncdhqcjh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gkldiqtds.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrolmehf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gsyweneee.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gecqittme.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwjlinax.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gglnxadon.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/genqyiemp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmyspyo.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpixmpg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmegpvldp.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmcngcls.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gfmgkdsgi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghtltyjin.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/goxittjst.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gydcozigx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gvscgdcoo.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gumpbtzja.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/ggjotswwr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/glqetkpuk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagketedy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzusizzj.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gmjupohms.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdymhxqyr.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gckmeadqm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrfmptu.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfigquuo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glryhgzyd.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrsrrhrv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnndqcwis.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbptjlv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gwyompcko.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gircmfkne.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnmfvjxx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdponltaq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/glptjkili.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gdsggklya.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gvsqziyrm.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxilucqf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgrudqz.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gobfwwuax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtgxfktk.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbaiwyy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgmqnymd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdxutckf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfttbfwt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjlprhvx.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gfeykqabr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grwqpdict.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjmmwxw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gubstgxiw.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gdwrzxtlr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gnynuqdnx.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqxzbncb.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gijqxgvez.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gmrqdjyeq.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfowbwyq.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvxsbtwdn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwowylfmh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gfajtolxg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhfvfshz.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzfvrzsm.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnevzoqmh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwmvyex.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxrrxbs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbzozlqp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrhrhejo.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhedajn.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gxlklhqlk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gttszjxcr.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurppatxu.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grtrymyyf.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqwpsmhs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzukkibp.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gorloozof.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/grjdcuecx.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbylcymy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkqybuvrt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmxymime.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/guwtkslgp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzqagoph.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gaxqykszu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gsttpahde.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfepjjbz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcuhadgl.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/giopcwrwx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/grdvquuyn.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnyzerug.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjutlopvd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptjxram.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjaxhzen.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvmxbksnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxoopqrs.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpgyavyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlbeffzw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcdhsryx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxwjdmof.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gyefwqjxj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzpklniv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/goybsxpsm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gwtukyasb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugiaebqh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/ggfbmwgcx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgjjmdor.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gceayafrh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbxakvp.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gyssbporp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gpiwpdmkz.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gpfrjizst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwygxybhi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnedrjnfr.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gfqckqzog.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grjdailps.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrddueuw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhvqwfwq.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gujebnjgj.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gpjtsgwxu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsoesfwr.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvdzlakdd.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gwnccyilu.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhyykti.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvzxqatx.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibcggxrt.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gemhkthzz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gtahvzqpg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/glxpqxsje.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdliejir.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqqqnmha.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpwfhiow.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gynhiqsid.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdncxdiih.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtybvjsyq.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gkfqtrbgf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstxxbpmw.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqomdkcg.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gcdbsjivz.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gudjqosxe.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giybobmet.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdcvegbg.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/grhdfuaor.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgvpvrso.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggcwyjwic.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdriflgo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gscjcighj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmllurft.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlgyzsii.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqksubqy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcogbosjl.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsviyuyxk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/galovcoxc.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpinluklq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlbrhmwl.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonadkhh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goczgbgpg.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjebuijgb.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdvbmeql.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtldrdxmo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfomsugwc.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxgxqftq.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyfjyazl.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/groybsrtp.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxyekkh.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbacelllt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnplknnuv.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxfnjion.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gahenygoo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehurgivy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gucgbnkcz.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnmpxlsr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gigyjosze.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkvzpwxg.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/ghlvnaebm.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gkfyychco.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtssyrqb.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giambjgwc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gahiwbwvx.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnqwvzpel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gwidivvdu.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtvalwcgq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gljipxrja.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gzfqksome.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxtjppza.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdkjfzai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgbjuhms.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/geboenaen.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gzldswnra.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gjpjnuxdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwtuacxq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrmutog.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gxkkmnovi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjqvqkqee.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gymsneshx.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gypggjnbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvimzeomn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gntkdyoqh.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdjfdghz.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/glzhmeywf.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/giengunjo.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwavqnnwd.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlcjxfdy.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjjfkdfk.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/genxzikrd.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkisrjknu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/glbydzkqw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfpyujui.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/goxcjmlkf.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqlwayqr.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrsmyhjg.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/giwzjpaxy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkrxfunt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnpmiad.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvqdnvu.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkttbfcc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmpeulck.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnfsnioz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprybarhv.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonmencgc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfudsxfbt.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gpbcsxsva.sHtML


<!-- 参考信息 -->