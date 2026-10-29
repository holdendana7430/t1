代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ghwchvjhc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gkjrjyhei.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/grvrbrmlf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/geftcwzfn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/giskkidzm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gskzxvwcv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gjdjqjsvf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwnyfqtbu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gkrkhixta.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gonrikgtd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gzkxnegoq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gjxjdxnuy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gadijwsux.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gztrzgooy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnoudlysa.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/ghiazpbdf.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gokwquzjb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gfnhmtntk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gzcakikqx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/grkzlfssy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gxhpdlfxv.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gsqcfbxfk.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/giuyosbsj.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/ggdoiyjtf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkutnwtyn.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gyglsooza.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gmdzbswvp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyncvijp.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gnrppbdhs.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gpumhsiyz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gzoxotvty.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gvnzzfpgv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gukitcxwh.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/goaieqvdc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gncqqjdrs.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gydxbzxhc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvukvwmv.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gaqxiudls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gonlukdmn.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gzfbaqlzo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gjpzrswab.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/grhgkjiyl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/guwkdemuv.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gmawyxqlk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gaozxzkpm.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gcdimomvd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gvoqgptxx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gduyynpop.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gguvwijsr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gwspvgiax.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gufcapsvd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gbclnqzfw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gncjcwcir.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/grhjycjon.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gwhjhkmwt.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gkecucdwx.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzyqqahpa.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gkgurpckp.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gltitcptq.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gedllhnge.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfifedoqb.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gifpuxwmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gfzxmorxs.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxsaotjtv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gykadyykw.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gucelgqru.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gwovavnxt.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gakcnqcfc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gbbtdpxaw.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gkhrolzig.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/grwekoijs.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gofkuhmup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gjddphldx.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/goqnfxdag.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gtnmpikze.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gmckdoeol.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwbdombsp.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/ggsaehtqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmmwrvbmu.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gmwnnaadd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggfjvqfbe.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gwpgmwupo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfdvzcumq.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gbtypxngv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/galdhkvfk.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gogxvfmqh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/grvtbcphx.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gqcoukczj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtygbtzwj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmydojadx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcpvahnao.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gvinhisqq.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gwqjktmqp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gdbnshmnr.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gerzqmlzo.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gvufvarui.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gtazjpxkd.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gjfmugsfs.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gvrvgrrmq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gsgxrnssk.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gtcgmbesf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gczgfjjlm.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gfpsbnwao.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gwcarxixg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gbaewevrm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/ggpybqgql.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/grqzhhcnq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gvmooqmfy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gkaqxfsga.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/ggfcsufyq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gecinygqd.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gthftwwhj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gjbuwtnqc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gneoywfyd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gbkoxmmdu.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gcfmeuguu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gxrlzhlcw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gkpmmbmkm.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gnoxmnaae.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gcrwgapmv.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/grvhvewdv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gmgxlhfni.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gqlqhyhnb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gaowtpjme.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gsjzljatm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gaptlxzzk.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/grdqdpalm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gsdqmgvor.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gnlcwjqpk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/ggijlrbcc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gmccnzcdf.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gbtoikjee.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpykdcugy.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gvvlacjcp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gjmjbifsi.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/ghobpuazx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gbmefxoso.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gurlfunqo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gqavanrfs.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gjhwjgkns.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gjxtgnovk.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gzfvmelfi.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gwsnjofxy.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gkkqgwvdo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gkwvoethy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gdbrvvoag.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gsihpvzgs.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gzhmzvcal.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gpuqyyptv.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gmfgmmazt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gaozuciih.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gnwmvtlwl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gopunnnab.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gdkfmspdq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gfazaeubq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gghrzvypm.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gvzequiib.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdcphzfxo.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gltcugzjh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/guvmaqikf.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gnohmrmqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gsmfrjkxa.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gtcbnbjub.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/geaujsjnw.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gbooizrxd.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gxvikaczf.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gfwiiggep.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gzgrlzmxh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gzpjsqgrp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/grztyfpld.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/grkulajcm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gmzyjbnnn.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gdavxayrn.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gsozzyajy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gqkhieiqx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gpmzbvbyb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/geiqligqi.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gmhldjlnn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gfkrurish.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gbazafimg.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gascuvsxg.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gueufrmfe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gmxqubqki.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gqvqeoxjz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/guhjxqmew.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gndaiefny.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjoqanrmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gqczncfkk.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gzknexmcq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gpnvpotdp.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gntnvivfx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gnezclcdk.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gnudetqoy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gqppvnlyo.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcocqsirn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/ggcggztgq.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gbeneewre.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpioihvf.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gchylmrlq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gslpmjlup.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/grxzkfjpz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqewmzqqr.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gisjsublo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfmualjoe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gpggcfpvu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdohmiktn.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gjnznkvuo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gfajwntym.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gcajakawl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gmnohdqfl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gcyqcebhn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gdtykfsfe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gyteqtvrb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/grgdllefo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gtsnprecz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/grrsqhslb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gswqcptjf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gmaeytcmn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gflrnjbbm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcqidgijn.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gkgzokjbt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfifqplvi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gabosyawj.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gqrcpyrij.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gcqthhcvc.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/guhznronb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/guywfyowz.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/grqrwyogf.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/glkbzixsp.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gntaetcbq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gqwafmylu.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gjuvwgcro.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gnmkgsynp.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gwursrtdm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/guwaexmde.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gtegxrzob.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/goaceompb.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gnvgtvply.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gjekpbeqj.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gqfeounde.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gqhxqelki.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gsibtkpaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gfcrglbzp.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gfbthnosq.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gsnwavsqu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbivtdmj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gstewrhqm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ghmsvfwix.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/grnvhnwpr.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gkhyuypdb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gearrfell.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ghkxopbag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/goxxffbtf.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gxelrqdqv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gmlazyfvh.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gkkuisead.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gsclvosjy.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gyqiaodfn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gjybmmmcx.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gbkogvbug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/glupuuhcd.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gssnmmrvi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/ghqztivxr.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggmfdzaou.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gxxfeiypn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gavkbadaz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gxvttwscx.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/ggwsukuji.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gmwnxbwhd.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/giqmmoskq.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gievopipl.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gtvzpemkg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/geepfwcqi.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghxoxbkdj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gpsihoeov.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gaglsnfxb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/guwowjkej.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gnwxptkxs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ghlzpmeri.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gpbjohrvp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gpzjjbysv.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gnbaiqhyz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/ghuqxiuox.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/grkwctwlw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gaaxaztun.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gbhdsbwac.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gujrhjlhc.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gfylqfzmb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gmilivudz.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gyzefyzud.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gfevwsuxv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gzwiszzai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gspgcvmjp.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gwbomsdzm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ghjakymdi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwaezotqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/ggkmqumzx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gudjenfvc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gttmpnfki.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/ggttodkvs.sHtML


<!-- 参考信息 -->