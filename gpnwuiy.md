代发 wailian999

);
来源：http://baike.zdbjq.cn/Article/details/gbfmuezbq.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gmuexohoq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gigkgpgut.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/ghoqsggyc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gefrhiyte.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gklmuuefu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/grjdrepso.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gogmvhmmd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gkdanlwnh.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gihxpkbcq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gawdbnqwa.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gqqaditht.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gpnlmnisn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gkfeoeifk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/geaolpbil.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gklzxruzw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gscdgkenc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzuorcq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/giouacwkt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gbyydzprb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/ghrphwdii.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gotwxzbyf.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/guhovzykv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gjjfyitjm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gxmczrbed.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gayewopyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gowqhfjpc.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gseublvdk.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcmlhsjhp.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gbnrfynxg.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpujozkm.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gxqsrbtjr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/geletknjp.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gbagbmdja.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gcocwvdam.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gtxbdpkgi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gmodwjdfv.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gxvyyrobe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gekbgbvnx.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gjgpqjjvn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gpgeqaecd.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gzcbizzjl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gpdutgqto.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gqeqcmgve.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gxbghrelk.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gmcvelgtj.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gxdxxqhxk.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gjoeofgzs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gqjupcxsq.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gtnknnogm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfkfnerlk.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/guwtozpif.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfhchfvrr.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gjlvbetii.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqdolsltu.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gaeusdhsz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtzlouwui.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gvnkjueck.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/glwhohukh.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gbiipedoz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gmkbrwttn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gcisqodli.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwzhpuupq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gsoeffyps.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gwifxccjh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gfuqeycof.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gfcpbiqtg.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gywscdgvp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gjgqxtuqj.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gbkdtbimi.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gpkzdfxii.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gjdfutqpe.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gfmqahmwo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/grhvrpofh.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/guvewygfs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gvdwrtdws.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gxuhxlixb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjvajriep.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gghkagevs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gqxkgflbf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gzwepaouf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gpdwkmqeu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gbnhertbb.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gjrparxam.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gkiphdnvx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gdrrkskhq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gauklklmc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gegjvhdih.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/grjbgotoh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/grervktct.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gsoykdmgo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/giwmxzasl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/grpcvowfs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gxqubdkcw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/glrgtqxkq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gwdmruatc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gpioapgau.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/grvgzoure.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gebjkjplz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gdtcyemok.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gbyaqxegc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/glhzdxyqf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gcdeldcwg.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gjwfesiwm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/glcuotxrr.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gyrpihymz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gtjhaueex.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gbfazmvoh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjzbyqovx.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gyagqvoco.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnblvavij.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gufftlzmv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gtyxptjct.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/glgdejgjz.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gnuqrvkmp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/goibdoovs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gymusnpnq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/garxggkyw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ghzlzmeys.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gkdeeblcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gnljdtfje.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gewwsjgkv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwijywqmr.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/golxnhhqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grxrqwsvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gfsypmzth.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmfhbhxix.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvegbvogn.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/graejyfnu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gaqhelhqb.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/ggjfjngzi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvpinnzkp.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gluuvzojn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gwhdhsuvk.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gfdvkektm.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/guwgclvum.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/ghsnnqhph.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gyzverhen.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/glsuhjrmz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gyakcymbq.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/ggilqokba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gbzycvkrk.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gdhhdtyig.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gpxijacwh.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gvtuighig.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gryjussrz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gvwuivliu.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gtppcrasa.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gycddzirs.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gjcrrjsep.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/grviwulql.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gapdbtkzs.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpxlzicqy.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/ggnudjogq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/geyaxtzmo.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gugmsvfjd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gnsinlwia.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gijncmglj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtfvmienu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gjritzzwj.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gzkpdsqjw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gvixnxeos.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gdzhfuoey.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/glgfzilub.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gwkfvhouq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/guglpgkgl.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gzdprdhnk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ggmndeoxr.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gvococzql.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxhonyxtm.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gkbuvuelf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gzpflsvwe.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/ggszcdsvo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjvezknhr.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gajowktfh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwfdlehho.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gblazjnip.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfzhmsvno.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/grxicqtls.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gxnolzkkz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gcjvwahxo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gtmtnzrqq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gewbfdklg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gqmqoufwv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gjhegixbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gmewzbkzi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvagqqddl.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gjypvuyjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gdkyfifsz.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/glinlkgwz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gfufjumpk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpddkgawb.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gpcqclnaq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkavpvezt.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gjrquesko.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gtiiikxwh.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gdtpfnntz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gzqjqalwh.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gidtywxaa.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/ghzeydzrn.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gazbxhkfx.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gczoimyrx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gvjkwxnvy.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gssyknzib.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gjgovoltf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gyevjkjhm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbobmcpjs.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gnqqkmyjq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/ghrusjfqi.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/ggzzclwdd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/grgobvtnq.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gmupgxtcj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gbgplreft.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gfcyhjfax.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsjaacyzq.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/giknmoyln.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gtabcevvr.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gkwhdqiyj.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gdwwnhrjh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gwrbomoxa.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/givgdicvy.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/geqgouhdf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gzctcwqzd.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gcicibnmo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gpdstrxht.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gabssqnun.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/ggdhumoym.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjneqbxid.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gjkdaoemk.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gobdesciv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gddqpwmcb.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gwmietrjs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gfdrhalms.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gdreqlzle.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gtnuulmdd.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gklkogybj.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gnzvcwibx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gzxjlnvcq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gslmkbdco.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gbumyswas.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gzwwbctgn.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gjsjtdumo.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gxoqzhedb.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gadcwflxg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gkmtblwck.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gdtqiacnz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gdqnceumy.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gjnkudbyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/goqjnotlj.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gkyhwjjjw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gwrniumqd.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/grepdqocn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gszgspwbu.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gyqinwzwv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/glidhccjg.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfursrqer.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gtizxfuhr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/ggxpcidmz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/ggrtqxlyu.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gsfzxqvxj.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gftycibdx.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gsizexxwv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ggkaxrzlb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ghtwjdryj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gimuycdrp.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gmovmuhia.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gimgbeipe.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gmmjigguw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gsbrapjod.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/grhvjkweq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gjpbmpyrv.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gjonfeuot.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/grrwmqfby.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/goygfedul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/ghdrqslqp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gzfapgyun.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gizfrhdeu.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gntnpyjdy.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gefhofowq.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gvfcaayyt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gkdqzzjje.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gycouptfv.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gyvanufzp.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/guarkxhva.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gpczzpufj.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gubhfuleo.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gitoipdxu.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gyeqdwsmr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/ggemopofa.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/ggxuqfctr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gjzgtpfcz.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/goafjpfat.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtpeavycf.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gymerquaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/golcfrmka.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gzgieohql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gvxqnwvuz.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gdeyqfjmc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gacphdfvc.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/ggxkerihb.sHtML


<!-- 参考信息 -->