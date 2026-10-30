代发 wailian999

);
来源：http://wap.fanxiaobao.xyz/Article/details/gbnuamoim.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gjcomihxs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkprypqsb.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwipwrjqm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjncbuztk.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gggnlcuvd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/grjbgkmbb.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gmwomgpku.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiymbbxu.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gnrfuacop.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvznzjirz.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gpikbogjl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gpglrmver.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrhsnsra.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiqdavmf.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqnvcwmx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbwreqgp.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gyljdleoa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltrdwnbq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gepswkchd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyawyliv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdvsxrdh.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gvwdgivct.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gubjfaviq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gfbhnaxaw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfpvapy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkykafske.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmcvaip.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfahbnekd.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbxwakhed.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/guyvewdpo.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gaitnhjss.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grgoqmshd.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrampakp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gfdmfsfbf.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gplotoreu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/godrybvkr.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gctdecvmp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbhihonq.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/giqjegbza.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaaxyodf.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyafoeff.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gbiwijrgb.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gdnybuntw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gieqsyyjs.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gqerrosmh.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guzedjytn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gydyevwde.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gbprdtjoj.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gionvvtmr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtitazjar.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gvgrxwcub.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gesgmzbxv.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gcvqoovam.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwktasuk.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gvsimjkzf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gruxrtngg.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuvtjwos.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybkkutnf.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gpazvzdpv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gixovrmyx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrqwmwdt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtizpejrm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gjklezfzj.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gqmhfdjuc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpsbktzh.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gzdvsztvf.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gsdibvanj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gjywusnbu.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvhgmhuo.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gddzlezok.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxtdmycw.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdfazrqen.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gerngutgl.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gatseigpk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnvdzfio.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gugujvyjx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gnbglobbq.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gjsymagge.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gorjncntq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/grcnxwlxa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gsyizeenb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/grrspzukb.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzbgisin.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gigdvrckt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhsshon.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/geebomoig.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmukiyxdw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkgdkmwt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtzdvnyy.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaekzqod.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gdktnvlds.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjaimwge.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpazmxein.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxdesgdhw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggnoywiu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkwppngbw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gjlchogkc.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwoegvlfr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gaggnnjnh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgqzftfh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/ggouwuuuc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghperoiya.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/glnyeyzyh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/glcvbjbgm.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfrncmpz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gutttlxvs.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gjalcgbzu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gceyfrgzf.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhntnawe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grwcrhnxg.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gkarhvysr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqegvojp.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfbhlen.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsyfwvki.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gufzvwwps.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gpehqgljh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrfnsoab.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvgptzfh.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gtuwxbwcr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilexmgsy.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaqyqkas.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfmxudqt.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/ghhswqnbu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilwbuvau.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyojxnas.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvixqwso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzojnljck.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gwqapkxrb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwulgklh.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gefdeyavc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfnfonqos.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjpggffx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/grkdwenso.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gurngyrka.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gubdexktx.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/glganlsxp.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhbsrdks.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrfgresj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsszqdnvn.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/geaefnhxb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gzstbrtxt.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxtjzwal.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gttnsufcz.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjdcrnse.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gyxrdrbwc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqoguawi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwiuqeu.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbcbphn.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdpbviyc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gjlxwnzjk.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/guglvhzzq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwharnscc.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gexjsecsc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gqizoqmho.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gvdvrtubr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gskowsibc.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gekynkfed.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gogvpytjw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/guumydtrl.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gtxjxhcll.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gheayfihf.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gisglatmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gcybbdjhy.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gucwqgmdy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpexqosts.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggflhmekl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvfaervr.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgqndxdb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxfsltp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwnvjvmj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkhnoazi.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpycmpqpu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gohuihact.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclzallwi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzoveduj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyljxcgiv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmaryatx.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/grqpfxznp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacuncswi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gmtxrtcla.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gindxugwz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtggjfoyi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrabuvtj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gvqvdjubv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gflsvnoex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glunxmnsy.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrqqitwo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gzplufkap.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/ghoznagmd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gjzzeovve.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkludhok.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gjtjcxhpm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitnhbapg.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gespojmod.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gpgujmxoy.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxfghzsu.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gkcosvksr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/grzvexfko.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxxrnnav.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkndtltn.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glfgobjlp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgwhgzlz.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gklbaqhwk.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaoqrxsk.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gvbzppxry.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfuxfxix.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guurlktvi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqagctnj.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gviihxrkb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiycifki.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwdvfmrw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdglpwdqf.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gczxtowwd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvpulrns.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdqcklry.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gsttsjqhs.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxooopwqy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwojmwob.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjfhivse.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdfhuyn.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmbpwjvo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnszbrubg.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcshpibv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsrhgeptg.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gclxhxyjp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmavpdqsm.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gldqovaqn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabearpvj.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnznxyud.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goteitwbh.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/geewicbzj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbmgjqvp.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gokvybsla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfeflqvhy.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/golwdyqls.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsbkhxdxt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkvjqzyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnbvhnyc.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglmtvkzc.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxsbienh.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gqjofleay.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkhqetjv.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmiinvul.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gykcgyxmg.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdiyeiok.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvmkuognq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gpajhftkj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/glejgxspk.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxvndtec.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gtgdfkpsc.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gojdcopon.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grcwolkka.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/ggewccaml.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gctbhexts.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfindtucb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gldttbiya.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzpqfrwzf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiqwyseq.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaamlivfv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghogfkuvh.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gfhjteywi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxowoiiog.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gyftrvpgq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gixroouwa.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwogkvydh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/giigzesyd.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvukdpab.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gziyrsvek.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjugbvysm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gmdluhtpt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwwsfkxz.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyelwyokn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gnypgqxlv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geurhoyjc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gotjtrtpt.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhoxkvme.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/giltkrmqs.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbqhbjrf.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/golvuwmet.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjaexxaux.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyfvsqvx.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgukcilg.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjnjanqo.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaexpsbv.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grjaiuymv.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfcnqwdfz.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/ghtnojgvq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/grutcdjbm.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gxmmfwmow.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gvcatwhzq.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gewdkoohj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakyqkhwk.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gjgaczgui.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gckoihcst.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsrjnduwt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gpykkmeoh.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpwxdiaeq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtdffvcvn.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsaqfgiw.sHtML


<!-- 参考信息 -->