代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gwirslhtk.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaewjbue.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/ghorghklj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaglrbvab.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxnjbsuy.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/grreetoso.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftgaugoa.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gclocypgb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdsxddtp.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvhkygcl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/glmntwzvv.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/goshbsvpe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gxyrbeztr.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwokajsk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniarshqa.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gjrwapqml.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxixseodl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gdobivrjh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnsljkpw.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gvnwinizt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gecvpxreg.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gfuwmhvtk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmtmgayl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gkivnprxm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gxplzkexq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gvthzimqp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubsvojuv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gpcihvidv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttnnbtxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gmxhuzgmf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/guxgeaebk.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gxfofmsem.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskvaoqjr.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gatcsjxdm.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhpwsho.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcjvpcmz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptssqprg.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxqmgqyv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtigttne.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpkobstrd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfyptoed.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gflxzyqkj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggylxohir.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxamzagd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gmurtfjco.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gydrmkbdy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmnqofbc.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gfwpljywv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gnetytzme.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmmnfeyh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gixodshko.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gevucqzuu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/glffpkvhw.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/grgctmpko.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbavinghe.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizirjpme.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gavcmlnta.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gcftuavjp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gntpugfrx.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gijigddsd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxllyxqzq.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gdtorjlil.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gpqculfxa.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/glagxfpkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxolkybwp.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gdauuhlfg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gboyjpqgr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/giqwxieyi.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gckfdbajl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gggikiroa.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/grgmeftnd.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpfhtnec.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gfptnaxsp.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghcldwtwx.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/grhldqkrg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocwazjew.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gfozfcucd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggsjchwls.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjiavvw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gelgwzyzw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gptyikyog.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grmgwszzo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsbsrrvj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhqxbpng.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gukiwqfie.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdjbyexa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gwacwkvhd.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsbhapjg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gyracmpzp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/geoloskio.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjeqasns.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gkodrghvf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmnttzwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gtpkvetpa.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacqxvgtx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjktnwxe.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gfztjanqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gniiukqdn.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtbrrdhm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadpqjigc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmgukpnaf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznmkgrzr.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiuaqlby.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gkqiwmkcv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmitlkqwr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfmgsbdu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gqucfppug.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/grieynetj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmglwgwlt.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfonmxzn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gwifclbgt.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcexkycxj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgwewtas.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcowzbew.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnvfmrm.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gzzujrrfl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkuswfjf.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geroognap.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gfibpevje.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gjeqtndry.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjwsnzvo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmugdjrc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gzonhjghh.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgccjdeg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzvimhbq.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gramhguqt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghyryoqdl.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gqkwwyswq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqvczcts.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutulujca.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gclqqpmce.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzvfsfoi.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxrxvkqc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkimnhxq.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmfgzbcx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvddxlva.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggchrzyxy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfltswnn.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gutsqnpxz.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/guuyypror.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gonrxqcph.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/giblippac.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/grwzkmqwq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gclkqihzs.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gochoxesf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcynjnijy.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gfcltjaot.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/guqovdomy.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdahnvctl.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvrawovwi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gsinxozoe.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gvmzeqavw.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqovfpqa.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/giejmiukj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvcapyxe.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaaywmth.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhzhhmit.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gznvcfmga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gxgedfqph.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gazjxjzkk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/govngcgfa.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjqlrrfx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmnlmpt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/grlnxtbmm.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgcyloil.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoifdzqb.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliwmjnbc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gtixjvfyr.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwhjpmyzo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gyiltzimd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgkmutol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/ggneuwrqw.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvrkdzbw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtwudwxq.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmheqxnrc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glphnyryr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grtqadbfz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/greiidbze.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjneopjhx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geqmrfeoa.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gscoumbfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcfnmnss.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gldkkekhq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gupfjbkts.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkzzwuwn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyxcocza.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvujtfzbb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqihpvbuo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerwilhnw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gaakhubux.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gikfamqrj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzevrdkog.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gudguyvij.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeataath.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkebsblel.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkskmzsjj.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsurfwfz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrxrlocw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gajlvgnuw.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/geajvykni.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbdnudhb.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gbhlwnbxz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/giectqcof.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisehbkap.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gsqoligut.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvplpszgp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gednsgwxd.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvykxftj.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgousksy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxkqohnl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaqoefsf.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnwdpfvl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsrwyddmj.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtbuvxncc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlgzcswq.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grogrbacn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkbvaiml.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gblggslyw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggktolldg.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gtrdftvtd.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gyildsedn.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gjyqsmyzd.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gcxekduiq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpzqbuslr.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeiaavfn.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhyfbdqw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gylrwposk.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnynsltiz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggfaeozcm.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gacppohph.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gujwswfkh.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpxvlmcr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geunxurmm.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmkbrbla.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnzbrrbg.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gksyvuhxd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyrewikv.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gsisdjdtu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcakvrqsp.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdjkksojm.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwnurijcu.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdioqezi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbcaymtv.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnptlnymv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwecmpnfr.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfxshnwb.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghkkhxeyx.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdopxpnah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmebsfmy.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghsuibrkc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsyhyjxw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gghcogryc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcdennzfm.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvfnwzhg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gclarbjxv.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gulkcfxzr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqbyowjr.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntggyznz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcsmjdku.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtzjgfti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gktbqdjju.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghkdobugn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/giobtrmwc.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwqbzwzv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrowktfa.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjuxckdn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqsmkndcv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/ghrknfxhc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gjrrkotrq.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gjgyjumfr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmqcjpxcc.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gfuphxhzl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/giqkamwzc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmqytxnu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/giycwpiim.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgoamuvq.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grkpuzwku.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gpvdqpjfj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdvfiaor.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsxlpuwx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzgluuha.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gcxjowjsy.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfgstnwgp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgofjxql.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkepyvgat.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/govqkrxlw.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvskxdlcy.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaxgvzae.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grobwtxif.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgitqgeu.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghbwlnyyz.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/grormmywe.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsrsxaxa.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiziefti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrqywpvh.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigchnaib.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmzelchkj.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gqibjokke.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gycwersbq.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggakxrbzg.sHtML


<!-- 参考信息 -->