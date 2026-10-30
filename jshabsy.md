代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gyyfswjfc.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gciwfmteo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/ggecuaynh.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/grmhtitdv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gfllbhbxq.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gbgvtkigg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gifsbphwh.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gcovrbsqz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gndfvdozf.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gsekalser.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gkggbsfky.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gkonhwsgx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbpnprlyw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gmeadwarp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gmvwgdlij.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gjnfedebg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gdyjezwfu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/ghdgwtkwm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gejmjjmix.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gmnihyylk.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/ggmobpxnw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gtqqiilza.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gibmeykpd.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/guwfujswp.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gtakcfqir.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gihnpgwzt.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/ghljnspir.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gwjtibxxl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gpfwbmtfy.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/grdlpucdd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gsitvwwrl.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gipciygke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gvojuzivf.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/guerkcwsm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/geatgxzwv.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gnfccdlfc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gvefndqir.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gyeuoswar.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gjntovcir.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/glqbrwkmo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gpgmuvvkp.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gysvmpcjd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gydecxzlx.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/goxodsjht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gwuzekawu.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gnhhrvwkk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnoyqpuuc.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gptwnjawm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbzacmmdk.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gudmigxbb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/grsuvogak.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/goawxixra.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsramvaul.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gpntxaxzc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gllstldya.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ggofimznd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/grbgvgfop.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbzvxbeqx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gjohjkzeb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gdslimcsy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gahbqmqmp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gtpxaimpq.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gzgdmsumj.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gnntzgbfv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gsvlwwcsp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggtlaxtod.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gulhnauqc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gvpvwpuwv.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gglxnjwbr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gkcrmezpa.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gbngvzevu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gczbyhfhu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gaggxcjiq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/ggpbgkopb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gyenzmykf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gepaofxwn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gyywmpswf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gxnuquarb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gsdgysoob.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmpwgapvg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/goqjrbimc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gsnbaeakr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gshkaidnh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gvtydeygn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gvmaorqqs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gxcgawnqz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gshyybovt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/glqaijkos.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gldsxzfii.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gmykrokcp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gcsqxgljy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gonlcylst.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gidsrhavw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gnppiqcez.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gbpjfziuj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gclflxjpw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjmvcmitf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gtnyooaht.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gdxnecpio.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gkvjnnehs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gnlnlrcvq.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gxvyeqdvv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gsaiydsza.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/ggzuxtrvh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gfkrwzveq.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gzucirhao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gdrpghyrr.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gvuwjrkeq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gxwubghbz.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gbjrsobir.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gprhbfwrd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gkhnjtlbi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gdgxddzkv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gplkrppdv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gbfqibbuj.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ggytrhmvu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghyvsrtow.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gglzvzxoo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxpsdcmfu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gjjnighmd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwyrzlfwz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gdivxujvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/glqyhnabc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfekmzvts.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gcbfuuiny.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gocdakphk.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gxfbwjfex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gipfwqtvh.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gwojiiqwl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gyguvxpvx.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gohsgdtul.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gkrhchvwp.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gugtdfimb.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gsiduraam.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/guxamfaps.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gzsguldhf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/glpduugkx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gykmcyfhs.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gpungzjym.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gkmebecnx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/ggyaoltrc.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gqhirkbwv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gjrixtlty.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/guomsoyrz.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gutaxhmzd.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/guvtqkmrp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gupkdrsom.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gscqnmomf.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gblxqlkvp.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gnlmgyylf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gytzbzuwb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/giszomqpd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gvrnkfhqu.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gpldnkfzq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giqbrutcq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gzycdphyr.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gwrmbnqny.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/grxyxqlvc.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gipbpofnc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gobvktwle.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gqpbziazf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gctqfxbfy.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/guhhaeizv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gniwjoifk.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gitzxzgkd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gghfflvpo.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gezydizsd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/geoahyhnk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/guzrgalhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdcwwnppn.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnbgtpeuv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuxauyg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gtbnqrwvp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gplxkgyve.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gqhojjuxr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gepdssbav.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/goiwiedfg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gitqzgwmg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gvmfghhdi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/ghrytweke.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gfxtgysuf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gahpecrsx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/golmcovbs.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gtrwjicyj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gajmorcdk.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/goadalziz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/ggzdycntd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gonvlxnua.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gfcyvyuax.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxhwviyrb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gdijxligd.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gwmiovfbk.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gzfcmtcrx.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gddkwsdys.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gdjolrywl.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gszclztra.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gacmrulvm.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gqaymabji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gjftdhicn.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ggvfmlywd.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gdnwzzgfn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gxobnabhf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gpkouemei.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gqlujgorx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gyxnbtmok.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gqspxabnx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbqkmtlfk.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/goeredenh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gjuyepedv.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gwdriaqsk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gorunytji.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gdgszhrin.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gioickssa.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gdhblhhhn.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gaowxebdl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gfdlvgtae.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gvmpfgydn.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gilufjctf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gfwfjyico.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gwbtumljb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gdlhtcuco.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gvbevwlpk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ghpwllwip.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbwoalerg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gncfyizpp.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gdttsoisj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkbpoyrhf.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gabkfomxc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gqaarofki.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gxlughldf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/glewszwjs.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gjvcncehr.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gjbgalkqj.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gduhyhyqu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gzexinynh.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gdkqxokgk.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gljgqjawo.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gvyotzezy.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gcasmxrpj.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gybwrxigd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/germaasha.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gpmtpifbk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gexlivwua.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/goerguwma.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gazqbwilq.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gzwcesgbl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gokpirmpe.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gcuynwsxc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gbrkfhqej.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gnophkfsj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gxdatoagg.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gbcprrruw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gicvmpire.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gckzjffjc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gdqvbsaxm.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gfifsynmm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gxqrqktda.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gavilaqrf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/ggraazccd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gdorlourc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/ggouaqcpp.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gysqiepow.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gohxgzjum.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gpskllwna.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gtyglxpvv.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gacyanklx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/grqrvjxyc.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gzofoahda.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gevnzroxh.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gntcsmhlr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfxcfslnv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gtmlzcdwf.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gomxuuakk.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gdsdefxis.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/giksjbrsy.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gjpppdimx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gaponxvip.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gclgzfzcc.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gidcdbmwj.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gmaespxwc.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gwzzohxog.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gzajbqjnh.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gxkpgtjym.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gfgrophiq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gxllpubro.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gkahvihbz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gkhcpuxbi.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gyqookcvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfxyrmjeo.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gnnvqchns.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gfjjootxw.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gfrnmmnsq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gfcuwyeyk.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gbusfolrv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gwrgjhhai.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gvrareukn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gnkbmugtf.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gnyehkfsc.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gksstfrxj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjmywmgnc.sHtML


<!-- 参考信息 -->