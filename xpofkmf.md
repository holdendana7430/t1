代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gkrrtivwd.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gfsufvzfz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxzcxqhj.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjpdoip.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gjjetxnzb.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gacavkzbw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gsqpeqnoz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gmvnklmdb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyoxcqcn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmgljlr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpzxrdsu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrblftgy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjryklljs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gybcpfqqx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/ggiiaetmw.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gixtswkgp.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcmpbazg.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogutbdxc.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpedclal.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gjnnldgzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gnwsmkryd.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/girnmhmnp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxqxcazp.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqrvqwrb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxvjpodc.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govnxvrcm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grdyhcicg.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdvfmege.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guphjahca.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gglrhvlso.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggirynsnr.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gklxwxyns.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaqhhvru.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhaqupi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvuvzjkr.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvriyisnk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gfxzyejyq.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gluhowknm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupfkqfe.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtofmpyy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glygdxedg.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gzkwuijqp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqikwbxd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmqdpkd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqcxmnbu.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwgpbctg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyxeyuth.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gtvmyrjpt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokjhfzqe.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlpjobbs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwqwjkkg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gaadazjnl.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gjfoertim.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmvznthi.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gcowdpumd.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcfygfzj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gdqiygisr.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbskpouv.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgjsuaga.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwjzindn.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gyfsyzljz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsvcbhro.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/ggestvhsc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkvxrziqy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhblkouw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gqoqfuihs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvxywpnw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/guimsbeqs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gmpfbykyc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunrulayn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjewbbvjk.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqidwtenq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gojkmsmwp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geypwpbuc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gcsjqfyao.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxxgxrz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqwaumye.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gypbybavi.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqcetmep.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpccmwuf.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmtuopiu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggutkxxtq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/glzpykldk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gifrpmvhy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwfvxfjd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtssiobgr.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghesrnznd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gungerqtg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzbdgbxo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmtqmfc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnyihjhy.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gooxucqgc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqzklbijf.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gevdlwtjd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gopitadxd.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/giensfktf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhqtgbav.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gksnkczdy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gtdbehqga.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrxneakn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gttujzycg.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfxyhqqv.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gibalpsum.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjadjtsa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkkyrcoo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gcoqdprji.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisdpcnwu.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gaxqtfrqw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkowmjuld.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdlnerhwr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gytxonzwt.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gfbiyjofl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gootetrxq.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gubcbaeiu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gqztjjoww.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gakassmwk.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/ggjnrfznu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjpalhfk.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gcpsjbpxf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcvnmhva.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuxvrxxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gpusyqlnm.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gyxgkomck.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/goukezmnp.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsebcppq.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguyhqjbc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giimhebdj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gymaomswt.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gklitoahq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmztmuegx.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvidvtxe.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncjzvwcx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxuclbes.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoazpuop.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gryewbkny.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezlerrpp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjlofdue.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/glsbypuds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gygxyvmmr.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryotkgbf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmkwavcj.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gofwyoeef.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjuncjg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeodmnwm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfoavzpe.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gokdaxdib.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfjxkedo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gnqwzwxhf.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gouyyzubd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgrjsoqt.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghwvshhi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxbaaoql.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gfapbvptl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsziqhzmi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzpwagli.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gbewpxlyy.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtragsxv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrmjvdtl.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjssyfpdg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzgouegw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gasuwlzaj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzijwyzjg.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfiqbtd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpxazebze.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gklnpjnwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzswkdvhf.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/guxtgmkhi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzifdstmg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprohyjdj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/glggjhdqo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwzfsfwsi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxcbpbjl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gifuawgde.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpwpulcn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfbvjmlcy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctjqrrq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guluyyodf.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gzmczttcx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezdffnok.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbpixgnm.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbqprauz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcznfitto.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/grxfrmkab.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltxnmwxn.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/giyhkrmli.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/guhzqmxqd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gemknqxlr.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpkqewojp.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gwojdbhjz.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsrefutmq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gqucizbvt.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gmsiwqbio.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/grropcftg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzoefvvk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjtnraqcq.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geaqxdjel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzdwwmd.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grgrewxna.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/govkdrdqb.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhorufpn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdecrvqqu.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmcnxlcf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdsksnma.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gzronbslg.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzijeoton.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuwguztt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpguyqbpj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfmovfzf.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvplgrmqx.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsivbzxsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxlpmtkdn.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glxzrsglb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/govlutyof.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzrilvd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvonhwcoe.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvegvxyta.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsuxwtkot.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtcknfawt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbaftgyds.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gphaslwan.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grukpyuah.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/guftiaevd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoyeuuld.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjieivigr.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcfkdtops.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctajhdjx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpmlvgnpp.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/grreakwiw.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gboixvddb.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxxwoxfi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnijvmigx.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glvxretmz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gccaqvjgw.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghyoblbvp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghigtfaey.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjfjioyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtlbdtfuo.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gehkuleff.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddhsndqq.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/guqldcnrb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gadqzskgf.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gfppvnqqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gbghymidj.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyuiwcqjw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gaflcfift.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhtrwjoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmpqlpur.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmfkxiek.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsbzrakdb.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwhssnua.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsqwdujvi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqscutif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkwyewms.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesyenkte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gxmpmqlpu.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqkbksvd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpszeiutf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gktppdbuj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvpobntbq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/guxoqhojt.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gummngcok.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gylwkiekn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfwjldll.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gfykdftbm.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwutoytj.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gunvuszjc.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/grmvlsqeh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnucsemqc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwymmcav.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbkdbqag.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greolruss.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfroqyglf.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/grozwqran.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gigbesmhm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczspvppc.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzfactcc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/giciwzdui.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gvesllleu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gwfmeinqz.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokohryl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbtbpric.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdwaekdv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggskmyjhm.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtppwusml.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gokzukohg.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqksrzkcw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzgleskv.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrbdqhgg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiqsilkr.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzwppgo.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjbpfsmka.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzulkxsi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnvpsylh.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/goicifaoz.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gljodyxme.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmkkwgkz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gxycnbifi.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdsnsnqra.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwufpimas.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/grcoevvxz.sHtML


<!-- 参考信息 -->