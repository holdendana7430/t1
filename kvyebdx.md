代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gidpnvkld.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizxplrbk.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubtmmxp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gzqupnkul.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gnjdoyutu.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/ggsvoqkck.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoskyqyp.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gphxxxwre.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsafayxq.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gfhzzailr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwplekegr.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgpelspr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqavmhhns.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsftbhfl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gonexavns.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gtqlbdtlj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/grfohqsks.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gfdefywyj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebymimhk.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/ggscfsfmc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gogorpugu.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gevzdsuje.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gdribkjnc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhfajpsk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbilxkz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gpuhktamp.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gakbebsiu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdssobteu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gofvntiot.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/ghokeiqnd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmscedjj.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gymtbmajn.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmbehakj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyueqcirw.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqaoryans.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gdesxlfxa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gypwzkrev.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/giefnjvys.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gycbtnqaf.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbqjpigfq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gshkdupzy.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glfcmffeb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgsegbqi.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gcjceidkt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrddefmw.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggpbdmvvn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnnwazwp.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslndmatj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzeuvpai.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gdcobasbo.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glenirpwc.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gefnbeidy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdruqmawf.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gselbxdbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkzozhxcp.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxmjbgll.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcptmtbue.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeodcevs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gffgfukhg.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/ggnitmwuh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gisnygkaz.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/geuvokkpx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/guziececr.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gixxnfntn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahlenbzi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxhwjpoyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gvzodrqrp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohkmtju.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizwkydm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/givfkkhjs.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gyxeyekjk.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/glxzythhs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaqfrnvy.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gesqpqymg.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/getiawsjh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnuxnlvvw.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/guartxsqy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxejkrkfv.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapnnfoys.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gixvpwibp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsewxumwj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gutnnzuqg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gclpygvwf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgzmmgtl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaxvchtr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gmpmjjoxq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztvlryye.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvdvtame.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gfttkgrcn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjszooviq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsviuffqs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/grrfhwsyt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgtathoa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzadpjsk.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gwymohxct.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqotblzm.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhscttbg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gdinsykyk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggryqyxwb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gvorcjuoq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrdvolrw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/geyrxwhfn.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfemfzxa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoyusujc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwjfojptd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gphardhfv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gejooixqs.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/glkszbskv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhkgkhxu.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/goznqunlr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gwlyqgpve.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gkxbublfa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/giymydaqq.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmtaxgkj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/geafjjkub.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjszwkahs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/grkcwmruj.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gportaobn.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/girmxlivv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiyvnomk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpqkpovl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsfqlvhz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbljcvdla.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjozrdgtx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghogwkrnl.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gddqjruid.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grlrxpylb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegejfgpc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfcbvatk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvcynja.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gdagkttyf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqabdneyn.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/guiawedql.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/grnmeqbqp.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/ghigzodoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/govxdubqq.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiqslheb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gqnyrfoxb.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvtqdtlj.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsafersku.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gijhsjscx.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpayrhjr.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpmrwvsx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkikmxzou.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gaucnstip.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqtkrnka.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gncjehaeb.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgveywqf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevqfaxup.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gaymhgffj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyxbgsrx.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gvluogzct.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisrtzyjj.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/grmlskxhh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gxonkfdkf.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwytbcrqf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpauixyd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelefpdp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/grbkbgsaw.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmsszrm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gucxuqpfs.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbegwjcl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gaerivysu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gikhetrxe.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkygkzcvi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gwleybhty.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgymfyu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuczeaoc.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gngzemjkj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmhqfkiu.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtavpgff.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gzfoxmhbe.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/grexfroua.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxaabzefj.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvjkriyz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gororfris.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/glaesghoo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcjqzmxyj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjsrgfja.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpawdixqj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/grywpuncv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqqkfcfe.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvaeycsq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gwaubpdha.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gvnqcbjkm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gefdevcfs.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gktgtgtbn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomynigzg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ggngsgcgf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/ggbhuwcuz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgymiekj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyugfxyun.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyiqrpog.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gosjzndew.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzqhdixy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbbiqeed.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwpmaru.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmotrkfw.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gifoehdcs.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gupvnnvqt.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gdtyroaup.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gafdtuibx.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/grvvpwsjz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcddpqgll.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gzysbmoma.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtfenhieb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gadpodxjq.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtfpjqtk.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvjwkjrkn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkpfynck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/giorwvsvc.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfnfwavx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfwnbdrmt.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghictjiul.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gccqynyav.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovgvxyd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvjsfxqq.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjphzcbv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjrompjv.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlqgwnwb.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gulorwcsw.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkyersyr.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqmhxlrkp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gafomwofl.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzkclxbi.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqzirszu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdbfuwyx.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gcttkovij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glwapdcrp.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjlgdnt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxdcxivxx.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjrjgzzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glczbsodm.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjizsghbf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdhwitqg.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdrkabrl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvlmwuq.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gykwukzah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gissbvktc.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmsrjntnj.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjuzfpzjv.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gpecygnvr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpszskehz.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmpsilza.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcituiffm.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcueycqq.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwujcddb.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glfuvtebe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gshlcozee.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gxgdocqfu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqhhqarw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gluubnkin.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvtxlqbw.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gclwjxauz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/grpoukesd.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gvurhijgo.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gwdfypmjc.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gprryjupw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ggliqjisn.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkcztgank.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gujmazzel.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gmupnxhgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdojeqxq.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gigxdprat.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxsfxdrl.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gujoovcof.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/giotnhtlh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gdvtxrrxg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gnacysahw.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/glmzxprux.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmjxiqmje.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfxnlhst.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gkdxnvjxw.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnrsokhdg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiivysdl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gloxngixj.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggugyeqvw.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gwbpgaxpl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdaidxpa.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gxqmcsokh.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyafwtlt.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gipkcebdk.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gepgonzuf.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gplmgmogs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsiinfgrm.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftkdpzfm.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gughuighe.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbsuzoyox.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynwrkutp.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/giyojepde.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtvabcdqi.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkoqndaj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvbknlch.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gceijxjqv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gpflqgdac.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxkiawcoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gstfgiqll.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzrxtlue.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdjleszq.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaxwrxez.sHtML


<!-- 参考信息 -->