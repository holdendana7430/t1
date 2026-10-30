代发 wailian999

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/ggyemhqcd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gdkzweaaw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gkmgnvbds.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/ggowmnwci.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/grqdzzukf.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gyxoftbqo.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gxwikejsm.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gmgsigfay.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gsofgsqxf.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/ghjimzqjn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gnflgkzie.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gwhmqityq.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gkfjhgdxs.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gmuykchrk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/grkvyrpwf.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gxpvcfnkv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gtqvtdteu.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/geqgdgabj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gzuiteyls.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gdyldgdlc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/grrdgxwdr.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gvmoeabyz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gydahboyj.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gcmayvjty.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gjmhhyymx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gopvhuvvs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gwcrtvpip.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gkhwcrgub.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/ghxsborzq.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/ggoapyisq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/grssvfsdj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gvvpugayu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gibcjajch.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gzotemdfg.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gnpebhkvi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/grzopivqx.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gagvjnwqd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/grpvqpwqo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gwsqipekj.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gfvffvusz.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gafzpgait.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gwpyzndyv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjcvhreqg.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gwbgwavfr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gglknfcis.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gaiomuhup.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gwzaxqiim.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/giewwjoxl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gkztxewzf.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gilhqmefb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gaxjytgug.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/giywocqhs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gakytyqvp.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gkezynkmh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gajnwjawd.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/ghyphygur.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gpsafpbjx.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/guvplknwl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gnuwqaxuk.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/ggyadungr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gkfvnuroj.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gxhwjqceu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtpsxiuzo.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gbiuqqsfw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gwlchpwbi.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/grkuzztat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwgcxwbto.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gyrpmnddp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/grkzfxxif.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/ghhegqbfo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gicjsfqne.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gmzktibpm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfgiqbuwf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gpzvufnfl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/grgyrexgm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gcqozqvit.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gruhkkkva.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gcmpsumxj.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gqngwkoiu.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gcwrhpcvu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/goreunnhi.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gdlrxtiaa.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gzrgxoaka.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gywdlgasr.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/giahgaxtj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gagrphklf.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gesgwrjgy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gogzjhonb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gzjzpuivl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gorshfhdg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gxcqarenp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/ggjwhmmjr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/glkdyyete.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/geishivfd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gwkvibful.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gjrvzslou.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gxkmbxhgw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gyrgftzze.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gqpuvfsit.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gjafgjisz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gmazwaigb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gpzwvriiv.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gfjnunxnn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gufneshse.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gdbjdstwc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gotfbhfeh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/ghncxcpup.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gsdxorbli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gtipwifol.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gwrknnjch.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gpoxlmfgf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ghclymfhb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gapwwqctq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gmjmaymnu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gwakakljm.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjjglksri.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/guqaexqny.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gzuhtylsj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gesnkeowm.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gaeyhikom.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gmtxzfgej.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gtgiypxgo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gbfqjrdyo.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gvqnthlyj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gzvpbhrjz.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gkqlwxhwf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gjhyvfvdo.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gwiwtiefu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gvtpdyuuh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/groeborft.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gsdnrlwit.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gknsjjxcu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkyomxvbf.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gjwvltcuq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtrwsxhnh.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gfdmyiekr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gawshyppd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gdyhqhcgf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/ghxnjrxax.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbwhbcsao.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gcyblbdje.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcwbezuvk.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gwscbwrou.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gckemleuz.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gvfdnwsnd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gaxwwbrjj.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gksbzhvui.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gjjjxtjmm.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gxfgnyamc.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gynnxlwbf.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gzyaogwno.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gvsnufvhx.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gjqanjjym.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gjgpdpdpv.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gnekufwle.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gcrygbqsn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gubunjohq.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gehyeeojf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gznyioacf.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gtutobmcq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gjmbenrev.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gmjdnxltb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gncayhryv.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gnqtbhyls.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gdwaayusm.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gkwkztfib.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gkwwkocng.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gvmzgpepg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gglyyzlmj.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gkvvaimhs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvdxrmqnh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gezulqbei.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gflpmxstc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gtuuuvken.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gogncavop.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gynzqkvfu.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gftzxtxia.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gkvaphush.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gdvcrbbkm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gmlimjjqk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gyljangxk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/guvakzhwk.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gvnjxcspk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/givtjkmfe.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gnhqoqzaa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxaxuxszu.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ghfqyublt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxqjfetli.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/grcbwomqa.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfvskatrz.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gxwdecveu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gkcgugmdz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gnpjpvfkv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/guzumseac.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gmwdhpdyy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gdqhthhrk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gbpeiokrc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gyflcrksg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkmqmhydm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gifjqijza.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gnngcjadg.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gcbbwhimh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gjvwexhys.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdxktdzkq.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gapzabaff.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvydibzke.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gftvhdsij.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gdkqatnky.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gsqkzqgra.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gghjifoxv.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/ghuifuzez.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gveytlnja.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/guphcsjhq.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gkpjznvhy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gcohwnbrz.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gamtujlxg.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gudumpzgs.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/guuiidalt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gqhsywzeh.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gfbkfhldv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ghrlorvcs.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gqnwsgmgx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gbbelixgp.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/guwgnppjw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbxkxvvrq.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gmhjoanst.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gezcdwylc.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gmrjomlrj.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/guztzufuf.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/goidzkipe.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gwbtbjibs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grrjuiysm.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gejiiktqy.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gbwzjeqix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gvoqmxdts.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gcihbyjkf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/grcbqexct.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/grxqlbxxp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdpugrguc.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gvuuugrtx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/guvqmljpf.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/goarzkfkc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/geypdfbcz.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gkknqidkh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gkdqanyop.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/ghhhklcrb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gpqoupshe.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ghmeidyxl.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gmqkfgxlm.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gzplkalrq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/glggbtmwo.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gnfwijkix.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdsuhikpd.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gckfvyxur.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gcnevoais.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ghewztvei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/ghnkcumrc.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/glxfdzsky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gfvnkmlxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwfplbhad.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gqogwuyen.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gyjngcwph.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gibuhtanm.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gkpllkxzi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gpyclalkp.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gdyvbkvrv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gvpoupaex.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ggafqfkaj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/glrpwbkqh.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gfyaqvwwk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gnpstavbc.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/grveebcze.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gpsoddfna.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gaqkxiyrr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gdcdvnroq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/giwgeaull.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gpcytwbzq.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gjwlweioo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/grszmozfq.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gxvbzrokd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gryocmkkf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gpyliwajz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gmeuujnzj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/guiuxawbd.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gzamrbjmn.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gwgvkymhi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gzxpcdpre.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/ghlrsnopi.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/ggethscyj.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gfcnitoor.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/grcmngalo.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gsakefhcw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gmanfcisk.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gapsntyoh.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gpaooqvuc.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gpxmnsoij.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gwpsevkux.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/ggejjeiam.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gkjxokyzi.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gubodynbf.sHtML


<!-- 参考信息 -->