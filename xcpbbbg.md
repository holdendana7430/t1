代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gwnccvuqm.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gpxfyiqdq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gcorxstxc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gktlyzyxp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gbujdcift.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/glcwtsors.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/guyfnoqsp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gtwcpfald.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gevozpizv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gkchsopys.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gmujbbxbf.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gxtkaziqu.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gggpgqfkn.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gtwkvslae.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpgrdevug.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gcjiqrebq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gixgbgrts.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/ggxtzomct.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gizyupunc.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvjshmwxw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gghrmnaml.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gkljxywdc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdajjbjik.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gybhsrndb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gsfgvuejq.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gutpktzks.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gusteyzuk.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gjkiycirc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gytymnpox.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ggmwslaze.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvyojqvjd.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gxeclmcdc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gimmfdqac.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gtxizkeep.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzlbxbttj.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gyoglrias.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjnxetupz.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gdcjwgspj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpmqowhog.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/grbxdlrco.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gywxcdozs.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gpsnsppis.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gqqczfcoq.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gxynjkfey.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjzsxkoje.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gqrsonwwl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gczejzciy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gzslwrukr.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gcdcqlzal.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gbxkekbgr.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gauytolgv.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/glvsrqrnn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/grmpxhesb.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/glvcjakve.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gbppcxlvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gdocnwnfb.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/geupcgpjc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gxywcalai.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gnqiwbnag.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjcices.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gxqvnsxlw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gejngnetp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gxqmjguno.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gjthrlyps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/geuqurbjs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gfngkwxsx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/grikehwlh.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gjkjhuibw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gailiswbw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gnusioagh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/ggyitftpp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/griadwhdf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gondlnhec.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gsjevqgos.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gcvrhswzk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gxbfppyar.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gkxeczrqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gvpvoxrdy.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gggunzlfz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/galtysywm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/grtzzdbyl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gsexszbhs.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gurxnvmzp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gvpavatgg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjeogrlgc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gtpichjwp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/grqlkvnim.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gxdglepje.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbjccwsit.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gtnwckcaq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gccjmisjv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/giiuhuaec.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gyyphrgzi.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gmnrshhgf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gznjcojtq.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gwoxwnmsn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gcjjpnhcu.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gxwtggcww.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gymgdbwbv.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gkyitybrx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/ggmgflsmq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ghitaqahg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gohlwsxbl.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/grfbyotfk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/glcvmkqta.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gcohxxzmj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmzyznp.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/ggxwtilyz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzxskzbqs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gwyuvqctn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/glijbrmaw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gggfnkbfo.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gsobmlbvk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtywtvsrg.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gbrlhnpys.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gopxwlfdf.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gtzkgvscq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gmpemnqoo.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gbyljibrb.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gecrikjjf.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/guurfvbab.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gbckvqfck.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gyfwutbeb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gzaqmqqmj.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gkmsgsvid.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gipqiijvt.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gswvdgxag.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gngvxvuqp.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gikmcbguu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gxkomtvyt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gvqelpisk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/golxntcqp.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gwsvdcfng.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gdotsaifo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ghquehmgi.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gzomlnimc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gszeppzww.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gmwlxylea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gcxtuzvyb.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gddmcnrsj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gqufuzwkz.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gprgjwvwx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfskyrlrr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/ggwbaxrun.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gmhnkcsru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gfyvvgfje.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gbqtkrusy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gnerydnnp.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gjogeunia.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/ghtnifxin.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/ghnettyfe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gyiczqrrz.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/ggdneidxu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giueomtqs.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gakqxryio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gxhsushht.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ginpxuplt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyahdytcy.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gxwogcmjj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtvgnwawu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gfrhiqmfv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaxntlcsv.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gpuejdikf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gpjppqthq.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gmcxnpafe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/goqyfyltj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/ggaqzfuzg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/guajyzeyo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gjbgspvop.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gaihhlvyl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geroegfvz.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gogiwvnxu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gqhjhjqsz.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gslpbdshc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/goaijukkf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gffwnqpqr.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gfrdvrqjm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxhsdcwxj.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gbqwcnuci.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gvunnpghp.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gpnddlkhf.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gshuemztl.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gqkiwmoif.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gkqjdvrqn.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gmqmpuabg.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gzjqzcilk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gkggtahfm.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gotmudcpv.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gbcypddti.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/ghmlsihtu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gpeteujgg.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gusgnvjik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gzzowhdea.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gdkthpvxg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gtxhxjlyd.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gkyhtbtng.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqwzszpwh.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gmdwsvdac.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdyfyworn.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gfpgjisoi.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/glrdidbpu.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/grwtaqtde.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxapttvzb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gphbberkq.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gznxdntkx.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gnhudflzc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gavimdmsy.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsrshbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gctjsqbsk.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gnoudgkja.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gjqmdoznu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfdvzkifa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvmtwfnfl.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gpwjkcznc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/grgzwqiha.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gckpaacqx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/grjjukrsz.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/ghcwylypd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gcsgsqaak.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gxmamaiyx.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/ginypvwuh.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gfzidwghv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gmkkgzhge.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gdxtcjpyo.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/ghnnfwtna.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/guyrfeump.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/glqjtgnrk.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gohwheyho.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gdimizfmm.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ghthvypim.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/graonpqmr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gsxwfowlb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gohqxtszd.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/graxlwyjp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gpvpvwkiy.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/ghfexpjrt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gpdnvnyje.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gcdriivmm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gegrxrlkq.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gzzqbzmwl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gptwlxekq.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/genfidbpj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gtcbizoeo.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/ghfpflozj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gxtvmtzno.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/geimpqhqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ganznxowf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyuasmk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gdqwhehzc.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gcigmmvvi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ggirmfltd.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gaesdflhx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gelpmeizk.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gsgtvkgfl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gnjcstebs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/ggikefqoh.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghvkrzdfl.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gbldjftwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gronsatjb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gvflljadw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqgyipquc.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gjgfmltcc.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gquvyqpgq.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gmdkjuzzu.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnmroayfu.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhpjerl.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnywrwr.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gexajmrzr.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gujhlpvwf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gqamdpsbs.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gfeojcbet.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gaqteemgq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gllycapow.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/ginxshpgy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gcqbkfwux.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/goekzdaaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/grzelazfi.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gnkbhqpnb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gwgyirqag.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gcdrllvdb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gvvzfwomc.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gbpykktgs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtvxetzlh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gsrqtytbo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gdbymydui.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxmlvizhv.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guqdieclf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gvxhwzkkr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gkouokqan.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/glooqymdz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gwgnzooqh.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gblqqbdfu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gjssiazbp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/geszbytdm.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/ghirkvrqw.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gjahutged.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gwgchuzoi.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gszxgyvwc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gevaqvxrl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gewyobyhu.sHtML


<!-- 参考信息 -->