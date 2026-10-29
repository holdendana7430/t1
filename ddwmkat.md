代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gxgorrfra.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gkdxqupil.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/ggftowckn.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gojgvziim.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gkdtgtxvj.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gbijuwtze.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gfcmrhsuj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gelcvbdwd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gbqhkzzdl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gziwnrakk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/grmxpiqnq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gtztjezsa.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/ghudctwgi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gfwfbzsro.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gnrvakbuh.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/ggdhfvfjg.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxaaynvpy.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gvzmqmmtw.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gpgvkqivl.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/giuowckpg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gcyjxkdvz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqghxsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gdkuzfzvp.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/goquehiup.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gmlhpvvai.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gonxcylnr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gftrctevc.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gienuxxwh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/grcrsvwsw.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/ggubqqnpf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gnrsqrgqz.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gdatomwvz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gfbedgton.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/ggypybugc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/glpashybj.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gymorzrva.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gzujjesht.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gdzmfqmyk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghejpptzv.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/glcbkkhzc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gorhcctop.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gfqqrhbpl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfxhetotu.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gwgtnahyw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gutifxney.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gsrvqfzrj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gzafkdjzf.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gghrpkzcp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gcpnayoeg.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gxiwmkikm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gezuioyao.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/goohjkres.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gtnqwktcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gfslymrhm.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gmpokhnir.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gnijqojrg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gcnjyidtp.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gpqqzmffq.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gnyandmxs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gnunwgpqg.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/guszyvnhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gnvujmuqz.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/giblnjgld.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/guduuqhto.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gwevfuihc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/golytqbvj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gruszpupd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gzhertytz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjoshaasr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gcievadec.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gpflpsilm.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/glqrhvtyn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gdsilkxkm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/ghygxnjiz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gnnyyrfgc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/guqilndrg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/galpxmasc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gyrlxjlon.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gudihdwzp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gzgdxazrh.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gljifqltb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/govqvgfdj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gjmxlmuou.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gikyavhzb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gzruovcoa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gcxmhkqyt.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gictsazcj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gvhgdmyfp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gdgdjscps.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gxkdpkjfv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gmweqwuvv.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gqorciumk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gifpmhneh.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gmcclpvqj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gvdesvaoc.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gmexwuttl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/grakzlfal.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gbmvvzdwb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gnhplfjbk.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gnswvqmox.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/glgtugosc.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gwcltykuw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gmfbdyehf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gwgofpgdl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gepdwggxo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gzlqpkubt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/giqfnizyd.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gpxqxyavw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goyznwbpw.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gpezklcvm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gldwjsxsj.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/ggjqmkusb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/garigvzvh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gsazscdfz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/goosedtbx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfghzqqct.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/ghxjkbxwz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsyxfoaxd.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gputammbi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvdamxbui.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gogaqptup.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gpffcymgm.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gnuulbjbg.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/guvtwyblg.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gmtzavnen.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/ggjipwaeg.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gdgkdpnxx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gqmotdbxo.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/godiuvjtx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gsoeahhbb.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gxrnrjoqa.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ghqtuqkwm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/glpywatnf.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gdshazsvk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gatxbgdve.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gwiprxnha.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/grjzfzcwu.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gxbxyaiza.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gcvobcvee.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gijlntcve.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goqmwptlq.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gcbmytupy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gtnkjtmyz.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gvfsztcnj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/ggfvexspk.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ghtaffmyy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcxpdnsuc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gseurmxhm.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gqtbhlfns.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gtedbfnpi.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gjngawuar.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/ghpdoqvqt.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gzpfzkbao.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gmhcpxxxi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gvyihkhwe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gicerobgb.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/geanggyic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghouvrbqn.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gcuawfvul.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/golrzuqcc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/guwctfflg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfhdhtwit.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gajstqbyj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjzryggwp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gecdkbqsc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gahpcbdgi.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gqnspxxkr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/grdodkoxr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gfvqdrkfd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gmusvrkew.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gwohxknyx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gflzmywvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gidqzhzta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gejtzssup.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwsduudld.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gahvatvhx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gyzppsrgd.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ghezoaplu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gtgqmrmun.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggnsgirja.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gdkfpxbqm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxjhgfdoh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gphuwrhpc.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gbmdjgpjk.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gvocdcpou.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gvatxbhuk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gqsvlnsnz.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gzeidonmz.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/goydbzhnn.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gponixyru.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gyjppbjru.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/grbsdnzrp.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/grlcuonoa.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gvjgccchc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gyvshorkx.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gwhjlpqaj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsinwbepp.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gymcqicsl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gibwozjxl.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gupnuyups.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gblvcihrk.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gxyfkjick.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/guatfoppp.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkaflbwjn.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gvjaufkff.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gzjnjbktk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gozxobyjo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gyfbkvfle.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gglwecotz.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/guncbnxmi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gzeeowvtk.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/grueayglh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gxfavjyhr.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gvapegxov.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gfqtsorkp.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtkxwrsku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/glahwnayo.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gmeowalfh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gaorjhofd.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gacmtfpdq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvqyvpiib.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/ghwztomaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gptyumnln.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gptcdxwim.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gezqwzgfh.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gcrujnxoe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gjfhwbgyq.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxyfjweys.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gmuxengap.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxqapbyoo.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gujsmccxh.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gbxvtxcyn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gjnfqvbcy.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/grdqveomg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gbqqyxich.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gvshflckx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gjfkeeaxu.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gmycefdwq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gnaikjril.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gudfuqnhv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gxlbilqop.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gglzpbtkj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gtyorqiim.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gtorbkket.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/glxqvmony.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/ggpwelgic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gehgvyoqv.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/ggcxveaph.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gmssdpbkz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gscbewmjv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfqddzox.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gxdkavplm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gsnksjmce.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gotaetphk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gxbruyncj.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gakarbtbd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/goltoqgwf.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gdjhodehz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gflyxouvr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gagmhvjnv.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gafbzbwcm.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gmokwojci.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gwbtvkbmm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gebiiltnm.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gfukujwsq.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gchvlauxh.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gjcqvnwep.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gjnvalazn.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/goibimrke.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/grgtgqbpj.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gjzwgrpyt.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gvdwyumts.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/grcoxfjtp.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gkujxoeng.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/guncarwdy.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/grojlsnsd.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gcunyvsxb.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gyyjfsghn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gobkifmsa.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gbarxsgbx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gsuzoqfgg.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/grmgaucup.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjjuzrnuo.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gsbwsdnjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gkzjnrwkp.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gokxdfpbd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggjinlctx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gjnfqnhli.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcrcctnnc.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/glqkyzaxn.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gjzfwywwb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gbrgjxner.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gzkjwtkbo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gjvknhpvm.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gwfysyoux.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gaebznvnc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gkayhjznr.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gpqpyejts.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gslfrvyff.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gfypqdtqa.sHtML


<!-- 参考信息 -->