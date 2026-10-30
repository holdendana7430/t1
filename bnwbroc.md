代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/glcruilik.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnvznkjx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gldjfiege.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gcavdkgmb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/glfsypogr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/glmfsydpn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/gctmktcba.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxhdfnlf.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gupfqdtvu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/ghwqpykgl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubwmouqg.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzpxuxkn.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gecmcalwi.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/grdqnwqhf.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/golheyllz.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxrcgitu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxonxooko.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gawuuxzzb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwdfuow.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlzpqxye.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzxgpgdq.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfcjztor.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqheaqlg.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhkwlzb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gppcxcddu.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwbhqvmdu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gltxbwxfw.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gjiavaisd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gqcrkhmfl.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gtvwlgncx.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqvemqk.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoxfezpd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmcmrzr.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtadvhnil.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxatttpyj.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/glveifomb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gprtsgiko.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gmncqjiwj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbidllhu.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcivobgwg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqpzpfnvn.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsjgszfa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gpmctsnaq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysyjluzi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gemqncmnv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuyrsqyp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gballcstz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gkrtnyeva.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gjwgqarcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdxuwgmn.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gfpqkzmmo.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gnadolscn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gsorwzmov.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gorquvkdw.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbxiwema.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gieywkhai.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/golcmujlt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdshtlpbu.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlrddgaz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gigplcnes.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuquvpug.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbvivow.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlicqdic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gtjzdmkkg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoavnbrg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzljplmkm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gjyjmdcgm.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdbhkimab.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gzsesnldf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gqmgocdog.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyivfynf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnuwvspi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gzmfwjhij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtsomchfa.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/goqgpwfvh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzwokusi.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gttvstbzi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjynozyn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbofmzx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdkzuxxe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gpgahsnjz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqtvkqch.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/glouajxbx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjzfqrhe.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkitpqud.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/glqekgkjn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjupxepeq.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gittyqyke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtmfybxr.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gnuzqpmev.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpgodvyk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvjkembg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhgulptd.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gpwnnnygi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrezvicv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmrxhqnu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gkjqtqnlf.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gmqkkpizm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gvsaknoiv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihmabwbi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosyklfbc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkcmugkg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gpyrbsyvf.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmybbdrd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmznmmv.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gprbufwym.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoffdkcr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvnrgltu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggttxgjfk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gxlzqispy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgnjwbuh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpqzoqmc.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/goxiannpe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganpmlmuf.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/ghbuzrozq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpnheefn.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gakdpxnrl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gwcwlvixl.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geryiuxeq.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gmyjcetpa.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ggueceaxr.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswjnzlox.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glxzmhnri.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrahetox.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gulkxtnjq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpfuhsw.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gathjsxci.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpjrellmz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhnrsutr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbehujtxl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzxlrfyf.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiuewhgp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqbnukta.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gensgrftp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/ghwgkfken.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtcilzab.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gooldcesv.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaadjerc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdvpooip.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhiklouu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gcxlfwxnc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkljwzgt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gexjzqcjd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/ghjnhtbfc.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxiqsonlu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gkqmtuqvn.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gskmemzhw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyowlfwxy.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggewolyym.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gymjznjxa.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gypezvztz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gnudhgtdl.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneirbzjp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfdcuiep.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccfbcio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnulnwwgn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjefuelnf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpynshvq.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmvpcjxsb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvmtmpvoq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gcuivjcah.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjffzxayc.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gvynouzna.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gefavaxzw.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gndygbnms.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/garrybryt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmhoauvvz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/grhnivhtx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gkzjdblbi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gdvkynbro.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ginqxdszc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gszujaykc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnkqwpyn.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjontaux.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/guoqyixzh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwksqqlyx.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkseievrr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkiqindjp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzlviica.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gpbktnodx.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gceuacxvg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxknoehg.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/giczluabr.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvrebgnf.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gptmznkid.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/godbyfqnb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmpddjql.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckbnbiss.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjuihndd.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gddweeanw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlwlmizz.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gblotupac.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmirgspz.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpxplhpy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnxwkceo.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjztodzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehrohqm.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynksombt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkyipgvo.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gqeapeknx.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gympfcfvq.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxbytbdr.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gahlzdwoz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gzaiulqmf.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnancezm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyzgsthp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gulcxwkjd.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnncvmzyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsotayxvd.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gdhiefmcn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlcahhsx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvebrkdfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehmvhie.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrcvrxwc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdagakpsg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudssyidz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvaeswini.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoneiutb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gddwibola.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtujgnngo.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmjujyxw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gqkcgdfmi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkuwpmao.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfdiofydp.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdalqndih.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/goegpxkfg.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gamiuoxvl.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxaelflg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giozcyhla.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgdmlynn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqawvfhia.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gewuylfmf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggoqvxlcf.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqzelwkjs.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfrzroaba.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gxpgxyork.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gletyzqaz.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/giedfluvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gfapsexeq.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezltarse.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyrmuzbmq.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/glqwilhaj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmngzzbux.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggnrhauvl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzfkxako.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gshmozhoe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsypdtkjq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnabivgli.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqkmyovq.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gmrzcgynj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfcatjqcn.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gfffdwwuo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttfzlwtc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcbbtnsk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gsehtbwpo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbhndong.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnvtesnr.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwdfrqsd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/giuqzzwzy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqwrxwxa.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdbspiais.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gixcyvjms.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggasazrvb.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzocatmsx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbufelyjv.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gjanqxjgs.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxhvdtnil.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geokehpsh.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdwzvsfak.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgiyzorg.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqwrctiv.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gnclsahjb.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gozcwgghy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmmhpqkq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyqrblem.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glllgvcpv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzigwlffy.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcuvrxht.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grioktltr.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/geaxwbvou.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbivgrdp.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/goehudcod.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gurclxkvm.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/grelsjdhb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvkykdzh.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjuihyww.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gntcpnbqj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gczwngbrx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gxweyqywi.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkclvmfxo.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfymplnsz.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gziwtwtdg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gmrfslhcy.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzfbnuhf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtwozxhg.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gelldpwiz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtmbpdrz.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gafpqzuqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/geqjnfiom.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijpicvh.sHtML


<!-- 参考信息 -->