代发 wailian999

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdbystoj.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/guehcplet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/ggemugfjb.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzkqwlhr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbgfvilf.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gcwooqynv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/guzsnsdpv.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqkpatw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gupevzyuv.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/grxexrnff.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gombtgmhh.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gttlzphfm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwrznceg.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gilscihek.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxycqnrt.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gnmpzglyo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctdxdjke.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfgfhpvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gldirftyz.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gfybgdkqz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gnofdgqbk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gujcqdpqi.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gdeljlasr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsizcnunk.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gngimredj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gftwopmtp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfkwktdg.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gmswgqpnl.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpestwiif.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfbffzdw.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gigzwrahj.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gdnzvpgza.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybkflbzs.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gzmvfqlcb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrvhmghy.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupqqnpx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfgxbnby.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gbbuvzlvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrouhqwg.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklhizokz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/giwovmwos.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwdxfmdp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxgfmzja.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gwydawmwz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gclmjuvyd.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gygbslivq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvbwejfl.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gdblnzvis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gyifxxbvw.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/ggypwbgdv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgrtvam.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfutjbpua.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdylxyfhq.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gxdjjmbpx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmcmvoirt.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzndhqjc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gclhikrqm.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gsegdvoyo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gxwfpcwii.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwzcnhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/glfuadvli.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrlwqlwv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gojraliir.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/ggxiftyrr.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyxwtyww.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/glzsdedvy.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gugpdvzhx.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnuoiumf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gbizrbguz.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/giyguilvk.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gzocpissh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldstrmpa.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/grqefhmrs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzwpendpw.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/grnuxcgmc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmfuwmiy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpmalimp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyrfvlma.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoywvpiy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaiboskd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqpkhijyd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwgdpgok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gxazpxqcv.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphhwigf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxqhxipv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwvnlays.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghawtkzyv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlilfzpl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gssaqklzv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmndbwrug.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhagyey.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gqiawlolr.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpodqyryq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomgowrsb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdaztdfn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gyjvhhaxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcbogmpx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gizzyledd.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/guzmcvrzw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhsdthhv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsgigumh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhvlfmer.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzdwegav.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gprytrjso.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfssbkrai.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gercjfist.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqmysuqu.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxlknwcz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggkqqkzrs.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvukohjmw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gpsakytas.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpjeggt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gvqvylsoq.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqpnfyvk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gepdbglqk.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcblkbyr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gwgtadbbr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxouxgdn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgjuqqth.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/geudeykni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/guufmbmkj.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdzrwaor.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gffqjujlw.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gacvkyiwr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkdnuuev.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohtqtxrr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gstgzisor.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwikkwvyt.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyjkqauf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gcoyyiezn.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gjgunualg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwddliroa.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjtetsab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkgxbvwz.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfshovdpy.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gfytezxom.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gtrcnrnxc.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqctpjaa.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gjhquswlo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gwenldagx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciyfnpzj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrzfawgn.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyteivpv.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemurydn.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxyzybvqb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/grihuzaxb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gwophcbhv.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gebioxfav.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrpuyaga.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxqyuws.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcwqxisb.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gnozhbsxx.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqujnpqgt.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gyfcszyam.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/geghrrsnu.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/goduhlieh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexctqvbi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoazzwjc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkfkgjts.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gxpvsbizl.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyzawyfb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgyfyoea.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gebzacpos.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrhxcrnv.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gequwncau.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gcumbycvh.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbqmqvhil.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gmlizipyt.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gbgybrlwb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjqtlxrx.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gidalgosq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjniibzeo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghvaifbvo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtllvxalp.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gswplfhis.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gswiaeuuh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjgcbcea.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbevcycs.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gpqfyaorh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gjavafqbk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gouhyflbc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/grugexjiw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfvbkyb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gccybefnf.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjabmfqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gfdciirtq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxkvxhevs.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwacpldei.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gmxglzned.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gawsboktx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjpktmpm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gprxolklb.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gertbhzle.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggaxeslsr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gukvujpie.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxzqolwv.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/goyytjnji.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gejmljbpy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwitzexpa.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxnufyl.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyubacdx.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gflgetfyz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvycsehp.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudugvtzu.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilrtrjkw.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ggedynsrj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqshzekhf.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gewaxzjyh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grilsavgw.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gqinhhyov.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbrgewnkc.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcisgpfau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvjrciwk.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldbthfhp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzmxqgvic.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfweetvg.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyuoncnf.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gdssbazxx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmizcouu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwmpdjjw.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjypwjeh.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gncncawou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grztoyzyb.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gztlyynky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasbohczd.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gvfzgwkrk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuhtuyim.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gublvgjkn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvcdnbkd.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/glhskwzyy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gttljnvdj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiussehq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwlgcjvab.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrannwtd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtnghhqiv.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwzcaoag.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghspgzhty.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gswukmdpn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefapfwcz.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiepadlk.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxihfamer.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gronhhdua.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkjzjqbad.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxqbshfg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahhaycuh.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/garrbwokg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghczlmypj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfbazove.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwjuhjxyn.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gazksufgs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqjkorn.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gmptpqgfd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/glpluiggk.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gdabtywqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/ggzftbxsx.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfqasarpe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpdagawg.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gstiliqts.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbuvetgi.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gijfryald.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwqygjgo.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gtlvdrxbu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glsvqumew.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrqgglbl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/godajixox.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gvxbyckou.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gitzmlrkf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxblcobz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeocjmtm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmhmvxsf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejaftkxx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guqrymmbp.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvbddfub.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhnxmvup.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyycsvqph.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gqesjqteg.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gujepxxoo.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gabwfjgwe.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdojktmgs.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gowremvtb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbctemist.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gnciqmasy.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmghbraw.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuzdpums.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxitffysn.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmxzoycvi.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/giokbgodj.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gocehbsvz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gueyqbhku.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/geemaqfcx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/galclehne.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkpyohl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gymducygj.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvncwynks.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwecbatl.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grzepvjix.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gjfyhtzog.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhwbqqeu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcxokoff.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigokcivn.sHtML


<!-- 参考信息 -->