代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/ggaziylcd.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gqbbgnjal.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsnubggs.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaasvrnt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwuujza.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gljcbyqyh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/grrnpqbqy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzellck.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/goslvryqi.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqjolctc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gecbwufjb.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsssgklbw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvpgdgqx.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjccxwxm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gisnjavvl.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfrvqwuv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/giifphmnv.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gamgskkda.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkgeblqh.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gwyikhaqf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtwhflhz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grpsqdytg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqeiptsy.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvtnabpt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gepkgxmyw.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gjdtvtbvr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/guirbqzjb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gtpjpihvl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtondjkgf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcczqhph.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gxxofsafy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqttcmdes.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpulkbxh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gjbsbhert.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gscgljrtr.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/grsjklrpm.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhdfltos.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhgzgepc.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzspesclx.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gzlvvivhq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmlacsbp.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjpeihbgf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxojbhuje.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gphoirumx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhlydecm.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjistbuf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozxgigxy.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdjetqmgz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpdqltqr.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsrxalqi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/giuzusqog.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gbuspaxba.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjhbeia.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbwkjwej.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqmxovfct.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gsmdvwicu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gzwcpdunn.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmegpauj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvyaolbu.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gyvqbnaac.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrvkrsrc.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrdgnrbe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurgozvhn.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gmyhaxiee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddbhjgra.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpzylyip.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/giabospme.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqsgbhef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbmwocnj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbanpmcxl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlxehpxr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gscdqnkkq.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsonhkzt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsxwejzw.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gekigxtzi.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjosddno.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwhvjzo.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbekgibyh.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/glsrklkmk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gheuwblhi.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gctpgcfxq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfjsvkwx.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwapbnagh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaunmlfh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyuedfuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbfwrpmr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfqyygsx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gghzoqlgq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gyvkbcjyb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/guyzwllok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/grrittpip.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyrwilaw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/goipljxpz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiejcjrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gztajvarq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylqdlfkj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/ghixrdvtb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjkizdhl.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsendqyv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjztrfolj.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/graalycrl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gouljynkn.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtvpvokx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvxwuztq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwatmeig.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxlinnomf.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gnryjaxyu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/grrpygdyr.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/guemrzskb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gukzvzgph.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gspkdhdjt.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gdowekcgo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/grlioxkky.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gypgvpkxh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gylezcrto.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gffjqihpk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbqwobkcx.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/giomrvuoz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxtbcnok.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrpbwhqp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvomlqvms.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gjytasxqn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhgezora.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuljomus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbcspes.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/giruybmfb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gntgwiuke.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gionchmnf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpspkclti.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggezcrelt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiysvzvb.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrotogiv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyttasitk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gkponiktb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgjafvsw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnrabeanc.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gauihrseo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsyfdnekr.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gvwlmdwym.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyyxsarc.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjdwqdnaz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqysihuq.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gbmyzahmb.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gerrieksh.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gtsmqsqdq.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrjhpala.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gldjhodgq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghhuylm.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gxfoquoms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwulxoym.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulkfldqx.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdslmcqx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcrbmooz.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ggekughdq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyewqpyi.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gelggczpp.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gleknwukk.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/grnwdyikt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gmwigexfa.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxqotsfh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjmjpcgk.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gwvbkbbgs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghsubklpf.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvdcrnuqb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/ggbgrixvz.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsanzpfjo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzztovzwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpuektwn.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gwtwqbdwn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gesoicotg.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gwadjhdgx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gckrizixu.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtedcjfnn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gdrtieyap.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicgrmuil.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeqmlvfl.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevjnbbyh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxevoljjy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnwyjxuv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztbrjbtu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrcsfiyj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzlezkmb.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqyykvna.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqyzbywk.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gyaftarvl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmuhhrxu.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gczykbghd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gctjqngkt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoeskimd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjmabccx.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/goyjlhhhp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gafftbkkn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gqblmkbrj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gizsnwbid.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpryrzvnf.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gndmjattm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giewtbced.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqjavclu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvmcqsgx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggjwxvpvn.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpxdqjac.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gobswepsg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqegeniyx.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/glvcxnhba.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gifkktetp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gieoywihs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuqnmrmb.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkvbduez.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkvgxbrq.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/glogpktcu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkoqpoypy.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/grmzrkrlj.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjnevtyn.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gcauqujtv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbgtygkhc.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdpqylfs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gezlcsluk.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gddcclihj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grkxnnrnc.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlagays.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqerqxjv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gpcizyjyl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozzblxe.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/grwkhyyha.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpwtyvft.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ghtzitzmx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcydsskl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gznztlvbt.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpmiulvb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gormcjhgt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjemgkts.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjctetbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkkixczj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhstursn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwabpwjqc.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfvoozutk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkvjttts.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfjxnsav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrnloenk.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gernhjqbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gicbknlwy.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gurzyfohs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyhuzbfq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmzkgwet.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzzrjdpf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjjalzss.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glvfqcifq.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvpvpdeo.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkbybhwnx.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/ghexyfgow.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvkmpewp.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkbqjnjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakcqyuud.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbvelagt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gisvbrvpn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gtfjqcpsw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/groelbkrh.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjcxkyuhr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlqewclw.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygwodapc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/glstsdmmm.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gmpeifsdu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzomoiwe.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggggqqlgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfohktit.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmmabmyiv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/guvneolsu.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpjrklmc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmogdbvx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffnedhy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqsqklrp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gxqioxxzu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gfchflcco.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuwibmag.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gjdfikzor.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ghkepwsiw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkylghp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxowkfdg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gjuimnnbp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvlsgrdz.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbqvbprw.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gmffgpnwn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gezsllvxz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gascppwro.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gchgluakv.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnhjffc.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gekhqtexf.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gzhmzalic.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzcuwhuo.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/grihrefck.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbywticv.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwkegica.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gtupkgxsp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbcyisbp.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqquxek.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/giczgdpqn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeoctysp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxnppmtr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gbqmoekhz.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmamjxjy.sHtML


<!-- 参考信息 -->