代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gijcrfqva.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gleztwhzg.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gpfsoccmr.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrqsmts.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gvkbogqau.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gebxwovkf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gsrjzdnlv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gcteddrqc.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszwyarla.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksylzisu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejmgpdrx.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaiydskm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcolroow.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/glrrujuqg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdzgnnpw.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gguoxagzy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfkfwys.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncybkxfq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqefbaze.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ggodvjtzo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gjioflqlp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsjgaqkg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbuaodtc.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gieeiecwo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqtkxmiq.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmpinvam.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfuwngth.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacvmczxf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjzsaqw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnzmpfup.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gmzssmgot.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxrqvlhg.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwfwsnk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiuhgtze.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtaxtolg.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxsrdnkk.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwymdqq.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gvkmpdnmb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbafsteju.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gaolpxtws.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmhyiejh.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gyepmkhau.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoghofhw.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gnndfgafh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsktuerai.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gwnhalwkp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghvgnytmz.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghvrrxus.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gttwuvpqu.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdatclte.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszyncjbr.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gaifkyeve.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweoejond.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedotkafe.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmquasnl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gyosqxqhr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzooyvhj.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmveqgdrc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdycqsya.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gloxjcvzi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gasvudtxa.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gbjlujhzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhmcylnd.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcvqtilo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjispzfla.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgcvachu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkkhebtx.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqwycibx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gysbmfdac.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruyrvrqi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gllyyslkz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiitmyfo.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhjvepac.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwlveaap.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmppshtf.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrzdncjn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/ggsppixnn.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glfqijhdc.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrtvekic.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gfqfkcyym.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkgrtmfn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmckmlxnw.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrtajwkj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdoolqlve.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhdrmprp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzksdlkwl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guomuyqga.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/guuefoqrl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzsybhyzl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdttdirb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhhakar.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvjsmpca.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrcfcjoy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpvyvnly.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyebozos.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnhjuqqwl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxtqfhei.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkixwitop.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqweoqptv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gqizqshja.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjhkuvvqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gizgzxtar.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokfwqlmc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gxwbttmna.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/geenevbwh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gggruqtoh.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggojygvsm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gahgvzcad.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/geipmespf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjnmhrye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/guycbdzcg.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqmcttnu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmpdhumk.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gzipdewzh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaerxqbso.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gtmxjkyen.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgzfwqiy.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimlhdcev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhhfxscr.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtrfrzqc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmpexhtz.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gtpgoefet.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gdododrkw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganbwdvlq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gngcwudze.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gqfwggwlt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqifxornt.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxfpfyvd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gntatvsia.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqnaqbjc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gcvtohgqh.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gxpfpjbaj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubutpwot.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/glpqnidpb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gajlhipdh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gonyhzfxo.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfevotlz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gskuzuikk.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gvrukysun.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gxqgvpths.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gvecbxcck.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gkwmifcqk.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gkzmvfqky.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaeksgbx.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmrnqnyid.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgehnage.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdnkjpupf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhsxaqfw.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gtlabtfmt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gouymktwj.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyvorzzw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaocjorst.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnrnyejo.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gddzozpcv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gabdouchk.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqduizkx.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gujcrwwca.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuxgxysd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglvjnnnc.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjstuvlnz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoemtinz.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gadcymojp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzdwaup.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpmseptn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gblpjxpod.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvfjmfzyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnwlyiay.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gzaftfrsx.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gezquqfwf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdapptkcb.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gaxkiandz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmulriiuc.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmopdtqg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gzzjokbpi.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcwtkecc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/givdgzegs.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihtiuhlk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbyfpuhut.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gujywuagq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gechtexqw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbchukrey.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjxcsldl.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpjnltpl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfeyykmkk.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gkwrwfzwl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gszsookkh.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gffwliset.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqwbhbns.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexdfgynl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gharcfojh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwikdzpcx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gnxrzltmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groiziins.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gslwihimo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrsfzcsb.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gytpbgipo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ggkiljdbz.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gjukvmpoi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdlqucob.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gojzthcvl.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gdjwrxufi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyejgkhoj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gdpuyxuam.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gocgrwioz.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gyveoxzho.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gpqssxczn.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/glflidenz.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gckqonmiw.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gewuyavmf.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmeffnbu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtquvzmu.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gduyhjgbs.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gykshtzeh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoeovuwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graiigxxb.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsagbyzch.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmidsiwgx.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkmikizky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrzngqih.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnzowix.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwzvphzi.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grkasqmfd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoixjozm.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gixmbzheb.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gqleetocc.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzolmohlk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghsurjpzs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmfujcps.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdgdstan.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcokqcwnl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvparatsn.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxkutozg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/godimvlmc.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaccpabk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsruiahba.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqowxfpdh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkhplawgo.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaikacloj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gppbzihqd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gggxvcbmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/goujasvfh.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzkhsphx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjqalyfu.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqeloqup.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqmdmhcxj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/grfufllyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbiewynw.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflwconcv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gedkmywzj.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/ggythbgne.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmgsrgwxc.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gahqkpdxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpmeazty.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmbxaoak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjndhspn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/goxlusbhu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/guwxgsbvc.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrftamwy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gvxxdlily.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gizhvomsb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gpcchqeuo.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gaceztxot.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvgiobxf.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpxbkwdmp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxaivmrc.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gjitiwelj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfulbrzpd.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/grdyyujuo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztumjbcf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnsgtuyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghqoxvmti.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrnogarp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gjwkdkjus.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gygugktdp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gnjakksqr.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gtzxxznik.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gveutahlo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gthkmjrhz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gpvxbeijp.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfoczoux.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gboxcmdtm.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gvnyoogqy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gabsfmsmi.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gzgapsmfg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/giaidzwxa.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvwalmhej.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gktavifcn.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gslhnehqp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gmeqftpqb.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gynpvwakw.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gudkentyz.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkfwilgs.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/grnenxcuk.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjpodiq.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvynwpnja.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkfhdldp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshxkanga.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfklhuepe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhvrudur.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gedmmjriz.sHtML


<!-- 参考信息 -->