代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gnplesnwm.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbaqtdbg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdtbcqxbt.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gygbepayb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwokvamz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gemcfiiia.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqabmivnl.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gcnxgkfpy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqaifax.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmqrilvd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyvypgur.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gjemxejxa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gsosleuxj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpcyylpd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gxihzlvtx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gexjjsngj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmomrszvu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfpschwe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gmhjjedtf.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhiuylzz.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgwvpqwp.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyapkkcv.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacjfadti.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/guiphqsmd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/golohjgkk.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwvponep.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhnfnjmz.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gunpzqtgv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/ggtheewja.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/ghrxfqxcj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtrrwmovj.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeloglsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gkiaeprrq.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcajkvkbv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gytuvsogu.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gaghfanid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgmzwrq.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrqvyebx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzhmvohk.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/ggfwllbba.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gdesdjrig.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjnsubvx.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaisvhqy.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gpjobepwc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygbvhrvx.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gtbfmgzdm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfyxjjjs.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyfaicos.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljvonadr.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/graxboezx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyliljeff.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfebftsbi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgejzgik.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gacqlfhum.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvulmhuuj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqocexix.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gvfcwxacy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuadegwi.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpddoffp.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/glztpvmkz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrjlhhyr.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqtsgrrb.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gekwiepwp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaknqalmf.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqcoiima.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gekvfnlqy.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/ganlovqdg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbsfiluj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbhhylry.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/grikeevnu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gubagmslp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdikomseo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlerytez.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuitdisy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gozpeblfz.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhomhceh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gihpqjkqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwbynwy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gitsotntr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gngplgfkg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gwjbaakxy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkunphyw.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gokxccpup.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gysttyeid.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqpcrqtr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkygzofk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gutbrijni.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gclawiixx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gteskjjku.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gfyawmbza.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/giogmdcwc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbmlwqrz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxzlntxa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzygkcxm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkxapfbd.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqfvtzti.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gqebtquin.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gnbuzstkv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gedypfexm.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gehfyarrs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwavxqvew.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gludqqyqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdiupptn.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/geyiyoimo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiaumgjr.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwtvnqvl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdqotsvs.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gqrcqjdit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdmyfdqo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gazxrhjmi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gydsfdjff.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gkxwagxnw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goysljjnb.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtjtvhkxy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gkaangmad.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaooynayr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyihqkbm.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/glscahprk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/glrtijtnw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmiwpjsr.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gqlmipzjl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gilecydwe.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goruhfquq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpmrtozp.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gucvzhtmx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwvdvpni.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gtvapvgdq.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnpseozz.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gaozgmmdp.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcppxfxwr.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gflmpldrz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gndhohmht.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajpnqfc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazpwgus.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrnkhmuf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqlnkpt.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdettxqhc.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gybusjdls.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gkkzzlzmd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqauinwvr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcanombpx.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gxleyiiia.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/guwfvbyam.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gecrwxfhx.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsnonxck.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktpmbvks.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gnghqrqew.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gpncbbonc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbziitnyc.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkdmbync.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqeysjrey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/grbkkubcv.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gvybqirda.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/giurnchwe.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/grdnlpkpa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaopkuhj.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gnxjobsqr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gzqjsylca.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijkeuon.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gxelwdkvi.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuqbnymp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzfbucafv.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gexihzgkg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gslodfpcu.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsnapeix.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtqejeani.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gakiayper.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefiqzukg.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gpvwlocxs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfehsahtx.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gbilqsars.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxbwjkrr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyoyojmx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjaahbsd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkztayyu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkpbkzbx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gwzpqikcw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gcefywdcj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gogpcpkkb.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gecnvculp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwwtsenm.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfryfcvam.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpsyznza.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbbhfgst.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gejlepyug.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gujbgaohy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqaowsrc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoseugbj.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmzhyat.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoyfdahy.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gkptldoho.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskbmjned.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gqprjtoah.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcjfunrmy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/geustayqn.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqbdisx.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gynxjdrqy.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwffykyfc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqppfbge.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gibrpyquo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqobbizem.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmgsyicjk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfcnebiuv.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmptemuk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glvnpunda.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmyqezga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsuiselvy.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnwfbzd.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gcpswbfnv.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gafdpccek.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpifdohtu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ggncmrnxc.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gyhuazyrq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getggrnjh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwubimunm.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gplskaxzn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqcwggyf.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ghxzlxcqm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjvldsmdh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznssyyoy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gykvniycf.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdjuoaklm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gigucgyba.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ggtsxqbix.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpzxpkjqc.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbtrhmuzu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gufjqvila.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlpfbnxx.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyanzllnf.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gbihfdeqp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdtxeapik.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gctcbsftq.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnblgmejc.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfoquxfi.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyixdiawb.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/giablmkuh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghhkhurvu.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gboezblse.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyejblrqv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmmfpqn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghobqwhug.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhnfbezt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gabwvsimu.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gduelhzkm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacuvbev.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhyqkfsi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecmrskqv.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfukbyytu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/guvsqqutd.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtriijsbk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylysrmnw.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gekjzvgzv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqicsyxts.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gkldkhtqr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gorwiwtqu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjqewkhu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/glgtlbkjg.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsowmzzr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvcodvel.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqshbztm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gbdlhjrxa.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxrhebpy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsimmiun.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gikhonlvn.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gslkuqnan.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gcgxtaxut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfsnkprv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzysdogxh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxdpqhff.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnqyjgkr.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gauznvchu.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnllchyrz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykpbotla.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gvkvsauqn.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwuixaqj.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwtboxrru.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gnaabpkzi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvfznzwr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclljgsmk.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidnuiprs.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbqbqqe.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gogzjvfoc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/guhhugzpu.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gntmrszoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtrugyklf.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gzdzyyxrf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbuypzsa.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvyaejsq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gflljrysy.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gewrcnnji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohinfju.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/grkpyyqfy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggelzqwbf.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpflnasx.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaxenizh.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gdudvbpza.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/glyswudvv.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdkbqtibc.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwduwrtg.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gkeovmgjy.sHtML


<!-- 参考信息 -->