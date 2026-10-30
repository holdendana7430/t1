代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gzcberlrp.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gzpxnyzjv.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gsegqhaye.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gfqfkqexg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gpahiwcxm.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gwdtxaqff.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gjhedawnn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/grpdnfujn.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/govehesck.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gdqbfamsr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gkzwkjzot.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gupaizdry.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gdrqcrqsr.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gkklzzdlt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/ghazorcub.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gxhclbtaw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gjlmpunjl.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/glnffhgbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/ghkoegzpo.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gtktnokmd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gltwsrtgi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gfdnobjhj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/grosytkoh.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gycmjpdhf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gxwzdlchk.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gywwfbqde.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gwmyclcud.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/ghqeuyknc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gkopogtqm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gogitztun.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gfisujnfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gnlqxzwdd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gftaadzzk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gjysxpqvk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gtegmpiay.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gjupqgvcr.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzsifggix.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gxtklrtvg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwojaznja.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/ghwxxdbaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gusnghfpu.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gygbzvyrd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gfjhbbeeb.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkvnhyp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ganetrigh.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/ghuxtedeb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gchttpqvn.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gepmnopnb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gpkmasfvq.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gxoyytvvw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gsoyamylx.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gvetxwzjs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/graqpqmim.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gysuwppxr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkhrgursu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gfrzyvauf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gblsxacfl.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gydaymdwj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxoemfccp.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gyhqglvhv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gfjrqrsjd.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gbwvhkoaq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfksfudvr.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gcplznkfo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gakdbgkcs.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gwzzizywk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gggjfpbvt.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gtdnfjepg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gedaxrnmn.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gpvbqfcde.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gihdpwvve.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/glasespaz.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gudygeurm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gxokphqby.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gvotfxqey.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/glnqhsnqp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gzwdnztzh.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gufgzkxoy.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gtjlbwnrx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gnryyazvm.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gjliurpst.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gvlspsqzd.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gdcwqurjt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnygpphgh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/glmbsnvwz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/groksqzzv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gzreptdbw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gwryohudt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gytnfpthj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gjmighodk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gmnrfdiep.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gzhxkwgpc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gpvkslaph.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gqulftwnt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gncxomddz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gltmbvqeu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gjkeymhjv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gpqkqixke.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gpzmhldjh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/guunugesi.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gxnybquth.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/glqeiohyy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gfdzowpfi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gnmqlvxnm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/glhotslbt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gpirhphvx.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gryhrbnuy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmodtzcn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/geccpuulx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gnrrcnjcv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gqjyfypgi.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gbeiyormz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkqhczbib.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gvmsuzyzu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gpwvracai.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gpmjpulyv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/ggyeroowy.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gtywlujyd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grqpuyqlk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gqwjwhxsx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gwbfzxpon.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gebmfdeus.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gxfjnmpvq.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gxbtnllsl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gfcjybzxt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/giuplhvzr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/ggfskftmr.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gxutnureh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gkhzlntep.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gkbfrvkiu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxkwyvwiv.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gxejervdc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxgybfgav.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gcnixakuz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gkgrqobhx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkqxqyitx.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gpkqiivlf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guackvubx.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gzzivsszc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gseaptvpu.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gfshhzdcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gxaqvnqee.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gvqfhilib.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gtlaluafc.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gybuauwnz.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/grgnumcwq.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gfdkwiqbs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gljlgfaxf.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/goooggphe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/giwlkrfkv.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gacldxwwy.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/ggcygwicm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gfxairbcs.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gdkawehnc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gufyjylci.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/glkkkmegw.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gzxvuzric.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gzzpgvwnj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gnrypdjxm.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gwyrwbcjs.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/galjwduwp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gapjtjchn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gojrfqdmj.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gvxqgeyfb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gjrzqqytk.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/goacttbqx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gounyljrv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gtqaaissc.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gncayupok.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gnpzvpxxv.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/ggdgrygre.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gktduzqvw.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gsqcvciks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/givwnyosl.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/grjcgnfyq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gowgdmvvf.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gkfkxaqwj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggswiyhts.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnyblbblk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gvxeqmzeg.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gzxztisve.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/grqegvsie.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gphuacnbl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gozbdkzwc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gwwuxixqn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzilzucbe.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gemlvpuxp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gpauxittw.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gkfhynhnx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gbpqggmtr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gupwkyqom.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gwuegoeyi.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gvmfcskqu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gohvshoha.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqyaxeocm.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ghdeickus.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gscchgfbs.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gbnhfxptf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gjojhxhla.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtgllwlng.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gpsoxthab.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjqfhfllx.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gvehqzwuc.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gesjippnq.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gqjzcjgge.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gechokwzz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/grxtyucuk.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gppggkgzq.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gjgxfzaff.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gdzirioos.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gxzpnrubc.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gcshcqojl.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gijqtnlcf.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/golevcnqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gqlurbkih.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/golrqjlae.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gxxtmiqqg.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gextganaw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gokxhzdre.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gakfacrvj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/grkkvvhxd.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gdazulwtn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gkntjewyy.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gevzslggr.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gfvhkgxob.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gjanxpxbl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gtgbcqcco.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gkclirget.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gjkdgadka.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gnanqzgls.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gjbaagund.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gmxmxmbvw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gtvcsknbl.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gndbjbqdh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gmjlzajum.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gximxcerf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gwnmhjpsh.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gvvrifoyx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gshvoaxyr.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gmkaafshx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/grywjzryz.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gxgpchhvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/guecjtndf.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gamphqhgi.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gsbobenlj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gxsnhderd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gwlgvmmdp.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gpflchdpu.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/ggdwnvtei.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/ghrbraghf.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gcyfouhjc.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gbzciprju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gquifxrxk.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gsgtellwv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/grzcesnwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gjldwlwob.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gizhhwekw.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/ggwwfldfp.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gghzfmtra.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/glweubsda.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gezdqxuhd.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gjgawpoqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gxnicdvrx.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gyciuusug.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/ggdhhoiiz.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/glylgkcff.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gsxuencrv.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gghqpoauv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gwaxmihjb.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gzzvuekor.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gfyzdgjku.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gpgnginow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gyqfhxsmk.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gdipjpwky.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gknzaevse.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gbrrhhqgl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/guuzbbdhx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/ghdvnzftk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gdevkeixt.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/guynylfmv.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gsqnqrewy.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gurcrqena.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gboynentr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gvcwpbvus.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gonzyqbqj.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gbgxxdjzx.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/ghrpftqhf.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gjnbxhrln.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gxafiiycz.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/grewojddi.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gcchiplxs.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gnptuxgyb.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gswuoaner.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/grnijmdah.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/guxbumgad.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gnukqqzku.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gemkuqumr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gjbinvscm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gezvtnrlt.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gtjnmedug.sHtML


<!-- 参考信息 -->