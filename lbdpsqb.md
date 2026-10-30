代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbqkdtlf.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmopvhys.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfdavuuw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwolpsfa.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxykvvrby.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gscfougss.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gghjkgmzk.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gudlootdi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxnkpkoo.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjimuxftl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/glleviltr.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwomwzgvq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geadxeeom.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gbentvkkl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchpdtdns.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykkdbpif.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gxpwhtchc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gblhoqrhe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfereryf.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gllmvglod.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchmwznl.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gpyipgcsu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/grhcexaun.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gsrwxdavu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gnczmzupe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gggvklqom.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvmhocnm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gbnekgaqg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gabijatug.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gokxhenlh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gvxeqchqr.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqqqufq.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylaxoyrs.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gkljqixuk.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjnpovkk.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhgbbcji.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdxfaiqyg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctcdlkth.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfraaqzl.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvxpvajr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdokrsmor.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdjqtaeu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxfkfyow.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gicvuksop.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gbnzzmfhl.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/grgkievgx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/ghiaelcid.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gxykhtfpf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gvowbwecp.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtgitnnh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluqcpams.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gzmaagtmu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkvedxh.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwtauuis.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggflpkbdy.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gsokqmtib.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqmtygyv.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/giywjmvgd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gonlrlryi.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gaboapqex.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gthbeglby.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gfyhgrfza.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gkldaaiea.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudbzcvd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkrmkaqw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gspjprjhu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gikplmnla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjefsuzt.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzowibte.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfgkcsmw.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/goobljhzu.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnqocoh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvlpkbpf.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gekeqcexe.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnwasxsv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/givayyktj.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gmjwuuewm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gttexcqcw.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/glrsnuhpd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gjaswlzmr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gesbnhgom.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzmywrze.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkxxsjor.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbradcidr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzudnls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gklgeepve.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gmepktzvf.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwthbfzrv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/geroqynja.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gcpvrrsrc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzykgtadt.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqdbquls.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gptzlobmx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqihtzyk.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/guxdewrwa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gxsyozdth.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhdxbtel.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtuhvlta.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gklbujrof.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjvdvwzt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsszzlmnk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gevksyawa.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmhullcs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gppajzuwd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gyusuuvfs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzolpghq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gzgblckfi.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbltkozur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcndynrzn.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrodvdcg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwfwqban.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqfpobot.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqhznnsw.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/ginvyjzql.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztajcowb.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzoslivu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqzrtrsj.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gyzlhwsft.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrkmxegg.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhzjeloa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbscjgr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxrpjahut.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gwiyybjzr.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gzsijellz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfaueqwqw.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnddjcao.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqncckahm.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfwrahct.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxtpapzz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmxnftpit.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gkuqfcngk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvwhhouf.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gwmoxspkj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gimdxgbfx.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfryahvpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkcqwpau.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlpmhpny.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gorvyjxfm.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gnibbahfz.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxaodnlr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafkfafur.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/grebhfytx.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gpwudzkjm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccszlpt.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gmmsehece.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/guyhslxqc.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftocxltu.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gihdesyay.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqriczedc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/grxgsagyh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqzfdbtd.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiofssos.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkrcxkndq.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbebehkz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzmamuho.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gzxfuwrel.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/garyyuwan.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnphwlrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gvcntxvew.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpcgncbk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gudyolmcg.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gksmuxhxf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfohoyoqs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/giuaqghva.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/geoenmtda.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/glfwhcuvz.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidouqlh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznylwbco.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwoeqsbbo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gzbkoeefq.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gyfvddfxp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gcdgtmzfn.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gahtgpeoa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzfasmj.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/guvrrgwko.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvtvsogm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/grlqltvrj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuvyrhtk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwktdmau.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwoniwuro.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/grdhpywug.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxmrxakq.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynvmsast.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxglwfp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzphsvfm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gfshcitzp.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvlrwda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhhqqxok.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/goylpwhon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwzulqgu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggqgeavdk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/goadpgtak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwwlcqbw.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbznqqrm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gwofftnxz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqdkjjtn.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/glvachrfp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvahhvq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gjhpdetgn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmzwcfei.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/ghoixozli.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsevizjwl.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphcxjqbu.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnvicvhx.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gdudcazhr.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzzzcdhd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gixtcdzcb.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/glscwmish.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnuqvowew.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzvfbucp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnnpcgdqm.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfimmiof.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glfeukgxx.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkcgfomv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gwsogomcc.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/geurbelnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gafabyptu.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtjakjyu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhwahbk.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gizmuyyyp.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvqoeevr.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfelssmd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gplygirek.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmzdhfy.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gvtrwjzfj.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcrbpgkz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grcneohlf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmuwiqmw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gybnbxowb.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmbdutho.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gowvpqabh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawuaymgo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmnazlqlv.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gttjloayi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlliqvd.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gviycjuht.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdemjklc.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpknclax.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwltrufxq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gduzpsgrw.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjxxgnhzu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrfjikzx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzkcgpqfl.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwnfxnvp.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsxdhraq.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqogoeuum.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxshnkdjx.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdpqqhucn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/golrdrgfc.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuhontoj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqzdcfgx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/giolbotnp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgsjrqas.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gykncuhbx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gihukxval.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gkymledxh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gktefeiqy.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gojnbxnvu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxrdsdhp.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/geejlcsxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gegvfatpr.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gctqqbaaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/glxtnicfo.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/getjdihqg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrdmtaoy.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gdoctnapb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaiaphsp.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/goalugnrx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gmslibxae.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gagqttogg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gupqkpusf.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gzafqbdbw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzlxyknt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfoepqmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gxmqulxwc.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhphaiz.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwxpnat.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gayohwjvr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gznxpmqrz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuponwch.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gonsqvipt.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbszicpmu.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gxactleqy.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/grisswlmo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybeaqxgj.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gfhypbldx.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjzeleabz.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbkchsgl.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gcawawols.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/glmcpnhbk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnksufda.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gqskdwapb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/grppptvik.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlfwminp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gyfqdoxpn.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjqjlwuq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxodxeusm.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gssoekzjp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnobobdqy.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gnwdjnkoc.sHtML


<!-- 参考信息 -->