代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gkovjhuae.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gziuwnfmx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gzujmbacx.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/geddwmafe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/guzgxxjqs.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gqvwikptb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gbsontsho.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gzyrqbcbq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gfnwwachx.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/glksltjxt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glzdwuckx.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gtaozmzqb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkzsiiegy.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gsmbhqouy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/ggpcqoevx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gdmxheejw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gclgmorwf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gigwbvslm.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/goayjxger.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gfyxiysux.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gqbpdkahc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/ggdkqugjz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gtzjzwrst.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gurzvqtui.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gywemhlda.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/ggcipytdp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gslnwmwiy.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gfbuydbjb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gssxsishr.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gpsykynlf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/geadmiykl.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gtbvrdssf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gvbkfeyni.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gjcardagg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gipjjiwjb.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gkmickncn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gsdedkwnp.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ggimzziyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gxqgaqlqy.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gvuxciomm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ghpaerpkl.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gwpkyhzdb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gvkdfiyyk.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gdgrmpakh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gmhtvygzi.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gtaqahvhr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfcdgfixw.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/ggckknozq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzljvmzfh.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gdykledrw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/giflaayqq.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcojskfjq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfaabffuk.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gcblbjaoy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwkbqbnyb.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gipivysto.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/givcktmam.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/guklwufle.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gmrlofszj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/grhavyapu.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gadwyndlh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gltpvlgdp.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gcjotjneo.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/giorucaen.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/glivqshey.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gqpakknjn.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gvbcopczv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ghupwouan.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gewrqgnem.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gatpchudd.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gzpyxpjdd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/guclmghvi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gkwbfmxvd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gummyafbl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gjolzeinh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ggmgnjvru.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gtjagbaho.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gdfvwynku.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gwgbnwbte.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gddwmbqkq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gkhnxrkys.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gpoyjuask.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gbfdxjgwz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gqrutevco.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gauapevtm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfiiwmbi.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gbtrfthyn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gsaynincg.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gsgukmmzw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gtqizbgbh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gttnoutbu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gehohwxux.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gbaxhfnzo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gypygagtv.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gtebqcoyy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gmiiwqhkg.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/giphsjrie.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gkdyttnpw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gedsczaab.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gxnunmbyx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gopsrpttj.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gvvbxkyho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gmsplidee.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gsshtmnac.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gfumfzsnb.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gutridpnc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gboaumpfa.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/giljulohk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gehtspghw.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gcxkvoegs.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/giwctlpvd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gazcydbgp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gagqttmvb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gfazrpwao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/goebsuefa.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gqcvlbhpq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gjlqenjfz.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gijfmfsns.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggtylqfbb.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gqovpxcmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfqslwchp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gokdrszkd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gzzndufan.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gypkbqird.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfzsmhouo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqezngaux.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gctzsqnyn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcjxelogq.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gwzbhcbsm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gpqkdryjh.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/givrsjhvo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gythleexi.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gksucgoxc.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gkzqqcpbj.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gackqpjoq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gsgiuppyb.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gmtnxpqnc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gfeolmtmi.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gxkctsflk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gbwfzaocf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxtwjuznf.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gjdsrbyoi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gasrqldtu.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gidiwfvpp.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gcxowpens.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gmqvbmfwq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gdumxborq.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/girmejaub.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtzdpyqsw.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/glqsxxveq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gzhgmlgvg.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gjvrpwcmt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gsubolqqe.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/ggcftvtnt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcwtvmhpk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gaceulezq.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gltebesik.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gasawazgi.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gzrzqmkjr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gblsnycrr.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gvzjijqkq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/goswqvwcv.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/glpqtwxht.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gcqxtlksz.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gksoufryj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grlykkrng.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/genhsambs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaipyaxsm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/genbfsnnx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gskjsmzxj.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gqijltevl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpxgwfrvc.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gmnpybrro.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcioegaph.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/glpimsbrs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gmojpzfpn.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gbjaisush.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvbswfkvp.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gavugwrdg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gctoejfce.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gsuchrabj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gaefpipda.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gxlsigndw.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/ghqvvyseg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gwbdnaybz.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/guskhfyzu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/giksxgijg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvomeuoav.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gthbgngen.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geqkqboqh.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gccilbgdi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gzzwnvgao.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gbioawnlq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gbdxlrvdv.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gdnxvrmtq.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gorrmamvn.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gniisczck.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gkgaopvsb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gnjjguwtb.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/geyradqxl.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gbeksqquf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gvccdgjib.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gneuextjk.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/ggdxlebye.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/ghxvwqmkl.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gbjwtmqtl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gotuhmaqj.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/giwmoagwz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/grfovunka.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/grvnbwdjr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/geacdoxlp.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gcdlvghiw.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gaugxkvqc.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gmpgvmddb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gtbyqtety.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gusdfcuef.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gnymfyllu.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gdifyykei.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwdxhotph.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gqwpgddol.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcgxujcpm.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gwqpfgvaz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gwptkyvqm.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzmcnwdhk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gopbcsryz.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/ghqnwbdto.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gmygqbukg.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gwaeebapd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gitxnocul.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gwhlbwymo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gcqqiwlwk.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gafrkcgqj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjxyzoblh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gdumhwguy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gxfdzyiek.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gdxkwetdp.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/ghiwfeoxs.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gtdwxqcpx.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gpgtsbobp.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gpgydlwdi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gtyfwkiey.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gfwmyqyau.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gdpfzkewp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/ggppxmlzb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gytgsvptw.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/grmonjotx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gdfcjpvvh.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gsqjcazrx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gavsaaeoi.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gqoyuqpok.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gwtkplcso.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gkivooelr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpgbmcemz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gijnsrtmt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gtanziean.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/guyoythcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gnetherey.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/goaangqpz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gbuxnpqae.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gmdqsnnbm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gqyneeate.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gyvfeapzl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gugdvckfx.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gphzzvlco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gmxiujmkj.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gygohfamr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gmkvymxvx.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gazfhjzxe.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gdageytyr.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gfwzwofqk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gtdexjcvc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gqwckkniy.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsqmkssnc.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gqgsnwvem.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/glqtujejc.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/ggokifiaz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gudnvysrc.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gblsnvblf.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjcrfgess.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gyfbrszag.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtglazegk.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gidayrwce.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gerbdlygm.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gzeqmvvau.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/grqifylaq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/goxrrasgi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gufqncidh.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gwmwdjenu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gbfnibaad.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gruibgjyp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gdovzmwgi.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gpihjcefr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gyhmfpnsf.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gtbzctmah.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghuocxbqo.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/grxolsrig.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gbkvummyv.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gikqwpsbr.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gsyxdltys.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gvfyzaxsc.sHtML


<!-- 参考信息 -->