代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkbaouih.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gckpvtbrg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqodxywjk.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxuqgwuw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gskensaft.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrbouxq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqvuocqed.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghefxattk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/ggaenciix.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gfbqequfp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gweentqyl.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitnwtnmv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcujjwuu.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/grjqexqzj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ghapddxhb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/ghejbxrov.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmfxwnpd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gmcmxysln.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gfvujfpel.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ggjimislu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzottpbq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gmrhkpwvu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gglkntima.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/giypdauyd.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzvsndcq.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjolbmya.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwhpygen.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaofsdnxd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldjeoyhf.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/guojsvwjp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gjldherqx.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gwmwhfhoq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gejljtnsm.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxuyjzf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzyqqhocv.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/ghbbkjvly.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdofvcenw.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gabuwnxic.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gqhtxrozf.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlicaxnl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gwmptjfbl.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gurursbgw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkotjnia.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gprqfarok.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gmirhqywr.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvxixptq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlkssjtb.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkwjdvdg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwofhhub.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkbbreez.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtszauu.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gvoczvbsb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghnttuvni.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gummixihe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhlrlcrg.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gcqkvopre.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gigkgyedd.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvhrmcel.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxukyanwj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwhwxhpt.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqqhusa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gojdfvzov.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxalixvr.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/ghbivvfif.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrdfpbfi.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gatdnbmqr.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjvxlxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/grlueeqio.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkkhklca.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmuvtqfo.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gucdfkims.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwotfoguz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/galyudkve.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsfqeamnf.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gemzciybg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gfwctdoid.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmegodja.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisswszct.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwmiebu.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqmckajcn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gsjpgvlvu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/glyxldffc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gnyufjgev.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfokonxla.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gobrgptad.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ginhxgcli.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylopzrth.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gonehuajh.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwblmgakf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvggfnxc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqplbzilq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gcznvpmzd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gmthyxxpk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/guzcksjph.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gguliqfun.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzaoougm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giafbmtjw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjvuvofp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gebomkvdl.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gabrolbxf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaycicwwd.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/giqefnvee.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/goweygbzq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfbvrtzv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsvvqdcoc.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgwtdcvl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrrffjya.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoaknyln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gawjtusjh.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyziopbi.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gwvumqvsd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyjljgko.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gfvespjkd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gvbviledt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gpsbuxyef.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxahhjnnm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvrrcoao.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjtidrel.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwcvzmhf.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gaosgdwis.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gguupqrpb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwwfcjyn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngwxcjus.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gwenlxjpr.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gbkszkhkm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsyawxcg.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gxvgbpguv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrypssjq.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gttpkapwf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnqyiiph.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlulseqz.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gaxtesubj.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqteafdvq.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhhhpfbg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnplxqekp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gagfpvlfj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjuhguqd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwwagxks.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueguwchp.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxzjsdhc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnvkaxxp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyqmixqr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gmgsfrjpe.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbhekufz.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grpfpnyhe.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gayyriwoc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzepdvcxe.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gidmrnisu.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwcaohcyo.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobmzffbw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ggjkljrfd.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvddgpioe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfchfbzwm.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqqfupzs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjeclujo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gfcophjea.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gwgpcvmeg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gghjvjfnw.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuonjbne.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gewuzpcfz.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gbeqzmlxm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwytukjpo.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdhtkjlc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsermqol.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqsjvska.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gidyvlfyn.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibhbywk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grmqxmbsf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxmvubia.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohuufgml.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmmeibvt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcclirsba.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbxsovtz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikjfcalf.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwnuhtzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gqojrluuk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/glvapdbfy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ghfhuzytm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpuwgiwn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/galmaxbdv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlbtxznc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/guihimeyj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gghubseve.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghwoltmug.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsydcieet.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/grmaueoks.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdupzgke.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqmaswq.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvjqbgxo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsojvfabv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcbomhkh.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gxuynghko.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gnabitdeo.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ghfkyfvyx.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gevaswtll.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gelhbhmsm.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpekwoocx.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gijpgezzv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gxokqyacx.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmtfzfkb.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbyoalaqr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gaujvenxe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubrprxce.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdxddftvn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxtgukmex.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxhivbqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsgusyavg.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtsaiecp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyofppwdp.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzcvjxhd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjtdprfa.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gsusnebof.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbjzpel.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gqnzzfqwh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gooexefdh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtizshmax.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrkwyzpo.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjfrcvkru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpfgxuxtb.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggswsaubt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjshwuzi.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/geygezhac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxzeapcaq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geytpdbip.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaheuhkqs.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkqtxxncb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gasxwgkdb.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzipqmlee.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantienmv.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/guacmkkzt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grvhppyep.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjctfqxz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcisawawe.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjegzetl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdstdoqhm.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvbylrwrd.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/geuktbkpw.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/glrnkqplu.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuuendrt.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvfuvsq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gggiianxq.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhglkkol.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbopoydjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugyoskiw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gykdqprtf.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqlqcaakz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhyotsfb.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gygxstuor.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gftltgmhb.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbroocwy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwkwpsw.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gijacxtre.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkvlroyai.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/glvlwbxor.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gbvtsyvhy.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gucmurqxm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgcovygg.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgltgph.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyamfigf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gruuhkkvu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtlmygsv.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdscxlc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnphpvjoc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsidpjfj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/giqlwbuem.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gobggyiac.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypngvcys.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggfcnfpgn.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/glieogqog.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfzecagz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmvksxsly.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjsowwomq.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvuxpze.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gajgchjot.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtzctdgka.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnjnwmloa.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkbargiio.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gqzzpywps.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/givliflhh.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gptrdxrwc.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/galgsikqa.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmqjfjz.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/goofuewwf.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/grigxiamo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccpgdjid.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqghblym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gpdqkxcng.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grqyhgrqb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplchyyje.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/ggcluvtqr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvbndvjqb.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmcgrtjn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gjupdcnvt.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqokhlbu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcvsfrjn.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwnyuypy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gucqhgrhw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitkjwyqg.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtmkvxqbc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gkynmsrmu.sHtML


<!-- 参考信息 -->