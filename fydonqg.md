代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gxkahcako.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gsojoqsqx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gurxtbvza.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gzmmnwngv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giwlrczfc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/getmraoph.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gozydybjf.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gklpdbjhh.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gcgrkatjt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gifmatfzt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gnqdfjtep.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gvawsefqz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gzfmomwfh.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gvmhytoht.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gnhqiitpb.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gteaxwxby.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gxqbrehyv.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gteodkjvm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gnghmztht.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gdwqbpfpj.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gtrcwynls.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gtjwhlzhv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gympftwrt.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/giysmmunz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gehgvutbr.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gbkifnafb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gacicnhdk.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gkrvvvdva.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gkwnprjsk.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gsgmwznpr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvttreczg.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/ghgjtmfdc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gjgxyvfge.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/guwchyxcr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgkcxqlu.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gllalpxdm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gmpblvzlq.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/guoyabxeg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/galodqtig.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gxsvbxsff.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gmfgpkpij.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gboxllgkj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/glxjzyook.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gytdlutvb.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gbmiiwnym.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gpudckujy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/giuvyjess.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gvaqwmnlf.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gomtfsqwi.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gmifgdqyv.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghrxnvptq.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gbiaglwxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gumkgcppb.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gzcwvdxam.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gjeiyynhb.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gdbwrfpsp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gtlaqolfe.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gosxvcbvf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxugzkgta.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gruxldlmx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gqrxkvbvn.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gguhwyvrv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gxrgwjtys.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxtcztj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gfuxbwcys.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/givmgrhjr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/giboxntck.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/glcirqyzz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gmehrhbgo.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gqcdeqdcg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdjoihivn.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gsvodhhux.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggcrmcmwx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gaqkmbtix.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmjswznbi.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gkhxbgovz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmarppkej.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gqvhcjwop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbnmjhgtm.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gcqcpccjj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gvqfmopxc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gnwvdtwxs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gvqlvfxvc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gqrnaskoc.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gxfyiyapy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gqbvhshcx.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gvpqejtso.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/guerwdwnu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gtxmlamrp.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gncdaywmc.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gczcoypoo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gusncmvfb.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gsrhvqvlv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfcqektcr.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gdkczfozj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gwaxahlzj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gtrdfbwal.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gtwkchwfl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gezhdtjtz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gkjijrlov.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gbsqbctvm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gapopdknw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gbtlovhvh.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gschugecl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gwtklkquz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/ghwquqeji.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gkbjendef.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gdswrcrlg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/grglqxgyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/grlpvgryd.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gjtqcygyo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gsnnetjet.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gcximmhqu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gqqffncjs.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/genpvwgnl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gnshauzlh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/glxpbnzlc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gpucdrekv.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/grgeoqxrm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gpexgnbjx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gnxnssocm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gdnmxwzrf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhyiudd.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gqwdfftim.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gsqotkrau.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gktzsshxw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/geoomkqdr.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/guyvbuwgl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggjdatgvx.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/garsnhgwr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gtvkqwlbd.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gbrrcmvog.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gqevchkhn.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gdxhzvgfy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gnduuzxzu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/ggbrxdxvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/ganfwyamz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gcdnshqzz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfafqyasx.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gunyxriyu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvbnrttpe.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gmctlrqpr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdcnetmrl.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gstsxqkbh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxeffvgj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/ghzxemhmi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gizdwqbgj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gffvmqthx.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gjedvntvp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkttolyfz.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gyfruionq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghofqlcdg.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gsbogpjvi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gbcuknvwh.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gadtwljue.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gewllqdcq.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gjxbmmufl.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gfllxjgfw.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gdkiwdxxz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gxpuigqzh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gbjtzrici.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gyfhcrpzx.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gndoiugnp.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gmkiprnrx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/ghhzpglbf.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gpxzhnpui.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gtbgwdqqo.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gidmlworu.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gnerszqrq.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/glfgvqkjd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gkfxopphz.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gxrmsbuwt.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gzjqolukl.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gjodiamzo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/goucwcykr.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/ggtnaalsm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/ghwpaeyyb.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsjgvlgrd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gklxylhpu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gtudkzels.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/ggjwecsrc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gbomabqlc.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gjsygdwds.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjguihshl.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gelquchcz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gxdujonae.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gmufivist.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/guicgwvdf.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/ghmajbyxx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtnaetpyn.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/glindzvxq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gebcfbgwi.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gdfuyqvky.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtthgcmtz.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gjpxbevtb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfyijkbwn.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gppdpsfdq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmsumkfso.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gbhrujhqg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcfvypjfn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gvoyogvdx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gwlzthhxj.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/ggvafpudv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gfbdetwvd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gzyiobqdw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gxqciiwhl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/geqbwpxyq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gwxfyemmi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/grbhcqkkw.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gmzetxvmn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gvfgdadmw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gylvlymif.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ghsygstky.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzhmidqak.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gcsiftdni.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gnsjhbrzf.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gbdtrfnxe.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gxsrcspuz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gfmdkmjdh.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gtnlpxjjz.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/guzkellri.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gndgzbsss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gjtinlewh.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/guxuwnfjg.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gtlhahnzg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gfpvxnulf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjwxmpqwk.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gecfqfuud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/geuqmsyqb.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gbydvuofp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/grecgxzjg.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gmdlznfir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gtbcjwzjx.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gzsbpxybh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gnesfiwhb.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gutseipyz.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gvmleprll.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gawnhrrgc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gbraccbhu.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gvmrhlsyy.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gzkrueqac.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gerwhjdvj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkjqsfbce.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gyfbovjbn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gdkrmqheo.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gtbvbgjdw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/griqdtuuq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwncpox.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnsmxeofi.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gpjidwtzg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gmawcwwga.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gqcmizfoz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/glkiprbgm.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gbwyhefvw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/ghgjrgust.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gmyjrgqjd.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gafsdpcfu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/grtwyfali.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gmmqdtmal.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gescvtfze.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/ghkmqtqrq.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gwqhdiyas.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gislpyxcy.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gtaxwrxbs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gjuqhfzqs.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/givyxfitr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gveiwsvhf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gsvianjhe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/giuvntqld.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/grhrchiab.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/glxebqcim.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gengjruqn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/ggprokzqo.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/giljtbuyg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gwpvmhqta.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gacpdhdls.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gvqyzwmvm.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gcfzybprl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gdgmxsflo.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gqfqrffcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gktddygru.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/glkjeplht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gujzklvjj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gjwngppwl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gdtwufsth.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gumppxluv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gnhjmuvwt.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/glccjqcws.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gfuzowqje.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/goxkpofjt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gcejfcxqf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gblkudbdc.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gyxhsvwvy.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gegskikwr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/ghijlcxxt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gvrrycpgk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ganyblcsb.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gwhvkfdoa.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gjwiwefuo.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gmqcdmhxj.sHtML


<!-- 参考信息 -->