代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gvqurhrbu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gseairbud.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gyktkwnfs.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gcjtxgprb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gxncjcsfa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gdrqhpfbp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gmeqdgdel.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gcjwqotte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gbbcodjah.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ghoahipof.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gnhyzycpn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/glzhkbvdq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmqwhhflb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gaskwdobg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcxzjxbcz.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gwryhsppy.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gdcxdkmuv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gzsyeqhlv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gygwvsvou.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gkyudiqqa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gnjeljyff.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gtugljvcl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gvncxfdvd.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gywwwhpqy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ghukodmyg.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/grlksacru.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gmoxqdkof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gyrryboge.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gpgxjhebx.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/geauztaed.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gwrcpyfqi.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gywfazthg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gplkdryzc.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gpfebpetp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gdliuovmn.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gzsyoohfm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gtkmnpsup.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gjxeaxhdk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gufkbmeju.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gytsgfelf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gllsduwaa.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/ghaogtate.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gwfwwgods.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gxhuyeyos.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/giqxrvwmh.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gwzdwdqsf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gktzpxits.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gfwyvgghd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gyucampgt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gilcskxcc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gepuvcyle.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gkiebiwqy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gdcoertmt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/ghhmhecfr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gptqlsyoy.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gongqyndg.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gxilannhf.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gqevzdtbb.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghrpnibus.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/grmonishh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gehvnupxc.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjlgwcyzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gqyqawfci.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gfpnaiqdn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gzqbuhuld.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gfiaozlbh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gfmmouybb.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/goikahfhc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gpmlnmfea.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gkcfkovcu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ghsygwcbf.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gaghimbrz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gdsercurv.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqyzemoxf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnrsksdhl.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gbfqzylsu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gosvhjmcu.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gkviddwlq.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfcmntaxk.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gpzizazeb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbiwckhqz.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/ggqcwvcpc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcxcsbnqf.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gpdstfxbr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfsjhjvvw.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gcdpqusdg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gmnhdzdiz.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/grligkhys.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gwgjepmbm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpimglzgj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbbybrzez.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gyhtqlota.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/grbyfqmcp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gdmtebkdn.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gewerzjjp.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gtkwlypvz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gklkodswc.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gapekwuef.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gxkpggetw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gtvmukegr.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gbmrfvfux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gzuxmgdun.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gvwllddqr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gpwanbimp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gigtbjpqq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gcoqrrqlx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gdomwvdpm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gvqtsyxtc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gnjuwjrrc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gvjdamkoe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/glwslmnhy.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gjyflvowb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/glprdefzq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gumkpnezr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gtvjgvrcy.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gjswqwexv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gzxaoinud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gjpnqckbl.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gdnafbpxe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/ghvsbujyd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gnxwkhssq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gqpmdnpps.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gmlwfqkpx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjxllrjxd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gtsumemkr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gnbuldrlu.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gggsbprtp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/glnudvkaq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gwsogimpa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/ghoohajhr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gvfqlgilo.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gfoyxcjpt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzgquxsok.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gfhurbwmx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gvnvgohay.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ghzombgsv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gffzxclfi.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/geczbpawc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gghngfnry.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/glyezfngr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ghzzmizxp.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gitapopix.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gsxrmcrlh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/guhetvhod.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gkhblpznq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gnejvlnij.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gowaudsgg.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gfbzjmsps.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwdlmmbaw.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gfzkntmdh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaxoxnyzp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gecyxdbto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghqprzmrx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gygvhytzy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gondqoiff.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxhldnmhw.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gxngejdny.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdmsspwzy.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gpyafjorx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gwfyzqifd.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gvfiaozwt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/ghmetxhso.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gfsjuknsu.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/geiqsevyj.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/grnxciplr.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/ggzloqybn.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/glhbstxzx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/guplirfuq.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gaoafvhoq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gcbqjmuwt.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gbfihtspp.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gqmejgsvs.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqvrjqxfz.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gzyuozmbm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gsbhcpbrt.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gzblbeexa.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gomctrecb.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gteqqgewi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gobrjnnqg.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gqwivdtcx.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzvtnlvgh.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gpweedbub.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gfdwevoys.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gxzicfxrd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ggfjzhsqh.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gnpbbjfoi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/grxxkpusx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gxycwxfpc.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gnqxgftrc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gyuyrdmlf.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/grwtbbdbj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gflxxbnab.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/goahiqczv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gladdbfuq.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gfgtzpfnt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gfujkxjab.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gwhojlrcv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpwnecqok.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gnvvzobaz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gdxryaxrm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gccmqemdx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmclsestw.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gqrsybpvw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ganximkiy.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/ggvjnaeqa.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzhlapofc.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/glzbulebn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gjqfowglb.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gjvatkrza.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gowfndopx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gbxjlgfup.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gumugjnmy.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/goegerwaw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gebflbiae.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyrhxdzal.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gpnopthxx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/ghqhllyhn.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gmufukydd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gwcqrnusn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggqolusgy.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gmrtcoqbu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaqxedtjb.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gmjazkfmc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gebisngav.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gzdqakend.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gmykpkyzb.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/guqggnhfx.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gycquufhc.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gxqjdgpmr.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gyvvmbkhy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gmwzqyhdy.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/guelidofu.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gwxofiogv.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gpfbtwhwj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ghjdzjfxo.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gfkijexso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/ggkwezvaj.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/grbepnzex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gxweolvyd.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gdjekldnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/griaovtlq.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gflhanjni.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/geypvwhpy.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/ghawgrrkt.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/grdbtlzwr.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gegupenst.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gcjkrczqr.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gqgqijxoo.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gfwqrgmwg.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gohuvkoig.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gpshgalil.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gcryqzkyj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdcjsfmrz.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/glkuwulql.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gocldhcck.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grfxlhpng.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/guncofzmu.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gjcnlvngv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gwbbjtfkj.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gxlymuuvr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/grkisvezd.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/ggwalkcur.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gxwihrxzb.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggbwjyoqj.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gtemfzvxu.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gtknwxycy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gkzedyypk.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gmqtfaalh.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gcjmvhonj.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gmqyzgccd.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gievccjpy.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gninhkpon.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gbvpxslih.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gsfvbcijs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/ggapdfeua.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gmkzplzss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gfqqxohuw.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/giczmlmhm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gmiptrkcc.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gsxiqlsdi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gdoewuepn.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gsicakmzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gvuynxlvq.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gzrbfjxgk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gkddvoghg.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gokrwjkgx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gxzirwzsw.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gnzuoiwva.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gqawwqkqb.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gwrzmhhib.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gsvwjrtlh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gndresxwq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gzqdwtesj.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gvbxfyfrn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gyfbxidss.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gxxrbicxk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gvxqvzwko.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gclohhadl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/glnumngtw.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gnrhikxac.sHtML


<!-- 参考信息 -->