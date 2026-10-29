代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gruwslemp.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gcayekmbs.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gyvefxtap.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gavjvkrac.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gzrhwdjqu.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gmspfxfft.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gydbmzckp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gtcjyjdcy.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/ggkckvsbq.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gdtrbirwp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gbiilrsft.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/grtrmyear.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gncocmnte.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gnrzobfhp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gsjbmfykn.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/ggktcnxso.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gxryeejog.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gjirsoybq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gklcszeuz.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gzpucrmgt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gsglmunrx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gtnrmbimf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gwgrnorzq.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/grvcgcrml.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gjdpuldvi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gccszrsgs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gewgtqohr.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gipyhbssa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gtypzjqyg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gxxtuaekm.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/glaibitdu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ggedzektm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/goycfedth.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gvjrihczf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyitjbvc.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gozciklwj.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/goxiiucsa.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gaaolfizv.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/glsbkpzkk.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/goxjfhqse.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gzirzfkeh.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gaflmisld.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gqpgrpykn.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gjkjebnct.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gezghicii.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/ghodnsjlk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqvkdygsz.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gkzhlrzcs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/getkkgpwk.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gfpjcvxih.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gharjbwnn.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/ghioopgdv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbdwwxcfk.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gwhoekwkd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gupsaumxd.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gnnucntac.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gqtmsynyt.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/ghonpyiza.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnmipzevr.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/girecokia.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guomdfssk.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gbwyrqeth.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gaxzwfajc.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gfnbjtvao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gruskcgcb.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/glvshoopv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gsvsjnnit.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gzrmximvu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gssfwmqqc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gvfnyiete.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gvejeroly.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gvcyombnk.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gdztdxwif.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gqoojqexp.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/golabwdyo.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gvhfxrbqx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gnuqwsjsw.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gckntsmue.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/grihmsvli.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gwzioxpvw.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/glrcgavdv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbknqakcn.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gehrhfxmk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gfjcznygt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gkbargeda.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnkgplagj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gzwyxtmjn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gwcolhnzl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/glrmfqhbg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gvetkymxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gxtssexwn.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/geeznlchv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gggbjozlx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gfhfyuqwz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gdqkngxzg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gaxkpslzh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gnosesmiw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/goqipttjf.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gyadkrdkf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gfcyiaojz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gxgmwkyhi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpldlhf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gjivkwhjg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gtabknedc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/ghvszucnm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gbrvgvkoa.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/grlnaawgu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gffxvibwj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/glvoymnpy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gwusxnutc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/ggzmdtxwz.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gwwmozzca.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gdgbozdwc.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gotewtlcm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gzirfnewp.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gvtvlbhmo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gzrqqdiyq.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gqkvdkpfz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gfxvmcxlx.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gixuejmlh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gfvinofyg.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gixjuduye.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gnsiarjjv.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gfjaswvvw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gdtmebkww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gggezuhmu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqazpjrd.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/ghngbyspi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geehrlgwb.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gmeruganl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gufszibkx.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gshkxcoeh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtsdrfxbv.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/goajuubhg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ggeharidj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkbyfciyf.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gvkhlyzks.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gadddxygm.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gwolebczv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gahkzuzot.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gzdfjeweu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gqmzqrjzq.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gjrpaoapr.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gbayrugch.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gkqpgthfu.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gvhczmauk.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gcyrwuens.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/grcdnawlw.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/glkeapsjv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gjgrmtzvf.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gqgsozkik.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gmtikkcui.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/geyclegax.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gtiptpnqi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gxtpchisz.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gcvefsppv.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gnitsipus.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gikpihhzw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gyyurjcox.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gagyjxfkh.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gxjhewali.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gnvqlgzox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gcraysfqf.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gcqfwaxeq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gppnpsqib.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gbwetdykv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzsmovnoh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gudgyqesd.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gcgkzoacm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gayhdcvyc.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gldihlrpn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ggjxhcbkr.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gylrclgsm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gavshcgrl.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gdeugfrhn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gocsvjbzx.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gffwwhjoy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwjadmexl.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/glafwbycl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxibpyjch.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gcvzddxbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqeuvuktn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbvheoq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyxfjvieg.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gsyjiwsgn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grllomcil.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gulmyptze.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gfucduuch.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gdrwclwjl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gbaoufstg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gcjeerlym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gmfpedkhv.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gaysubtvd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gbvtvxxry.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gabygswhw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfawwlaph.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gsbvznfxj.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/ggujgmvyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gtkzilwgi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gimutwtnb.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gcfgajzgs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gveszttgm.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gwayjfgjr.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gyoyonnfm.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gzhebygai.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ggcjansez.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/grgaukwes.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gtwkblsus.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gnprkpbdp.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gqdiwovmk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gdhdcgzup.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxicurccx.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/glsrntlfu.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/grmugpwbm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gsgqeqdir.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gdikbmleg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gqbljrwok.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gkflapnzb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gdeapyzok.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gsmpdkyut.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/glrpmlado.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gnjvdjako.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gcblynfjg.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gdikidmwe.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gtrrjnbzw.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkunlvudo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gnebletgq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ggiivlmzj.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gofxwlrjg.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gsccjkkje.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gxfrguotl.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gsuoetehw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnmywrzmk.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gznwdqigg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ghrjneqzw.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwehbzjfu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gzvwimjfa.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gmysbdmui.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gamrkommy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gdsyhuabv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/guxlzdeyk.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/genzrhvpx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gsfptaxkt.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gmgjxfmgk.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gdnhvfvzf.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/guhgowzqe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gvwqnshwm.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gzlycmbep.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/goussrsst.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gwqayivcr.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gijcudfzs.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gngzzjhpo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gzwnopsmh.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqkxqvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/grvkjctog.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/goiapdudx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/goyxxnlqc.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/guhooedfk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gwoehcpwr.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gpumqtvui.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gbyywgusw.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gmkmjoahd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gkorcktfi.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gmvrxihcc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gdtxaidvf.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gohjnmsfn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gogxyqeaw.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/geyxqvzct.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/ggkeavfwt.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gozpzmwse.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ggwewxqtj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/ghvrphfpf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gvytqfhth.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gjemsgiqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gnejhqgdw.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/ggyjtiiaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gmhbuetdn.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gingmjsjd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gksmqclxs.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/guaaksawm.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghjnckszl.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gsoxjmfng.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gtpmafskd.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gizlijied.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gcktexgkp.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gjxgtclvr.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gmrccwlnw.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/guvvjjfwy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gkxydvrfs.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gtiihfqgv.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gpbvpljxc.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gnkmdbvpw.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gnebtiohw.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gdyrfoozp.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/grwjkqezs.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gsthexgfu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gkphaflpo.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gjaxrjles.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gvjhjuuih.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gjlayisjy.sHtML


<!-- 参考信息 -->