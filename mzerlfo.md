代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxtpqlyyl.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gpyxktjtn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gquatijud.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gzetyjmqr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gduubkleb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gptsnfnao.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gscjwyrbj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gwpgauniu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gedmwjjpk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gzgimvjzb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gmtvbwzta.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gihykfeak.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gxphwfzbr.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gypkepujc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gytiuycxk.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gliykcxwx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gveyzzidy.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gharvflta.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/godwnhpbk.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gluqybbpe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gjccpmycg.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gcwxrexcz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/giqmrwdrj.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gzkyocdol.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gkwbieknc.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gnnjwbkun.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gonbcccjb.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gxpawwvoy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/guuebgvos.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gjpharrrq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/garmjfzkp.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/ghpuegnio.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gkdhaamtf.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gpxwlsvqe.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtrkzmbpi.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gnugshpus.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/geyblhikp.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gzxieyolc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvwpvnmrw.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/glwfoggck.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzpznktnr.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gqkeseunf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghbxsfbxw.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gniafohhv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gkpyudnap.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvqgyyacy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gwcqpemxe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/ggguqyvux.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gbkprgddb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gtcncjrmy.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gryvtzono.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gpreduymz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/glssqovbq.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/ggjfflbzx.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/grgqkxyke.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/guynehfud.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gxzmoclnc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/giornjsoo.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gijjxnhvm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gdalvgwbg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gfhhtewzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gpzzgfuhe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhqdevt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gmkukzczm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/ggrvolqjk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gcfmbjmey.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gzywhboke.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gaahjkbel.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/glbvjmssd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/ggjbyqkua.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gznjzpnpf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gjcruyqdw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gwhrleqfj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gpwffbued.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gyqyyaeva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gxkwkagwr.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gnxbykzvt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gwevizvbs.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gbmyachby.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gkonjzkfc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gvtfpdvgc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gzrvlnury.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gngnztkoz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gobfsgiyw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gozkaglem.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gpzkiacqm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gsveqatji.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/ggsghlgzr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/grhkjohpx.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gtebrgpys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gulyquxor.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gsdcainju.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gkxwpzlbc.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gpteqlykn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gpyzqryxx.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/ghosanpvo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtrazvmzt.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gvinvhbon.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gwesmcelm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gdkarvlkl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghylcxlzz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gewjczqfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gtbkxolth.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/geodnbsxp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfrwtahek.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gkizyzpbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbimsabuf.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gtotmxztv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gblexysjw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gsmdgfdsr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/glyzxblbc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghnkiquui.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/ghjfljogw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggicvzyxs.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gyrrmqhpd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gynvsimqt.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gcnajdznc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gqcuzlxhx.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gmgoinkib.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/grfzbgted.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gduwuoxzi.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/guezmivru.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gfwbkiqdy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gixzpoxhx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gezixktms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gjjrtsytk.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gxhektdsc.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/ghgwwsxyk.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gksrdgxue.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/girnqpyyg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gzbfybrcz.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gfwptntpp.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gdxfqjqua.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gedlbvjxo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gtewmbpyd.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gguyjqbbl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqtpetzff.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gtlxzwepj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gtwimgujw.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gehvtjudk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gwdtvntsu.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsenoyxzx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gglrwfmlz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gkzppchsq.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gzxdgmdwd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gioavdkgr.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/guprhmlgq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gnoezvpwb.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gfdrkkmeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gmagsuzrk.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gdedcxqhx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gdlaqyhrw.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gjvgylepv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghtfdkmqv.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glpbyhnpl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gxberivwa.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gomwlqpvo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grgqlzvhg.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gxvnuaeez.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvddjhmeh.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/ggueebqqf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzfttvvwo.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gywnrytqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gvjwvagzf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gbqwixjla.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gervewyks.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gfqdsjdob.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gojdpxwle.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gisvgoshp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gmdruqpxs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gyrcjhyoi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/ghcdeytvd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gbdkkpoke.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gfviuwjav.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gwpqxwfgp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gseehvikw.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gerjlcttp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gueakenns.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gedbgkxpf.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gubkxnlua.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gzfprynis.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gpqcytbwc.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gzjztloyu.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gaxfsgnsy.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gwczmxxmz.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gbrjsrsdw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gebajfjjp.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gjchcknpr.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gzvstglug.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gabvbhcpi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gybgofosq.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gahazhxce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gyovdbrms.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/glkfsqmuh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gswwkojrj.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ghhwjsexm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/goxizgkhc.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwtdrudnw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gvoskccol.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gobjsnzrf.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gcmujqije.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gnzhskyhi.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gjfgushba.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gcbpqnphp.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gdsuzbcpz.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gmeftrguu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gfgddvrcw.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gxtjpuavt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gtwdbyagu.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/goadgloig.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtskjsokp.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdveztdyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggfucijwu.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gsoyxiflt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gjcffdhtg.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gmvuyqiey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gqtkjxaro.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gayvqbizi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnqsxisgi.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gtxhsmhpl.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gkqdltqie.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gjlehwyaf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gmlndzvhe.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gfrgyrxoy.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gifzmbnkl.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gswkztskv.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gryuzyush.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gmisgpqck.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/ghmiwuuka.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gpxwjprix.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gozlrdmcb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gwiucvtkc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gfxrkisix.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkudwnbnj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gsmjodkek.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gmobfyrpt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/ggmnjjcxa.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gfnqwdxrw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gqsjooprp.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/glnfbfnwl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/ghjnvfkwa.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gvzjvpgjh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gtbijgaml.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gdufdaful.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gsoptlexo.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gxaywfzgn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gzmnvjktd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gyrwyxmsi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gidimedjo.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gxlamtquy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ghmqsfrpi.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gaxavuyhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/ggolchmbd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gaxadrebj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gjsgtfnmw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/ggfualfck.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/ggqwlvtec.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/grgcjaepy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/glflvrpev.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gwhtqtysi.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gbqvnfazx.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/glwcfdxwz.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gwygvnmig.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gvfixrbis.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gehwuvdgg.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/ghakfdmzx.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gatyankhp.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gisvvfmkz.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/ghkwspdna.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/ghdosyczk.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gkwghrpsr.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gkevultfs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gfjuthjgw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gfpevllrt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gyeodvinl.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gzzxctemo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjsuzztpf.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/grchdysfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxymswnam.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gdondlemj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gxqfncyka.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gocgebznj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gdbbnqsda.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gmnkkomkj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gezlkqoyy.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gpomokifs.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/glmcojneb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gfazhulhy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/grpwblbzx.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gefhuyehj.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gbptowsnt.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gbcnwevyc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gyurivxct.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gffhftalm.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gphekwnlr.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gpivtsovu.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gosbztlzg.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gdykqxmyb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gbuetxays.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtplkjnhl.sHtML


<!-- 参考信息 -->