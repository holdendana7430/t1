代发 wailian999

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobyuygmn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnvbdpar.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijmerpyz.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfhixhrq.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/goxbtnjwd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvgjrqtx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gkkhfluoj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gtxtksqaj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gthogewjb.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/grjmpwtju.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gubdvramg.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gputeezjv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqbqsfzy.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqzbcmml.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/glmzblgob.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gqcnrsyno.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuebifed.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrswkula.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcztopsiy.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/girksyjwb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/grytqxgxp.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlcsdvsm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gebksoeqp.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/getuserzo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmayuneu.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbemmaby.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gjhbxselp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjijjtymp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbbnjmpp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdzugogp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtpfngnm.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbyzwrnh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/geocznwih.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/ggtmemvko.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gqglwefux.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gsqpstndf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gkbookdln.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gdxmagqfz.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmtsdxfr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gcrxzvymp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoizvtrw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gkxabkzgm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gylqmwzhu.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gvwdfxibv.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpdgyvfqt.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrotizmh.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gesdkuhjb.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gohzwttcp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gajinkefw.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/glfeygbvv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gsdehhvqo.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gerncyaan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gmlddoems.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gtmllhdor.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnlitrisk.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxonzlkx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxymttlrn.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkfxyxgas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgwjncn.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gzwfckong.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gcjihwghx.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gbebwlhdo.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggilbktbn.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjsjzqdl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gxomycmwr.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gqfgkzcxr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgmvzbg.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxppkacyo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzabskji.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqbzpako.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajnxexkp.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/glotthmnq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvcxpxgq.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjbxcjqm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbxepyqi.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwomkesgu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/guoheqrfk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/geskbcbyc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsxehakk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/glgnzpudg.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlqbsugo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtqdksbj.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/grzynssch.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gfqzdlroa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gcerunwzf.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grgessgri.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddovvqhe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadfrqils.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgdsnos.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gayxfosiy.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gljgeenij.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwfapgzg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxobjzh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngpxzpsz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gastaxgfg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytmwgck.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxckdrsi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjjicptm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjmidajd.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqiivchz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/glazqbrxq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwgoaski.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxilbnkff.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/guvxtwkhe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjoevowq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqqsxqnrs.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpolikacr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girnsbhss.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gziadjpcn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/giyxcbzbx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzqbmwoc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxqooerpa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljhasei.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxixdcne.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmgnvoee.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokoxnonh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgdapmzj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddgysrpd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpjkxkmf.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmfklaph.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgghdmpb.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpyvmkjb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxreteydm.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gadqoauwp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gppqpsdll.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gophzcuue.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggevbxque.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gybidjuuy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsejjfnko.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvetrnrc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gacmskhyr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gajsiymdy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsnjizjx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnaoxwvs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gkotztszt.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlzstblu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqtwelju.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrxikwip.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbnhylnfq.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvhvkmku.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjigjvike.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdknndwli.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gactncpca.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbnwtnlm.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gfzjwmugu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvxwzjar.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/geejukpon.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvvwsrqs.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdjmkubp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdeazdsu.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggyhloief.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gwocgnyoz.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnlgfxhks.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gfpllhnlx.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gagkvfpxj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gnndaipav.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gjfyfeujl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gdyqvjibq.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gpddwvcbi.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/guwtsvpyp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gikzabizg.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtediqnz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxztlabvp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gavvvurmv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsggqtxw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnuvwfdy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktmhgzms.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gdxgzxrey.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcgjmewsh.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvhgzbio.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giugtkqil.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/guhenuluj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/giwekvbio.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzyirgcjz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfttqgujn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gsnheevmz.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gbukehlhx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebgxhub.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzgoojsl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmtwnmgw.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gynijyxgr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gigfgvzqb.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfygawzl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjiellsh.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwobmxtt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwedlilqk.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlgugorh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmyrrdxhm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giqjbzlim.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigxxqvwt.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gydqvvoru.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuptyncs.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/grcubysrv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcdcwlzi.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsrvegzt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvhvuosp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexgovou.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gtblbxeoj.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwiwxdb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnosmlaui.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqsstxof.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gqvnuhnfn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gecbyfdwm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupyaeseq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyarymjrd.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjobjrqeb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gygiorjzl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gowescbsq.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkduowtpv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gukhswclx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gorelgmzx.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/guhdxltrz.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gyopahesz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfyvrkgq.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gfivlcsrj.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gljtsgpou.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbjhvqgy.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsguhetp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/giwnwyhli.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzejwfuez.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnecodntv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwjkvcin.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gssgbempd.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqldmwoq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdhlokucp.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/grhxretlm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsspqlvd.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcziwymid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhprphsk.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/goeovzvmc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoznmsbl.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjpjehnk.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gkspeshne.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwxgccc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqbtaouu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwzdvdxw.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gyhgrgahh.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvkmtfttb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnkezohh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudgqnqiu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnyeabbuj.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gpzmiwxgv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsinqbbia.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqeiyqyte.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxsbvkvku.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhstjdst.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzvcylapq.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkpefvjm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxasfdro.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gauamrhqf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtepuljq.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqtkyocb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgaumpve.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/grlwkhhna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvbatkkej.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbphcuaa.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtglisdde.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeyzzuey.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkuemksc.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghhdpfgky.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/giqovhysb.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/giqsoilnn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbbsvflwm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gkupcpovt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gruddxcyh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwtavcol.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqrvrmjb.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuvktzol.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/glrqbmjim.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gftssvrmf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gmjhzcljt.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gffbeponc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwywjuiih.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/grcuqzurr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gwkpeicnc.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/grojzflcg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtqfmyrl.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glznbwlfe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcaubuysa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpkbmsgp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gobjtgpir.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/goltezqws.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gtorbtivl.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/grspurldu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbafcemg.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyervptyg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmdztehl.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtwtiqhyo.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhkejuvo.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzbchcgw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkouduhf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gffkgguyv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gorkqitfx.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gnuyhyuvy.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grekrgbzr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwskzdiw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ggtwdjggs.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gyurhmrrr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqddgkmeb.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfdjjzazk.sHtML


<!-- 参考信息 -->